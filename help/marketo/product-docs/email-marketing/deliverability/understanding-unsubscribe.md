---
unique-page-id: 7514918
description: Noções Gerais da Cancelamento de Assinatura - Documentos do Marketing - Documentação do Produto
title: Noções Gerais de Cancelamento de Assinatura
translation-type: tm+mt
source-git-commit: 615ddd6ffdb3873baa159d440db7b24f3a07e6b0
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Noções Básicas de Cancelamento de Assinatura {#understanding-unsubscribe}

Há, na verdade, vários tipos diferentes de cancelamentos incorporados no Marketo. Todos eles são representados por campos no objeto da pessoa, assim como o Nome.

>[!NOTE]
>
>O Marketo está mudando termos como Blacklist e Whitelist para Lista de bloqueios e Lista de permissões em nosso produto. Durante esta atualização, você pode ver os termos antigos em nossa interface do usuário e nas capturas de tela da documentação, bem como os novos termos em nosso texto de documentação. Pedimos desculpas por qualquer confusão.

Todos esses campos estão incorporados à sua subscrição de marketing. Todos eles são do tipo booleano (caixa de seleção). Eles podem ser usados nas etapas de fluxo do Forms ou [Alterar valor de dados](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

## Assinatura cancelada {#unsubscribed}

Isso é usado na página de cancelamento de inscrição padrão. Se uma pessoa marcar essa caixa ou clicar no link para cancelar a inscrição em um email, ela não receberá mais emails de marketing. No entanto, eles receberão [emails operacionais](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marketing Suspenso {#marketing-suspended}

Este campo é definido pelo usuário para colocar pessoas em uma anulação temporária de assinatura. As pessoas só poderão atingir esse status se forem manualmente alteradas ou se uma etapa de fluxo de valores de dados de alteração for utilizada.

## Email suspenso {#email-suspended}

Esse status impede que uma pessoa envie mensagens por correio por 24 horas após ocorrer uma rejeição. Depois de 24 horas, a pessoa se tornará endereçável novamente.

>[!NOTE]
>
>Email suspenso permanecerá marcado mesmo depois que o período de 24 horas terminar, portanto, você pode consultar pessoas que historicamente foram marcadas como tal. Para ver se a pessoa é endereçável, basta calcular 24 horas após o momento da suspensão do e-mail.

## incluir na lista de bloqueios {#blocklisted}

[Use isso para pessoas como concorrentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). Qualquer pessoa que você quiser receber **no** e-mails — operacionais, de marketing etc. Eles não recebem nada!

![](assets/image2015-5-18-12-3a6-3a40.png)
