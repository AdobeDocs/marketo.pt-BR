---
unique-page-id: 2360360
description: Criar um Webhook - Documentos do Marketo - Documentação do produto
title: Criar um Webhook
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: 25a574719eb6c064d33b6a1cebafe2668ed1330d
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 2%

---

# Criar um Webhook {#create-a-webhook}

Use webhooks para aproveitar os serviços da Web de terceiros para enviar mensagens de texto, expandir dados de pessoas e muito mais.

>[!AVAILABILITY]
>
>Nem todos os clientes compraram essa funcionalidade. Confira os detalhes com seu representante de vendas.

1. Ir para **Administrador** e clique em **Webhooks**.

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. Clique em **Novo Webhook**.

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Nomeie e configure seu webhook.

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >Isso geralmente inclui inserir suas credenciais de serviço de terceiros como parâmetro de URL ou no modelo do POST.

   * **URL**: Insira o URL usado em sua solicitação para o serviço da Web. Para inserir um token, como o endereço de email da pessoa (**`{{lead.Email Address}}`**), na sua solicitação, clique em **Inserir Token**.

   * **Modelo**: Se desejar transmitir informações no corpo do POST, insira o template. Use qualquer formato de dados compatível com HTTP POST, incluindo XML, JSON ou SOAP. Para inserir um token no modelo, clique em **Inserir Token**.

   * **Codificação do token de solicitação**: Se os valores de token incluírem caracteres especiais (como um E comercial (&amp;)), indique o formato da solicitação (**JSON** ou **Formulário/Url**).

   * **Tipo de resposta**: Selecione o formato da resposta recebida do serviço (**JSON** ou **XML**).

   * **Tipo de solicitação**: Selecione o método HTTP a ser usado (DELETE, GET, PATCH, POST, PUT).

   Clique em **Criar**.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>Saiba mais na [webhooks](https://developers.marketo.com/documentation/webhooks/) mergulho profundo.
