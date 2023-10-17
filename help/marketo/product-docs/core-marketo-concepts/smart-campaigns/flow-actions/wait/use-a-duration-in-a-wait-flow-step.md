---
unique-page-id: 1146978
description: Use uma duração em uma etapa de fluxo de espera - Documentação do Marketo - Documentação do produto
title: Usar uma duração em uma etapa de fluxo de espera
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 1%

---

# Usar uma duração em uma etapa de fluxo de espera {#use-a-duration-in-a-wait-flow-step}

Você pode usar a etapa Fluxo de espera para pausar a jornada de uma pessoa em uma Campanha inteligente por um determinado período. Você também pode especificar critérios para o dia da semana e a hora em que ela termina.

1. Em sua campanha inteligente **[!UICONTROL Fluxo]** arraste sobre a guia **[!UICONTROL Aguardar]** etapa do fluxo.

   ![](assets/image2014-9-22-11-3a53-3a57.png)

1. Insira por quanto tempo você deseja pausar.

   ![](assets/image2014-9-22-11-3a54-3a0.png)

1. Pronto! O fluxo será pausado pela duração especificada. Para opções avançadas, clique no ícone de engrenagem à direita.

   ![](assets/image2014-9-22-11-3a54-3a7.png)

1. Especifique o dia da semana em que a etapa de espera deve terminar.

   ![](assets/image2014-9-22-11-3a54-3a10.png)

1. Opcionalmente, especifique a hora. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2014-9-22-11-3a54-3a35.png)

   >[!NOTE]
   >
   >**Exemplo**
   >
   >Uma pessoa dispara uma Campanha Inteligente na sexta-feira às 17h. A etapa de espera está avançada: 48 horas e deve terminar de segunda a sexta às 9h.
   >
   >O resultado seria que a pessoa continuaria no fluxo em **Segunda-feira, 9h**. Esta é a primeira data M-F depois de 48 horas.

   >[!NOTE]
   >
   >A duração, as datas, as horas e os dias usados são todos baseados no fuso horário da sua assinatura.

   >[!MORELIKETHIS]
   >
   >* [Usar uma Data Específica em uma Etapa de Fluxo de Espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
   >* [Usar um token de data em uma etapa de fluxo de espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md){target="_blank"}
