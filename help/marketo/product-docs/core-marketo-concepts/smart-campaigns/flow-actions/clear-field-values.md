---
unique-page-id: 1147324
description: Saiba como apagar valores de campo em uma etapa do fluxo do Campaign inteligente. Remova valores dos campos de pessoa ou empresa.
title: Limpar valores do campo
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/57QZb7T-y2JVdNeP4nhTl9PDjIX1S9GcQmRAMJ-53E0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 106
ht-degree: 5%

---

# Limpar valores do campo {#clear-field-values}

[Alterar Valor dos Dados](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) é ótimo, mas como você _remove_ o valor completamente? Boa pergunta!

1. Na etapa do fluxo, escolha o campo que deseja limpar e digite **[!UICONTROL NULL]** (todas em maiúsculas) como o **[!UICONTROL Novo valor]**.

   ![](assets/clear-field-values-1.png)

1. Após a conclusão da etapa de fluxo, o valor do campo escolhido é limpo.

   ![](assets/clear-field-values-2.png)

   >[!CAUTION]
   >
   >Deixar o novo valor em branco ou inserir um ESPAÇO não esvaziará realmente o campo. Você deve digitar NULL. Além disso, lembre-se de que as etapas de fluxo não podem ser desfeitas após a execução.
