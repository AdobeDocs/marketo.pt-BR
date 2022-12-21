---
unique-page-id: 1900573
description: Adicionar um token do sistema como um link em um email - Documentos do Marketo - Documentação do produto
title: Adicionar um token de sistema como um link em um email
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
source-git-commit: 65caed388ac33fc9f3142102343fe43ebc186e6e
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Adicionar um token de sistema como um link em um email {#add-a-system-token-as-a-link-in-an-email}

Você pode usar esses tokens do sistema para personalizar a posição de links especiais em seus emails.

Os seguintes tokens podem ser usados como links em um email ou modelo de email:

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>Esses tokens **not** ser clicável, a menos que dentro de um link de âncora. Além disso, eles podem **not** ser incorporado em um Meu token.

Veja como adicioná-los a um email:

1. Encontre e selecione seu email e clique em **Editar rascunho**.

   ![](assets/one-1.png)

1. Clique duas vezes em uma área editável.

   ![](assets/two-1.png)

1. Realce o texto que deseja converter em um link que terá o token e clique no botão **Inserir/Editar link** botão.

   ![](assets/three-1.png)

1. Insira o token no URL do link e clique em **Inserir**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >Copie/cole o token desejado: **`{{system.forwardToFriendLink}}`** ou **`{{system.unsubscribeLink}}`** ou **`{{system.viewAsWebpageLink}}`**

1. Clique em **Salvar**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>Se estiver usando essa abordagem para adicionar o token de sistema &quot;viewAsWebpageLink&quot;, você poderá **not** substituí-lo usando tokens. Em vez disso, use [Adicionar uma Exibição como Link da Página da Web a um Email](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) abordagem que permite substituir &quot;viewAsWebPageLink&quot; usando tokens.

>[!NOTE]
>
>Não se esqueça de [aprove seu email](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md) quando concluído.

Muito bem! Agora você sabe como adicionar um token de sistema como um link em um email.
