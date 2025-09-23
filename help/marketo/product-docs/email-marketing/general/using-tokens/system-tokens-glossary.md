---
unique-page-id: 1147344
description: Glossário de tokens do sistema - Documentação do Marketo - Documentação do produto
title: Glossário de tokens do sistema
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 2%

---

# Glossário de tokens do sistema {#system-tokens-glossary}

Além dos tokens de pessoa, você pode usar alguns tokens de sistema muito legais. Aqui estão eles.

>[!NOTE]
>
>As configurações de fuso horário da conta afetam quando os tokens de data e hora são executados.

## system.date {#system-date}

O token `{{system.date}}` renderizará a data atual no tempo de execução da seguinte forma: **Ago 08, 2013**

**Funciona em:**

* Etapa de fluxo [Alterar Valor de Dados](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}
* [Etapa de fluxo de Momento Interessante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}
* Etapa de fluxo [Criar Tarefa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}
* O corpo de um email ou modelo

## system.time {#system-time}

O token `{{system.time}}` renderizará a hora atual no tempo de execução da seguinte forma: **04:34 PM (GMT -0700)**

**Funciona em:**

* Etapa de fluxo [Alterar Valor de Dados](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}
* [Etapa de fluxo de Momento Interessante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}
* Etapa de fluxo [Criar Tarefa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}
* O corpo de um email ou modelo

## system.dateTime {#system-datetime}

O token `{{system.dateTime}}` renderizará a data e a hora atuais no tempo de execução da seguinte forma: **2013-08-08 16:36:13**

**Funciona em:**

* Etapa de fluxo [Alterar Valor de Dados](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}
* [Etapa de fluxo de Momento Interessante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}
* Etapa de fluxo [Criar Tarefa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}
* O corpo de um email ou modelo

## system.forwardToFriendLink {#system-forwardtofriendlink}

O token `{{system.forwardToFriendLink}}` permite controlar o posicionamento do [&#39;Encaminhar para um Link de Amigo&#39; nos Emails](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target="_blank"}.

**Funciona em:**

* [Adicionar um token do sistema como um link em um email](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} ou modelo

## system.unsubscribeLink {#system-unsubscribelink}

O token `{{system.unsubscribeLink}}` permite controlar o posicionamento do link de cancelamento de inscrição em um email.

**Funciona em:**

* [Adicionar um token do sistema como um link em um email](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} ou modelo

## system.viewAsWebpageLink {#system-viewaswebpagelink}

O token `{{system.viewAsWebpageLink}}` permite controlar o posicionamento do link Exibir como Página da Web em um email.

**Funciona com:**

* [Adicionar um token do sistema como um link em um email](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} ou modelo
