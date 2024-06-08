---
unique-page-id: 2360360
description: Criar um [!DNL Webhook] - Documentação do Marketo - Documentação do produto
title: Criar um [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Criar um [!DNL Webhook] {#create-a-webhook}

Uso [!DNL Webhooks] aproveitar serviços da web de terceiros para enviar mensagens de texto, expandir os dados da pessoa e muito mais.

>[!AVAILABILITY]
>
>Nem todos os usuários do Marketo Engage compraram essa funcionalidade. Entre em contato com a equipe de conta do Adobe (seu gerente de conta) para obter mais detalhes.

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/create-a-webhook-1.png)

1. Clique em **[!UICONTROL Webhooks]**.

   ![](assets/create-a-webhook-2.png)

1. Clique em **[!UICONTROL Novo Webhook]**.

   ![](assets/create-a-webhook-3.png)

1. Nomeie e configure seu [!DNL Webhook].

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Isso geralmente inclui inserir suas credenciais de serviço de terceiros como um parâmetro de URL ou no modelo de POST.

   * **[!UICONTROL URL]**: digite o URL que você usa em sua solicitação para o serviço Web. Para inserir um token, como o endereço de email da pessoa (**`{{lead.Email Address}}`**), em sua solicitação, clique em **[!UICONTROL Inserir token]**.

   * **[!UICONTROL Modelo]**: Se desejar transmitir informações no corpo da solicitação, insira por meio do template de carga útil. Modelos permitidos para os seguintes tipos de solicitação: POST, DELETE, PATCH ou PUT. Você pode usar formatos de dados como JSON ou XML. Para inserir um token no modelo, clique em **[!UICONTROL Inserir token]**.

   * **[!UICONTROL Codificação do token de solicitação]**: se os valores de token incluírem caracteres especiais (como um E comercial (&quot;&amp;&quot;), indique o formato da sua solicitação (**JSON** ou **Formulário/URL**).

   * **[!UICONTROL Tipo de resposta]**: selecione o formato da resposta que você recebe do serviço (**JSON** ou **XML**).

   * **[!UICONTROL Tipo de solicitação]**: selecione o método HTTP a ser usado (DELETE, GET, PATCH, POST, PUT).

1. Clique em **[!UICONTROL Criar]**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Saiba mais na [[!DNL Webhooks]](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"} mergulho profundo.
