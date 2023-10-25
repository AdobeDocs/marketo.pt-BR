---
unique-page-id: 2949413
description: Adicionar uma restrição a um filtro de lista inteligente - Documentação do Marketo - Documentação do produto
title: Adicionar uma restrição a um filtro de lista inteligente
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: aeefe7a5c265e3a7ddd50920820742a463ab178a
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 1%

---

# Adicionar uma restrição a um filtro de lista inteligente {#add-a-constraint-to-a-smart-list-filter}

Ao criar a Smart List, alguns filtros têm opções avançadas chamadas &quot;restrições&quot;. Essas são condições extras que podem ser adicionadas a filtros e acionadores para ajudar a limitar ainda mais a pesquisa.

Neste exemplo, vamos adicionar algumas restrições a um **[Valor dos dados alterado](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}** filtro para localizar pessoas que tiveram uma alteração de Status de MQL para SQL.

>[!PREREQUISITES]
>
>* [Criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Usar o filtro &quot;Valor dos dados alterado&quot; em uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md){target="_blank"}

1. Ir para **[!UICONTROL Atividades de marketing]**.

   ![](assets/ma-1.png)

1. Selecione a Smart List com um filtro ao qual você adicionará uma restrição e clique no **[!UICONTROL Lista inteligente]** guia.

   ![](assets/two-3.png)

1. Em **[!UICONTROL Adicionar Restrição]**, selecione **[!UICONTROL Valor anterior]**.

   ![](assets/three-3.png)

1. Insira o **[!UICONTROL Valor anterior]**. Neste exemplo, estamos usando MQL.

   ![](assets/four-2.png)

1. Em **[!UICONTROL Adicionar Restrição]**, selecione **[!UICONTROL Novo Valor]**.

   ![](assets/five.png)

1. Insira o novo valor. Neste exemplo, estamos usando SQL.

   ![](assets/six.png)

1. Muito bem! Clique em **[!UICONTROL Pessoas]** guia para ver todas as pessoas que tiveram um Status alterado de &quot;MQL&quot; para &quot;SQL&quot; nos últimos 30 dias.
