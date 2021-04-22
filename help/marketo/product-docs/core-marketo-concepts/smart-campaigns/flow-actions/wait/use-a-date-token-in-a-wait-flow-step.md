---
unique-page-id: 1146997
description: Usar um token de data em uma etapa de fluxo de espera - Documentos do Marketo - Documentação do produto
title: Usar um token de data em uma etapa de fluxo de espera
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Usar um token de data em uma etapa de fluxo de espera {#use-a-date-token-in-a-wait-flow-step}

Você pode usar a etapa Fluxo de espera para pausar a jornada de uma pessoa por meio de uma campanha inteligente até uma data específica que use um token de data. Também é possível modificar a data final em alguns dias.

>[!NOTE]
>
>Isso se aplica somente às campanhas do acionador. Não é possível usar esse recurso em campanhas em lote.

1. Na guia **Fluxo** da campanha inteligente, arraste sobre a etapa de fluxo **Aguardar**.

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Clique no ícone de engrenagem à direita.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. No menu suspenso **Type**, selecione **Token de data**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Escolha um token de Data para especificar quando a etapa Aguardar deve terminar:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Marque a caixa para aguardar até o próximo aniversário da data que ocorre no ano civil atual ou próximo.

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Use essa opção em tokens de data que se referem a datas anteriores, como data de nascimento ou data de início de contrato.

1. Opcionalmente, é possível modificar a data final em um número especificado de dias.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >Você também pode especificar o número de dias usando um token `{{lead.` ou `{{company.` que representa um campo inteiro ou um token `{{my.` do tipo de número.

1. Clique em **Salvar**.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [Usar uma duração em uma etapa do fluxo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
   >* [Usar uma Data Específica em uma Etapa de Fluxo de Espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)

