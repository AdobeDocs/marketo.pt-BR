---
unique-page-id: 1147324
description: Limpar valores de campo - Documentação do Marketo - Documentação do produto
title: Limpar valores do campo
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '95'
ht-degree: 6%

---

# Limpar valores do campo {#clear-field-values}

[Alterar Valor dos Dados](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) é ótimo, mas como você _remove_ o valor completamente? Boa pergunta!

1. Na etapa do fluxo, escolha o campo que deseja limpar e digite **[!UICONTROL NULL]** (todas em maiúsculas) como o **[!UICONTROL Novo valor]**.

   ![](assets/clear-field-values-1.png)

1. Após a conclusão da etapa de fluxo, o valor do campo escolhido é limpo.

   ![](assets/clear-field-values-2.png)

   >[!CAUTION]
   >
   >Deixar o novo valor em branco ou simplesmente inserir um ESPAÇO não esvaziará o campo. Você deve digitar NULL. Além disso, lembre-se, as etapas de fluxo não podem ser desfeitas após a execução.
