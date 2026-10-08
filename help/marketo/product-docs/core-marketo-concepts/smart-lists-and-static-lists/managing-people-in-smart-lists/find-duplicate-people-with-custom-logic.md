---
unique-page-id: 2952636
description: Saiba como encontrar pessoas duplicadas com lógica personalizada. Crie uma Smart List para identificar duplicatas de acordo com seus critérios.
title: Localizar pessoas duplicadas com lógica personalizada
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
TQID: 'https://experienceleague.adobe.com/-NvWt-eEzngL0QY7Kyl6lfjd75WcoQmcq3IiN7Uc6-w'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 12%
---
# Localizar pessoas duplicadas com lógica personalizada {#find-duplicate-people-with-custom-logic}

O Marketo Engage tem uma Lista inteligente de sistemas que encontra pessoas duplicadas ao corresponder seus endereços de email. Se quiser usar outro campo para encontrar duplicatas, siga as etapas abaixo.

>[!PREREQUISITES]
>
>[Criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Acesse a área **[!UICONTROL Atividades de marketing]**.

![](assets/ma-2.png)

1. Selecione sua Smart List, clique na guia **[!UICONTROL Smart List]**.

   ![](assets/two-4.png)

1. Localize e arraste o filtro **[!UICONTROL Duplicar Campos]** para a tela.

   ![](assets/three-4.png)

1. Escolha uma das quatro opções disponíveis:

   * [!UICONTROL Endereço de email]
   * [!UICONTROL Nome completo]
   * [!UICONTROL Sobrenome]
   * [!UICONTROL Atualizado Em]

   >[!NOTE]
   >
   >Todos os campos, com exceção do Endereço de email, fazem distinção entre maiúsculas e minúsculas. Portanto, o uso de &quot;john doe&quot; no campo Nome Completo _não_ retornaria resultados para John Doe.

   ![](assets/four-2.png)

   Execute a Smart List para localizar pessoas com o mesmo valor no campo selecionado anteriormente.
