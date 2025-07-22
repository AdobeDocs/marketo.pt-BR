---
unique-page-id: 1146997
description: Usar um token de data em uma etapa de fluxo de espera - Documentação do Marketo - Documentação do produto
title: Usar um token de data em uma etapa de fluxo de espera
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Usar um token de data em uma etapa de fluxo de espera {#use-a-date-token-in-a-wait-flow-step}

Você pode usar a etapa Fluxo de espera para pausar a jornada de uma pessoa em uma Campanha inteligente até uma data específica que use um token de data. Você também pode modificar a data de término por algum número de dias.

>[!NOTE]
>
>Isso se aplica somente a Campanhas de acionador. Não é possível usar esse recurso em campanhas em lote.

1. Na guia **[!UICONTROL Fluxo]** do Smart Campaign, arraste sobre a etapa de fluxo **[!UICONTROL Aguardar]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-1.png)

1. Clique no ícone de engrenagem.

   ![](assets/use-a-date-token-in-a-wait-flow-step-2.png)

1. No menu suspenso **[!UICONTROL Tipo]**, selecione **[!UICONTROL Token de data]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-3.png)

1. Escolha um [!UICONTROL Token de data] para especificar quando a etapa de espera deve terminar:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/use-a-date-token-in-a-wait-flow-step-4.png)

1. Para aguardar até o próximo aniversário da data que ocorrer no ano atual ou no próximo ano, marque a caixa.

   ![](assets/use-a-date-token-in-a-wait-flow-step-5.png)

   >[!TIP]
   >
   >Use essa opção em tokens de data que se referem a datas no passado, como uma data de aniversário ou de início de contrato.

1. Como opção, você pode modificar a data final em um número especificado de dias.

   ![](assets/use-a-date-token-in-a-wait-flow-step-6.png)

   >[!NOTE]
   >
   >Você também pode especificar o número de dias usando um token de `{{lead.` ou `{{company.` que represente um campo inteiro ou um token de `{{my.` do tipo número.

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-7.png)

   >[!MORELIKETHIS]
   >
   >* [Usar uma Duração em uma Etapa de Fluxo de Espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md){target="_blank"}
   >* [Usar uma Data Específica em uma Etapa de Fluxo de Espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
