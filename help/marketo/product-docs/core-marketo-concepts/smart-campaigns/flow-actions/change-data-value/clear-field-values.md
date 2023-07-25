---
unique-page-id: 1147324
description: Limpar valores de campo - Documentação do Marketo - Documentação do produto
title: Limpar Valores do Campo
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---

# Limpar Valores do Campo {#clear-field-values}

[Alterar valor dos dados](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) é ótimo, mas como você _remover_ o valor completamente? Boa pergunta!

1. Na etapa de fluxo, escolha o campo que deseja limpar e digite **NULL** (todas em maiúsculas) como a **Novo Valor**.

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. Boom! Aposto que você não sabia disso! Após a conclusão da etapa de fluxo, o valor do campo escolhido é limpo.

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >Deixar o novo valor em branco ou simplesmente inserir um ESPAÇO não esvaziará o campo. Você deve digitar NULL. Além disso, lembre-se, as etapas de fluxo não podem ser desfeitas após a execução.
