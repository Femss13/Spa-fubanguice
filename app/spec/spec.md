# App SPA de Fubanguice

## Contexto

Criar uma aplicacao SPA, com a stack html, css, JS puro, sem pacotes ou dependencia para hospedar no GitHub page.
A aplicacao sera um cardapio, estilo "lanchonete", porem para coisas futeis de hoje em dia, com um estilo de consumidora da virginia. eu quero com produtos do momento, como morango cristalizado, abacaxi dourado, sardinha com muita proteina, itens que hita no tiktok

## Recursos do App

1. Carregar os dados do cardápio a partir de um arquivo JSON contendo
   todas as informações do produto, organizado por categoria, com
   destaque para produtos em promoção ou kits "pague 2 leve 3".

   Critérios de aceite:
   - O JSON possui os campos: id, nome, descricao, preco, categoria,
     tag (hit | promo | kit).
   - Produtos com tag "promo" exibem badge visual de destaque.
   - Produtos com tag "kit" aplicam a regra: a cada 3 unidades do
     mesmo item no carrinho, cobra-se 2.
   - Falha ao carregar o JSON exibe estado de erro na tela (não quebra
     silenciosamente).

2. A aplicação inicia diretamente na tela do cardápio, com a lista de
   produtos, sem login, cadastro ou splash.

   Critérios de aceite:
   - Primeira renderização mostra os produtos sem etapa prévia.
   - Nenhum dado pessoal é solicitado antes do checkout.
   - Estado de loading visível enquanto o JSON carrega.

3. O SPA usa localStorage para persistir os itens do carrinho.

   Critérios de aceite:
   - Ao adicionar/remover item, o carrinho é salvo em localStorage.
   - Ao recarregar a página, o carrinho é restaurado.
   - Carrinho vazio exibe mensagem orientando a voltar ao cardápio.

4. Ao finalizar a compra no carrinho, o usuário deve se cadastrar com:
   nome, whatsapp, email e endereço. Durante o cadastro, o app deve
   solicitar a geolocalização do navegador.

   Critérios de aceite:
   - Campos com validação básica (email válido, whatsapp numérico).
   - Após cadastro válido, o prompt de geolocalização é disparado.
   - Permissão concedida → cadastro salvo e fluxo segue para o req. 5.
   - Permissão negada, falha ou timeout de 10s → cadastro encerrado,
     carrinho preservado, mensagem explicativa com opção de tentar
     novamente.

5. Após o cadastro, o app deve solicitar as credenciais do dispositivo
   via CredentialsContainer (navigator.credentials), como camada extra
   de segurança e prova de vida. Caráter de estudo da API.

   Critérios de aceite:
   - Cadastro concluído → app chama navigator.credentials.get().
   - Autenticação com sucesso → fluxo segue para o req. 6.
   - API indisponível, cancelamento ou falha → motivo registrado no
     console, aviso "credencial não disponível neste dispositivo" e
     fluxo segue para o req. 6 (não trava o checkout).
   - Feature-detect antes da chamada
     (PublicKeyCredential.isUserVerifyingPlatformAuthenticatorAvailable)
     e bloco envolvido em try/catch.

6. Após validar as credenciais, simular um gateway de pagamento genérico.

   Critérios de aceite:
   - Tela de pagamento com resumo do pedido e botão "pagar".
   - Clique em "pagar" exibe estado de processamento simulado
     (ex: spinner de 2s) e então confirmação.
   - Nenhum dado de pagamento real é coletado ou processado.

7. Ao final do fluxo, o app deve gerar um link de WhatsApp para o
   número +5511942668992 com o resumo do pedido.

   Critérios de aceite:
   - Tela de confirmação com botão "Enviar pedido no WhatsApp",
     link https://wa.me/5511942668992?text=... usando encodeURIComponent.
   - Mensagem contém: número do pedido (Date.now()), itens com
     quantidade e preço, total, nome e endereço.
   - Clique abre o WhatsApp com a mensagem pré-preenchida.

## O que o aplicativo não deve fazer

1. Processar o pagamento — apenas simulação.
2. Cadastrar produtos — dados vêm de um arquivo JSON fictício.
3. Controlar delivery.
4. Calcular frete.
