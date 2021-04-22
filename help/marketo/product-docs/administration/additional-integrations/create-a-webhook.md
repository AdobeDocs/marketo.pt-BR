---
unique-page-id: 2360360
description: Criar um Webhook - Documentos do Marketo - Documentação do produto
title: Criar um Webhook
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 3%

---

# Criar um Webhook {#create-a-webhook}

Use webhooks para aproveitar os serviços da Web de terceiros para enviar mensagens de texto, expandir dados de pessoas e muito mais.

>[!AVAILABILITY]
>
>Nem todos os clientes compraram essa funcionalidade. Confira os detalhes com seu representante de vendas.

1. Vá para **Admin** e clique em **Webhooks**.

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. Clique em **Novo Webhook**.

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Nomeie e configure seu webhook.

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >Isso geralmente inclui inserir suas credenciais de serviço de terceiros como parâmetro de URL ou no modelo do POST.

   * **URL**: Insira o URL usado para POST sua solicitação para o serviço da Web. Para inserir um token, como o endereço de email da pessoa (**`{{lead.Email Address}}`**), em sua solicitação, clique em **Inserir token**.

   * **Modelo**: Se desejar transmitir informações no corpo do POST, insira o template. Use qualquer formato de dados compatível com HTTP POST, incluindo XML, JSON ou SOAP. Para inserir um token no modelo, clique em **Inserir token**.

   * **Codificação** do token de solicitação: Se os valores de token incluírem caracteres especiais (como um E comercial (&amp;)), indique o formato da solicitação (**** JSONou  **Form/Url**).

   * **Tipo** de resposta: Selecione o formato da resposta recebida do serviço (**** JSONou  **XML**).

   Clique em Criar.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>Saiba mais no aprofundamento de [webhooks](https://developers.marketo.com/documentation/webhooks/).
