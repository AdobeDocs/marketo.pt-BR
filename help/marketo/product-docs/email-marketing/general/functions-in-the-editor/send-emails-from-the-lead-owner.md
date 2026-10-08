---
unique-page-id: 1147340
description: Saiba como enviar emails do endereço do proprietário do lead. Use a opção Enviar do proprietário potencial para que os emails mostrem o remetente correto.
title: Enviar emails do proprietário de leads
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
feature: Email Editor
TQID: 'https://experienceleague.adobe.com/iOBonqrup6ZV9QGhW-i1FpabLVBOKrNxz4xqThcexZ8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: eeae636f-f283-4051-94f0-4d74945464fb
    internal-label: Email Editor
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 6%
---
# Enviar emails do proprietário de leads {#send-emails-from-the-lead-owner}

E se você quiser enviar um email para um cliente potencial em nome do Proprietário do cliente potencial?  Veja como.

1. Encontre seu email, selecione-o e clique em **[!UICONTROL Editar Rascunho]**.

   ![](assets/one.png)

1. Clique no campo **[!UICONTROL De]** (exclua qualquer nome existente) e clique no botão **Inserir token**.

   ![](assets/two.png)

1. Comece a digitar &quot;`{{lead.Lead Owner`&quot; e selecione o token **`{{lead.Lead Owner First Name}}`**.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Insira um valor padrão caso o cliente potencial ainda não tenha um proprietário de cliente potencial e clique em **[!UICONTROL Inserir]**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Clique depois do primeiro token, adicione um espaço e clique no botão **Inserir token**.

   ![](assets/five.png)

1. Comece a digitar &quot;`{{lead.Lead Owner`&quot; e selecione o token **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Insira um valor padrão caso o cliente potencial ainda não tenha um proprietário de cliente potencial e clique em **[!UICONTROL Inserir]**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Verifique se você adicionou um espaço entre os tokens de nome e sobrenome.

1. Clique no campo **[!UICONTROL Do endereço]** (exclua qualquer endereço de email existente) e clique no botão **Inserir token**.

   ![](assets/eight.png)

1. Comece a digitar &quot;`{{lead.Lead Owner`&quot; e selecione o token **`{{lead.Lead Owner Email Address}}`**.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Insira um valor padrão caso o cliente potencial ainda não tenha um proprietário de cliente potencial e clique em **[!UICONTROL Inserir]**.

   ![](assets/ten.png)

1. Verifique se os campos **[!UICONTROL Responder para]** e **[!UICONTROL Assunto]** estão preenchidos, e pronto!

   ![](assets/eleven.png)
