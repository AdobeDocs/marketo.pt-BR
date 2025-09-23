---
unique-page-id: 2949413
description: Adicionar uma restrição a um filtro de lista inteligente - Documentação do Marketo - Documentação do produto
title: Adicionar uma restrição a um filtro de lista inteligente
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 9%

---

# Adicionar uma restrição a um filtro de lista inteligente {#add-a-constraint-to-a-smart-list-filter}

Ao criar uma Smart List, alguns filtros têm opções avançadas chamadas &quot;restrições&quot;. Essas são condições extras que podem ser adicionadas a filtros e acionadores para ajudar a limitar ainda mais a pesquisa.

Neste exemplo, vamos adicionar algumas restrições a um filtro **[Valor dos Dados Alterado](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}** para encontrar pessoas que tiveram uma alteração de Status de MQL para SQL.

>[!PREREQUISITES]
>
>* [Criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Usar o Filtro &quot;Valor de Dados Alterado&quot; em uma Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md){target="_blank"}

1. Vá para **[!UICONTROL Atividades de marketing]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-1.png)

1. Selecione a Smart List com um filtro ao qual você adicionará uma restrição e clique na guia **[!UICONTROL Smart List]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-2.png)

1. Em **[!UICONTROL Adicionar restrição]**, selecione **[!UICONTROL Valor anterior]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-3.png)

1. Insira o **[!UICONTROL Valor Anterior]**. Neste exemplo, estamos usando MQL.

   ![](assets/add-a-constraint-to-a-smart-list-filter-4.png)

1. Em **[!UICONTROL Adicionar restrição]**, selecione **[!UICONTROL Novo valor]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-5.png)

1. Insira o novo valor. Neste exemplo, estamos usando SQL.

   ![](assets/add-a-constraint-to-a-smart-list-filter-6.png)

1. Muito bem! Clique na guia **[!UICONTROL Pessoas]** para ver todas as pessoas que tiveram um Status alterado de &quot;MQL&quot; para &quot;SQL&quot; nos últimos 30 dias.
