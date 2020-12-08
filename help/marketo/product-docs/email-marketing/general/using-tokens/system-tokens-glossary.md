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

O `{{system.date}}` token renderizará a data atual no tempo de execução da seguinte maneira: **08 de ago de 2013**

**Funciona em:**

* [Etapa de fluxo do Valor](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) de Dados de Alteração
* [Etapa de fluxo de momento](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) interessante
* [Criar etapa de fluxo de Tarefa](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)
* O corpo de um email ou modelo

## system.time {#system-time}

O `{{system.time}}` token renderizará a hora atual no tempo de execução da seguinte maneira: **16:34 (GMT -0700)**

**Funciona em:**

* [Etapa de fluxo do Valor](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) de Dados de Alteração
* [Etapa de fluxo de momento](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) interessante
* [Criar etapa de fluxo de Tarefa](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)
* O corpo de um email ou modelo

## system.dateTime {#system-datetime}

O `{{system.dateTime}}` token renderizará a data e a hora atuais no tempo de execução da seguinte maneira: **2013-08-08 16:36:13**

**Funciona em:**

* [Etapa de fluxo do Valor](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) de Dados de Alteração
* [Etapa de fluxo de momento](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) interessante
* [Criar etapa de fluxo de Tarefa](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)
* O corpo de um email ou modelo

## system.forwardToFriendLink {#system-forwardtofriendlink}

O `{{system.forwardToFriendLink}}` token permite controlar a colocação do [&#39;Encaminhar para um link de amigo&#39; em emails](../../../../product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md).

**Funciona em:**

* [Adicionar um token do sistema como um link em um email](add-a-system-token-as-a-link-in-an-email.md) ou modelo

## system.unsubscribeLink {#system-unsubscribelink}

O `{{system.unsubscribLink}}` token permite controlar a colocação do link para cancelar a inscrição em um email.

**Funciona em:**

* [Adicionar um token do sistema como um link em um email](add-a-system-token-as-a-link-in-an-email.md) ou modelo

## system.viewAsWebpageLink {#system-viewaswebpagelink}

O `{{system.viewAsWebpageLink}}` token permite controlar a colocação da Visualização como link de Página da Web em um email.

**Funciona com:**

* [Adicionar um token do sistema como um link em um email](add-a-system-token-as-a-link-in-an-email.md) ou modelo
