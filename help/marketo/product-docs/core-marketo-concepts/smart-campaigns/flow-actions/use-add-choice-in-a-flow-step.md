---
unique-page-id: 1146980
description: Use Adicionar escolha em uma etapa de fluxo - Documentação do Marketo - Documentação do produto
title: Usar Adicionar escolha em uma etapa de fluxo
exl-id: 50ffcd60-48ee-4341-94d8-170c63bc9ecb
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Usar Adicionar escolha em uma etapa de fluxo {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>[Adicionar uma Etapa de Fluxo a uma Campanha Inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

&quot;Adicionar escolha&quot; permite usar uma etapa de fluxo e dizer &quot;depende&quot; ao escolher os detalhes.

1. Na guia **[!UICONTROL Fluxo]** do Smart Campaign, adicione qualquer etapa de fluxo e clique em **[!UICONTROL Adicionar opção]**.

   ![](assets/use-add-choice-in-a-flow-step-1.png)

1. Selecione a condição de escolha.

   ![](assets/use-add-choice-in-a-flow-step-2.png)

1. Escolha o operador e insira um valor de escolha. Isso define seus critérios ou sua escolha.

   ![](assets/use-add-choice-in-a-flow-step-3.png)

1. Informe um valor de etapa de fluxo para a escolha.

   ![](assets/use-add-choice-in-a-flow-step-4.png)

   >[!CAUTION]
   >
   >Os tokens _não_ funcionarão na parte de condição de uma etapa de fluxo de escolha.

1. Repita as etapas acima para adicionar várias opções e, em seguida, adicione/ajuste o valor padrão.

   ![](assets/use-add-choice-in-a-flow-step-5.png)

   >[!TIP]
   >
   >Você pode definir qualquer uma de suas etapas de fluxo como —Não fazer nada—, nesse caso, nenhuma ação será tomada sobre essa escolha.

   >[!CAUTION]
   >
   >Somente a primeira opção correspondente é aplicada à etapa do fluxo. Saiba como [reordenar &quot;Adicionar opção&quot; em uma ação de fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}.

   Ótimo! Agora você pode criar uma única Campanha inteligente com opções de etapa de fluxo em vez de criar várias Campanhas inteligentes para cada escolha.

   >[!MORELIKETHIS]
   >
   >[Reordenar Adicionar Opção em uma Etapa de Fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}
