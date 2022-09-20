---
unique-page-id: 1147344
description: Glossário de tokens do sistema - Documentos do Marketo - Documentação do produto
title: Glossário de tokens do sistema
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
source-git-commit: 93032a016a67fe0edf7a8093633d6b06ec25c18d
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Glossário de tokens do sistema {#system-tokens-glossary}

Além dos tokens de pessoa, você pode usar alguns tokens de sistema muito legais. Aqui estão eles.

>[!NOTE]
>
>As configurações de fuso horário da conta afetam quando tokens de data e hora são executados.

## system.date {#system-date}

O `{{system.date}}` o token renderizará a data atual no tempo de execução da seguinte maneira: **08 de agosto de 2013**

**Funciona em:**

* [Alterar valor de dados](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target=&quot;_blank&quot;} etapa de fluxo
* [Momento interessante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target=&quot;_blank&quot;} etapa de fluxo
* [Criar tarefa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target=&quot;_blank&quot;} etapa de fluxo
* O corpo de um email ou modelo

## system.time {#system-time}

O `{{system.time}}` o token renderizará o tempo atual no tempo de execução da seguinte maneira: **16:34 (GMT -0700)**

**Funciona em:**

* [Alterar valor de dados](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target=&quot;_blank&quot;} etapa de fluxo
* [Momento interessante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target=&quot;_blank&quot;} etapa de fluxo
* [Criar tarefa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target=&quot;_blank&quot;} etapa de fluxo
* O corpo de um email ou modelo

## system.dateTime {#system-datetime}

O `{{system.dateTime}}` o token renderizará a data e a hora atuais no tempo de execução da seguinte maneira: **2013-08-08 16:36:13º**

**Funciona em:**

* [Alterar valor de dados](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target=&quot;_blank&quot;} etapa de fluxo
* [Momento interessante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target=&quot;_blank&quot;} etapa de fluxo
* [Criar tarefa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target=&quot;_blank&quot;} etapa de fluxo
* O corpo de um email ou modelo

## system.forwardToFriendLink {#system-forwardtofriendlink}

O `{{system.forwardToFriendLink}}` permite controlar a posição do [&#39;Encaminhar para um Link Amigo&#39; em Emails](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target=&quot;_blank&quot;}.

**Funciona em:**

* [Adicionar um token de sistema como um link em um email](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target=&quot;_blank&quot;} ou modelo

## system.unsubscribeLink {#system-unsubscribelink}

O `{{system.unsubscribeLink}}` permite controlar a disposição do link de cancelamento de inscrição em um email.

**Funciona em:**

* [Adicionar um token de sistema como um link em um email](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target=&quot;_blank&quot;} ou modelo

## system.viewAsWebpageLink {#system-viewaswebpagelink}

O `{{system.viewAsWebpageLink}}` permite controlar o posicionamento do link Exibir como página da Web em um email.

**Funciona com:**

* [Adicionar um token de sistema como um link em um email](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target=&quot;_blank&quot;} ou modelo
