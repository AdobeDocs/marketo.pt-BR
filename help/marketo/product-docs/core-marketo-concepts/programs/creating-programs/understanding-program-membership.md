---
unique-page-id: 1147091
description: Noções básicas sobre a associação ao programa - Documentação do Marketo - Documentação do produto
title: Noções básicas sobre assinaturas de programas
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
feature: Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 3%

---

# Noções básicas sobre assinaturas de programas {#understanding-program-membership}

>[!NOTE]
>
>**Definição:** um membro é uma pessoa que tem um status em um programa.

## Como as pessoas se tornam membros de um programa {#how-people-become-members-of-a-program}

1. Uma pessoa preenche um [formulário em uma página de aterrissagem](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} no programa.

   * A pessoa terá automaticamente o primeiro status na progressão.

1. Você [importa membros para o programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md){target="_blank"} de um arquivo CSV.

   * A pessoa terá automaticamente o primeiro status na progressão.

1. Você usa a etapa de fluxo [alterar status do programa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}.
1. Uma pessoa registra ou participa de um [webinário sincronizado com um programa de evento](/help/marketo/product-docs/demand-generation/events/understanding-events/event-partners.md){target="_blank"}.
1. Uma pessoa foi [criada usando o aplicativo de check-in Marketo iPad](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md){target="_blank"}.
1. Uma pessoa é adicionada a uma Campanha do SFDC, que está [sincronizada com o programa](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}.

>[!NOTE]
>
>Para um programa de email, uma pessoa é adicionada à associação somente quando o email é enviado.

## Status do programa {#program-statuses}

Os status do programa são as etapas pelas quais as pessoas passam em um programa (por exemplo, Convidado, RSVP, Presente, Não comparecer). Estas etapas são definidas pelo [canal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}.

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>Uma pessoa não pode voltar para um status anterior do programa. A progressão do status é apenas unidirecional.

## Status de sucesso {#success-statuses}

O objetivo de um programa é criar uma interação significativa com a pessoa ou prospecto. O sucesso é marcado quando uma pessoa atinge o status que atinge essa meta.

>[!NOTE]
>
>Para um webinário, registrar não é uma interação significativa se eles não assistirem ao webinário. Participar é um sucesso neste caso.

## Programa de aquisição {#acquisition-program}

Quando um novo nome entra no sistema como um membro do programa, a Marketo define automaticamente esse programa como &quot;aquisição&quot;. Isso estabelece crédito para [atribuição First-Touch](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Usar marcas em um programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/use-tags-in-a-program.md){target="_blank"}
>* [Criar um Relatório de Desempenho de Programa](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md){target="_blank"}
