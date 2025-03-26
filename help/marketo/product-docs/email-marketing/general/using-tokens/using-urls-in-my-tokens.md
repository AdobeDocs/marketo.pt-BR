---
unique-page-id: 11382535
description: Uso de URLs em Meus tokens - Documentação do Marketo - Documentação do produto
title: Utilização de URLs em Meus tokens
exl-id: 6830c621-4d94-4f31-a608-2f7b2aced88c
feature: Tokens
source-git-commit: 165dca2573f340ede147866c3a30707bbfb6857c
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Utilização de URLs em Meus tokens {#using-urls-in-my-tokens}

Siga as etapas abaixo para usar Meus tokens para inserir URLs em seus emails.

1. Selecione seu programa e clique em **Meus tokens**.

   ![](assets/one-4.png)

1. Selecione o **Texto** Meu token, arraste e solte-o na tela.

   ![](assets/two-4.png)

1. Dê um nome exclusivo ao token, insira uma URL (sem o https://) e clique em **Salvar**.

   ![](assets/three-4.png)

   >[!CAUTION]
   >
   >**Usando http/https...**
   >
   >* Para garantir que os cliques sejam rastreados em seu email, **não** digite o valor do token https:// _inside_. Use-o fora do token, como mostrado na Etapa 7.
   >
   >* É altamente recomendável não deixar de fora o http/https. Isso pode fazer com que a [versão da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} do seu email seja renderizada incorretamente.

1. Selecione o email no seu programa.

   ![](assets/four-3.png)

1. Clique em **Editar rascunho**.

   ![](assets/five-3.png)

1. Clique duas vezes na área de texto para editá-la.

   ![](assets/six-1.png)

1. Em qualquer lugar do email, digite `https://` (sem deixar um espaço depois de) e clique no ícone Inserir Token.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >É claro que você também tem a opção de inserir `http://` se o seu site não usar https.

1. Localize o Meu Token, selecione-o e clique em **Inserir**.

   ![](assets/eight.png)

1. Realce o https:// e o token, depois pressione Ctrl/Cmd+X (Ctrl = Windows/Cmd = Mac) para cortar o texto.

   ![](assets/nine.png)

1. Realce o texto que deseja que o link exiba e clique no ícone Insert/Edit Link.

   ![](assets/ten.png)

1. Pressione Ctrl/Cmd+V para colar o conteúdo na caixa **URL** e clique em **Inserir**.

   ![](assets/eleven.png)

1. Clique em **Salvar**.

   ![](assets/twelve.png)

   E pronto! Seu URL será preenchido após o envio e, graças à colocação de https:// na frente do token, produzirá um link rastreável.
