---
unique-page-id: 1900573
description: Adicionar um token do sistema como um link em um email - Documentação do Marketo - Documentação do produto
title: Adicionar um token do sistema como um link em um email
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Adicionar um token do sistema como um link em um email {#add-a-system-token-as-a-link-in-an-email}

Você pode usar esses tokens do sistema para personalizar a posição dos links especiais em seus emails.

Os seguintes tokens podem ser usados como links em um email ou template de email:

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>Esses tokens serão **não** ser clicável, a menos que esteja dentro de um link de âncora. Além disso, elas podem **não** ser incorporado em um Meu token.

Veja como adicioná-los a um email:

1. Localize e selecione seu email e clique em **Editar rascunho**.

   ![](assets/one-1.png)

1. Clique duas vezes em uma área editável.

   ![](assets/two-1.png)

1. Realce o texto que deseja converter em um link que terá o token e clique no link **Inserir/Editar link** botão.

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
>Se estiver usando essa abordagem para adicionar o token do sistema &quot;viewAsWebpageLink&quot;, você poderá **não** substituí-lo usando tokens. Em vez disso, use [Adicionar um link Exibir como página da Web a um email](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) que permite substituir &quot;viewAsWebPageLink&quot; usando tokens.

>[!NOTE]
>
>Não se esqueça de [aprovar seu email](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md) quando terminar.

Muito bem! Agora você sabe como adicionar um token do sistema como um link em um email.
