---
unique-page-id: 1146997
description: Usar um token de data em uma etapa de fluxo de espera - Documentação do Marketo - Documentação do produto
title: Usar um token de data em uma etapa de fluxo de espera
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Usar um token de data em uma etapa de fluxo de espera {#use-a-date-token-in-a-wait-flow-step}

Você pode usar a etapa Fluxo de espera para pausar a jornada de uma pessoa em uma Campanha inteligente até uma data específica que use um token de data. Você também pode modificar a data de término por algum número de dias.

>[!NOTE]
>
>Isso se aplica somente a Campanhas de acionador. Não é possível usar esse recurso em campanhas em lote.

1. Em sua campanha inteligente **[!UICONTROL Fluxo]** arraste sobre a guia **[!UICONTROL Aguardar]** etapa do fluxo.

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Clique no ícone de engrenagem.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. No **[!UICONTROL Tipo]** selecione **[!UICONTROL Token de data]**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Escolha um token de Data para especificar quando a etapa de Espera deve terminar:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Para aguardar até o próximo aniversário da data que ocorrer no ano atual ou no próximo ano, marque a caixa.

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Use essa opção em tokens de data que se referem a datas no passado, como uma data de aniversário ou de início de contrato.

1. Como opção, você pode modificar a data final em um número especificado de dias.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >Você também pode especificar o número de dias usando uma `{{lead.` ou `{{company.` token que representa um campo inteiro ou um `{{my.` token do tipo de número.

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [Usar uma duração em uma etapa de fluxo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md){target="_blank"}
   >* [Usar uma Data Específica em uma Etapa de Fluxo de Espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
