---
unique-page-id: 1147091
description: Noções básicas sobre a associação ao programa - Documentação da Marketo - Documentação do produto
title: Compreensão da assinatura do programa
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 1%

---

# Noções básicas sobre a associação ao programa {#understanding-program-membership}

>[!NOTE]
>
>A Marketo agora está padronizando a linguagem em todas as subscrições, para que você possa ver lead/lead na sua assinatura e pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa; não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md).

>[!NOTE]
>
>**Definição:** Um membro é uma pessoa que tem um status em um programa.

## Como as pessoas se tornam membros de um programa {#how-people-become-members-of-a-program}

1. Uma pessoa preenche um formulário [em uma landing page](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) no programa.

   1. A pessoa terá automaticamente o primeiro status na progressão.

1. Você [importa membros para o programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md) de um arquivo CSV.

   1. A pessoa terá automaticamente o primeiro status na progressão.

1. Use a etapa de fluxo [alterar status do programa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md).
1. Uma pessoa registra ou participa de um [webinário sincronizado com um programa de eventos](/help/marketo/product-docs/demand-generation/events/understanding-events/launchpoint-event-partners.md).
1. Uma pessoa é [criada usando o aplicativo de check-in do Marketo iPad](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md).
1. Uma pessoa é adicionada a uma Campanha SFDC, que é [sincronizada ao programa](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md).

>[!NOTE]
>
>Para um programa de email, uma pessoa é adicionada à associação somente quando o email é enviado.

## Status do Programa {#program-statuses}

Os status do programa são as etapas que as pessoas passam em um programa (por exemplo, Convidado, RSVP&#39;d, Participado, Sem programa). Essas etapas são definidas pelo [canal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>Uma pessoa não pode retroceder para um status de programa anterior. A progressão do status é uma única maneira.

## Status de sucesso {#success-statuses}

A finalidade de um programa é criar uma interação significativa com a pessoa ou prospecto. O sucesso é marcado quando uma pessoa atinge o status que atinge esse objetivo.

>[!NOTE]
>
>Para um webinário, registrar não é uma interação significativa se eles não assistirem ao webinário. Nesse caso, a participação é bem-sucedida.

## Programa de aquisição  {#acquisition-program}

Quando um novo nome entra no sistema como um membro do programa, o Marketo define automaticamente esse programa como &quot;aquisição&quot;. Isso estabelece crédito para [Atribuição de primeiro toque](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

>[!MORELIKETHIS]
>
>* [Usar tags em um programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags/use-tags-in-a-program.md)
>* [Criar um relatório de desempenho de programa](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md)

