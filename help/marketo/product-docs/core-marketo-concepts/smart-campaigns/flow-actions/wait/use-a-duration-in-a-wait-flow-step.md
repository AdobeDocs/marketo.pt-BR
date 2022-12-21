---
unique-page-id: 1146978
description: Usar uma duração em uma etapa do fluxo de espera - Documentos do Marketo - Documentação do produto
title: Usar uma duração em uma etapa do fluxo de espera
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Usar uma duração em uma etapa do fluxo de espera {#use-a-duration-in-a-wait-flow-step}

Você pode usar a etapa Fluxo de espera para pausar a jornada de uma pessoa por meio de uma campanha inteligente por um determinado período de tempo. Você também pode especificar critérios para o dia da semana e a hora em que ele termina.

1. Em sua campanha inteligente **Fluxo** arraste sobre a guia **Aguardar** etapa de fluxo.

   ![](assets/image2014-9-22-11-3a53-3a57.png)

1. Insira quanto tempo você deseja pausar.

   ![](assets/image2014-9-22-11-3a54-3a0.png)

1. Pronto! O fluxo será pausado pela duração especificada. Para opções avançadas, clique no ícone de engrenagem à direita.

   ![](assets/image2014-9-22-11-3a54-3a7.png)

1. Especifique o dia da semana em que a etapa de espera deve terminar.

   ![](assets/image2014-9-22-11-3a54-3a10.png)

1. Como opção, especifique a hora. Clique em **Salvar**.

   ![](assets/image2014-9-22-11-3a54-3a35.png)

   >[!NOTE]
   >
   >**Exemplo**
   >
   >Uma pessoa dispara uma campanha inteligente na sexta-feira às 17h. A etapa de espera é avançada: 48 horas e deve terminar em segunda-feira às 9h.
   >
   >O resultado seria que a pessoa continuaria no fluxo de **Segunda-feira, 9h**. Esta é a primeira data M-F após 48 horas.

   >[!NOTE]
   >
   >A duração, as datas, os horários e os dias usados são baseados no fuso horário da sua assinatura.

   >[!MORELIKETHIS]
   >
   >* [Usar uma Data Específica em uma Etapa de Fluxo de Espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
   >* [Usar um token de data em uma etapa de fluxo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)

