---
unique-page-id: 2360360
description: Crie um webhook no Administrador para chamar serviços da Web de terceiros para SMS, dados de pessoa e muito mais.
title: Criar um  [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
TQID: https://experienceleague.adobe.com/O4xw1wSvFeTJ2xqZn4Eo7JbrUBQQmKcl7mvLkduFXGc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: fc9b09fe-b844-4544-887b-e420c3b82065
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 220
ht-degree: 0%

---

# Criar um [!DNL Webhook] {#create-a-webhook}

Use o [!DNL Webhooks] para aproveitar os serviços Web de terceiros para enviar mensagens de texto, expandir os dados da pessoa e muito mais.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/create-a-webhook-1.png)

1. Clique em **[!UICONTROL Webhooks]**.

   ![](assets/create-a-webhook-2.png)

1. Clique em **[!UICONTROL Novo Webhook]**.

   ![](assets/create-a-webhook-3.png)

1. Nomeie e configure seu [!DNL Webhook].

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Isso geralmente inclui inserir suas credenciais de serviço de terceiros como um parâmetro de URL ou no modelo POST.

   * **[!UICONTROL URL]**: insira a URL usada em sua solicitação para o serviço Web. Para inserir um token, como o endereço de email da pessoa (**`{{lead.Email Address}}`**), em sua solicitação, clique em **[!UICONTROL Inserir token]**.

   * **[!UICONTROL Modelo]**: se quiser transmitir informações no corpo da solicitação, insira-as por meio do modelo de carga. Modelos permitidos para os seguintes tipos de solicitação: POST, DELETE, PATCH ou PUT. Você pode usar formatos de dados como JSON ou XML. Para inserir um token no modelo, clique em **[!UICONTROL Inserir Token]**.

   * **[!UICONTROL Solicitar Codificação de Token]**: se os valores de token incluírem caracteres especiais (como um E comercial, &quot;&amp;&quot;), indique o formato da sua solicitação (**JSON** ou **Form/Url**).

   * **[!UICONTROL Tipo de resposta]**: selecione o formato da resposta recebida do serviço (**JSON** ou **XML**).

   * **[!UICONTROL Tipo de Solicitação]**: Selecione o método HTTP a ser usado (DELETE, GET, PATCH, POST, PUT).

1. Clique em **[!UICONTROL Criar]**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Saiba mais no aprofundamento de [[!DNL Webhooks]](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"}.
