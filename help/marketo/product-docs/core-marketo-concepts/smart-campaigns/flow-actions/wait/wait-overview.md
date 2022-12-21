---
unique-page-id: 1146950
description: Wait - Marketo Docs - Documentação do produto
title: Aguardar
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 2%

---

# Aguardar {#wait}

## Visão geral {#overview}

Pausar uma pessoa em um fluxo de campanha inteligente com o **etapa de espera**.

![](assets/wait-overview.png)

Observe como você pode digitar em linguagem natural como &quot;4 horas&quot;. Do **not**, no entanto, abreviar as palavras (ou seja, 4 horas). A campanha inteligente ainda seria executada, mas a etapa de espera seria ignorada.

>[!CAUTION]
>
>Alterar a duração de uma etapa de espera não afetará as pessoas que já a inseriram. Por exemplo: você tem uma etapa de espera por 5 dias, uma pessoa entra nela e depois altera a etapa de espera para 7 dias - essa pessoa ainda aguardará os 5 dias originais antes de avançar para a próxima etapa do fluxo.

>[!TIP]
>
>Se alguém já estiver em uma etapa de espera e você não quiser que avance depois que o período de espera terminar, insira [remover do fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) logo após a etapa de espera. Especifique quem deseja remover usando o [adicionar escolha](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md) opção.

## Uso {#usage}

Há três maneiras principais de usar uma etapa de fluxo de espera:

1. [Usar uma duração em uma etapa do fluxo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [Usar uma Data Específica em uma Etapa de Fluxo de Espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [Usar um token de data em uma etapa de fluxo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
