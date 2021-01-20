---
unique-page-id: 1146997
description: Usar um token de data em uma etapa de fluxo de espera - Documentos do Marketing - Documentação do produto
title: Usar um token de data em uma etapa de fluxo de espera
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# Usar um token de data em uma Etapa de fluxo de espera {#use-a-date-token-in-a-wait-flow-step}

Você pode usar a etapa de fluxo de Espera para pausar a jornada de uma pessoa por meio de uma campanha inteligente até uma data específica que usa um token de data. Você também pode modificar a data final em alguns dias.

>[!NOTE]
>
>Isso se aplica somente às campanhas de acionamento. Não é possível usar esse recurso em campanhas em lote.

1. Na guia **Fluxo** da campanha inteligente, arraste sobre a etapa de fluxo **Aguarde**.

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Clique no ícone de engrenagem à direita.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. Na lista suspensa **Tipo**, selecione **Token de data**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Escolha um token de Data para especificar quando a etapa de Espera deve terminar:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Marque a caixa para aguardar até o próximo aniversário da data que ocorre no ano civil atual ou no próximo.

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Use essa opção em tokens de data que se referem a datas anteriores, como data de aniversário ou data de start do contrato.

1. Como opção, você pode modificar a data final em um número especificado de dias.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >Você também pode especificar o número de dias usando um token `{{lead.` ou `{{company.` que representa um campo inteiro ou um token `{{my.` do tipo de número.

1. Clique em **Salvar**.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [Usar uma duração em uma etapa do fluxo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
   >* [Usar uma data específica em uma etapa de fluxo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)

