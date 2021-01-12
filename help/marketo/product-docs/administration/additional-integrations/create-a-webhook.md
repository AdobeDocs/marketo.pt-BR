---
unique-page-id: 2360360
description: Criar um Webhook - Documentos do Marketing - Documentação do produto
title: Criar um Webhook
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---


# Criar um Webhook {#create-a-webhook}

Use webhooks para aproveitar os serviços da Web de terceiros para enviar mensagens de texto, expandir dados de pessoas e muito mais.

>[!AVAILABILITY]
>
>Nem todos os clientes adquiriram essa funcionalidade. Entre em contato com seu representante de vendas para obter detalhes.

1. Vá para **Admin** e clique em **Webhooks**.

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. Clique em **Novo Webhook**.

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Dê um nome e configure seu webhook.

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >Isso costuma incluir a inserção de credenciais de serviço de terceiros como parâmetro de URL ou no modelo de POST.

   * **URL**: Insira o URL que você usa para POST sua solicitação ao serviço da Web. Para inserir um token, como o endereço de email da pessoa (**`{{lead.Email Address}}`**), na solicitação, clique em **Inserir token**.

   * **Modelo**: Se desejar transmitir informações no corpo do POST, insira o modelo. Use qualquer formato de dados compatível com POST HTTP, incluindo XML, JSON ou SOAP. Para inserir um token no modelo, clique em **Inserir token**.

   * **Codificação** do token de solicitação: Se os valores de token incluírem caracteres especiais (como um E comercial, &#39;&amp;&#39;), indique o formato da solicitação (**** JSON ou  **Form/Url**).

   * **Tipo** de resposta: Selecione o formato da resposta recebida do serviço (**** JSON **ou** XML).

   Clique em Criar.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>Saiba mais no mergulho profundo [webhooks](http://developers.marketo.com/documentation/webhooks/).
