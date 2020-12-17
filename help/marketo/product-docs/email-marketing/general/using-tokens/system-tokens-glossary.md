---
unique-page-id: 1147344
description: Glossário de tokens do sistema - Documentos do comerciante - Documentação do produto
title: Glossário de tokens do sistema
translation-type: tm+mt
source-git-commit: 1c4c4c62215550a09125f76fb76017348aba2bdf
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Glossário de tokens do sistema {#system-tokens-glossary}

Além de tokens pessoais, você pode usar alguns tokens de sistema muito legais. Aqui estão eles.

>[!NOTE]
>
>As configurações de fuso horário da sua conta afetam quando tokens de data e hora são executados.

## system.date {#system-date}

O token `{{system.date}}` renderizará a data atual no tempo de execução da seguinte maneira: **08 de agosto de 2013**

**Funciona em:**

* [Etapa de ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) fluxo de valor dos dados de alteração
* [Interessante etapa ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) do Momentflow
* [Etapa Criar ](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) fluxo de tarefas
* O corpo de um email ou modelo

## system.time {#system-time}

O token `{{system.time}}` renderizará a hora atual no tempo de execução da seguinte maneira: **04:34 PM (GMT -0700)**

**Funciona em:**

* [Etapa de ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) fluxo de valor dos dados de alteração
* [Interessante etapa ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) do Momentflow
* [Etapa Criar ](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) fluxo de tarefas
* O corpo de um email ou modelo

## system.dateTime {#system-datetime}

O token `{{system.dateTime}}` renderizará a data e a hora atuais no tempo de execução da seguinte maneira: **2013-08-08 16:36:13**

**Funciona em:**

* [Etapa de ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) fluxo de valor dos dados de alteração
* [Interessante etapa ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) do Momentflow
* [Etapa Criar ](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) fluxo de tarefas
* O corpo de um email ou modelo

## system.forwardToFriendLink {#system-forwardtofriendlink}

O token `{{system.forwardToFriendLink}}` permite controlar a colocação do [&#39;Encaminhar para um link de amigo&#39; em Emails](../../../../product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md).

**Funciona em:**

* [Adicionar um token do sistema como um link em um modelo de ](add-a-system-token-as-a-link-in-an-email.md) email

## system.unsubscribeLink {#system-unsubscribelink}

O token `{{system.unsubscribLink}}` permite controlar a colocação do link para cancelar a inscrição em um email.

**Funciona em:**

* [Adicionar um token do sistema como um link em um modelo de ](add-a-system-token-as-a-link-in-an-email.md) email

## system.viewAsWebpageLink {#system-viewaswebpagelink}

O token `{{system.viewAsWebpageLink}}` permite controlar a colocação da Visualização como link de Página da Web em um email.

**Funciona com:**

* [Adicionar um token do sistema como um link em um modelo de ](add-a-system-token-as-a-link-in-an-email.md) email
