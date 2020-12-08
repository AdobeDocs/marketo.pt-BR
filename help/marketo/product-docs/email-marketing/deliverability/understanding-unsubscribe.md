---
unique-page-id: 7514918
description: Noções Gerais da Cancelamento de Assinatura - Documentos do Marketing - Documentação do Produto
title: Noções Gerais de Cancelamento de Assinatura
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Noções Gerais de Cancelamento de Assinatura {#understanding-unsubscribe}

Há, na verdade, vários tipos diferentes de cancelamentos incorporados no Marketo. Todos eles são representados por campos no objeto da pessoa, assim como o Nome.

>[!NOTE]
>
>O Marketo está mudando termos como Blacklist e Whitelist para Lista de bloqueios e Lista de permissões em nosso produto. Durante esta atualização, você pode ver os termos antigos em nossa interface do usuário e nas capturas de tela da documentação, bem como os novos termos em nosso texto de documentação. Pedimos desculpas por qualquer confusão.

Todos esses campos estão incorporados à sua subscrição de marketing. Todos eles são do tipo booleano (caixa de seleção). Eles podem ser usados nas etapas de fluxo do Forms ou [Alterar valor](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) de dados.

## Inscrito {#unsubscribed}

Isso é usado na página de cancelamento de inscrição padrão. Se uma pessoa marcar essa caixa ou clicar no link para cancelar a inscrição em um email, ela não receberá mais emails de marketing. No entanto, receberão e-mails [](../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)operacionais.

## Suspenso de marketing {#marketing-suspended}

Este campo é definido pelo usuário para colocar pessoas em uma anulação temporária de assinatura. As pessoas só poderão atingir esse status se forem manualmente alteradas ou se uma etapa de fluxo de valores de dados de alteração for utilizada.

## Email suspenso {#email-suspended}

Esse status impede que uma pessoa envie mensagens por correio por 24 horas após ocorrer uma rejeição. Depois de 24 horas, a pessoa se tornará endereçável novamente.

>[!NOTE]
>
>Email suspenso permanecerá marcado mesmo depois que o período de 24 horas terminar, portanto, você pode consultar pessoas que historicamente foram marcadas como tal. Para ver se a pessoa é endereçável, basta calcular 24 horas após o momento da suspensão do e-mail.

## incluir na lista de bloqueios {#blocklisted}

[Use isso para pessoas como concorrentes](http://docs.marketo.com/x/uwOQ). Qualquer pessoa que você quiser que **não receba** e-mails — operacionais, de marketing etc. Eles não recebem nada!

![](assets/image2015-5-18-12-3a6-3a40.png)

