---
unique-page-id: 7514918
description: Noções básicas sobre o cancelamento de inscrição - Documentação do Marketo - Documentação do produto
title: Noções básicas sobre o cancelamento de inscrição
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
feature: Deliverability
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 2%

---

# Noções básicas sobre o cancelamento de inscrição {#understanding-unsubscribe}

Na verdade, há vários tipos diferentes de cancelamentos de assinatura integrados no Marketo. Todos são representados por campos no objeto pessoa, como Nome.

Todos esses campos são incorporados à sua assinatura do Marketo. Todos são do tipo booleano (caixa de seleção). Eles podem ser usados no Forms ou [Alterar valor dos dados](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) etapas de fluxo.

## Inscrição cancelada {#unsubscribed}

Isso é usado na página de cancelamento de inscrição padrão. Se uma pessoa marcar essa caixa ou clicar no link de cancelamento de inscrição em um email, ela não receberá mais emails de marketing. No entanto, receberão [emails operacionais](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marketing suspenso {#marketing-suspended}

Este campo é definido pelo usuário para colocar pessoas em um cancelamento de inscrição temporário. As pessoas só poderão atingir esse status se forem alteradas manualmente ou se uma etapa do fluxo de alteração de valor de dados for utilizada.

## E-mail suspenso {#email-suspended}

Este status bloqueia a correspondência de uma pessoa por 24 horas após uma rejeição permanente ocorrer. Após 24 horas, a pessoa voltará a ser mensurável.

>[!NOTE]
>
>Email suspenso permanecerá marcado mesmo depois que o período de 24 horas terminar, para que você possa se referir a pessoas que foram historicamente marcadas como tal. Para ver se a pessoa pode enviar emails, basta calcular 24 horas após o momento da suspensão do email.

## Incluído na lista de bloqueios {#blocklisted}

[Use isso para pessoas como concorrentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). Qualquer pessoa que você quiser receber **não** e-mails — operacionais, de marketing etc. Eles não ganham nada!

![](assets/image2015-5-18-12-3a6-3a40.png)
