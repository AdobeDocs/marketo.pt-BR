---
unique-page-id: 1900589
description: Saiba como adicionar links rastreados a emails somente texto. Ative o rastreamento de links para poder medir cliques em seus relatórios de email.
title: Adicionar links rastreados a um email de texto
exl-id: 10b4e029-de23-4054-83f7-b68fea68c838
feature: Email Editor
TQID: https://experienceleague.adobe.com/zz5DkOWG-x3y-oq-E77xRAZtcNdmimbwKsctKSChnXM
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 176
ht-degree: 7%

---

# Adicionar links rastreados a um email de texto {#add-tracked-links-to-a-text-email}

>[!PREREQUISITES]
>
>* [Criar um Email Somente Texto](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-a-text-only-email.md)
>* [Editar elementos em um email](/help/marketo/product-docs/email-marketing/general/email-editor-2/edit-elements-in-an-email.md)

Os links de texto de email podem ser rastreados no Marketo. Vamos ver como funciona.

1. Selecione seu email e clique em **Editar Rascunho**.

1. Selecione seu email e clique em **[!UICONTROL Editar Rascunho]**.

   ![](assets/one-9.png)

1. Clique duas vezes na área editável à qual deseja adicionar o link.

   ![](assets/two-8.png)

1. Insira a URL com colchetes duplos, desta forma: `[[www.domain.com/path/page.html]]`.

   ![](assets/three-8.png)

   >[!CAUTION]
   >
   >Se um email tiver sido enviado há mais de 365 dias **e** ninguém tiver clicado em nenhum de seus links nos últimos 180 dias, o Marketo Engage removerá a rota para a URL do nosso banco de dados, o que causará a quebra do link. Se precisar que o link seja permanente, não use o rastreamento.

1. Feche o editor e não se esqueça de aprovar o rascunho.

   ![](assets/four-6.png)

>[!NOTE]
>
>A funcionalidade da classe mktNoTok não funciona com links rastreáveis em emails de texto. Somente para emails do HTML.
