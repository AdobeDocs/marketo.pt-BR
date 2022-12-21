---
unique-page-id: 7514918
description: Noções básicas sobre cancelamento de inscrição - Documentos do Marketo - Documentação do produto
title: Noções básicas sobre cancelamento de inscrição
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 2%

---

# Noções básicas sobre cancelamento de inscrição {#understanding-unsubscribe}

Na verdade, há vários tipos diferentes de cancelamentos de assinatura integrados no Marketo. Todos são representados por campos no objeto da pessoa, como Nome.

>[!NOTE]
>
>A Marketo está mudando termos como Blacklist e Whitelist para Lista de bloqueios e Lista de permissões em nosso produto. Durante essa atualização, você pode ver os termos antigos em nossa interface do usuário e capturas de tela da documentação, bem como os novos termos em nosso texto de documentação. Pedimos desculpas por qualquer confusão.

Todos esses campos são incorporados à sua assinatura do Marketo. Todos são do tipo booleano (caixa de seleção). Eles podem ser usados no Forms ou [Alterar valor de dados](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) etapas de fluxo.

## Inscrição cancelada {#unsubscribed}

Isso é usado na página de cancelamento de assinatura padrão. Se uma pessoa marcar essa caixa ou clicar no link de cancelamento de inscrição em um email, ela não receberá mais emails de marketing. No entanto, receberão [emails operacionais](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marketing suspenso {#marketing-suspended}

Esse campo é definido pelo usuário para colocar pessoas em um cancelamento temporário de assinatura. As pessoas só podem atingir esse status se forem manualmente alteradas ou se uma etapa do fluxo do valor de dados de alteração for usada.

## E-mail suspenso {#email-suspended}

Esse status impede que uma pessoa envie mensagens por 24 horas depois que ocorre uma devolução permanente. Depois de 24 horas, a pessoa se tornará endereçável novamente.

>[!NOTE]
>
>Email Suspenso permanecerá marcado mesmo após o término do período de 24 horas, para que você possa se referir a pessoas que historicamente foram marcadas como tal. Para ver se a pessoa é endereçável, basta calcular 24 horas após o momento da suspensão do email.

## Incluído na lista de bloqueios {#blocklisted}

[Use isso para pessoas como concorrentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). Qualquer pessoa que você deseja receber **não** emails — operacionais, de marketing etc. Eles não têm nada!

![](assets/image2015-5-18-12-3a6-3a40.png)
