---
unique-page-id: 2949413
description: Adicionar uma restrição a um filtro de lista inteligente - Documentos do Marketo - Documentação do produto
title: Adicionar uma restrição a um filtro de lista inteligente
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 1%

---

# Adicionar uma restrição a um filtro de lista inteligente {#add-a-constraint-to-a-smart-list-filter}

Ao criar listas inteligentes, alguns filtros têm opções avançadas chamadas &quot;restrições&quot;. Essas são condições adicionais que você pode adicionar a filtros e acionadores para ajudar a limitar ainda mais sua pesquisa.

Neste exemplo, vamos adicionar algumas restrições a um filtro **[Data Value Changed](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)** para encontrar pessoas que tiveram uma alteração de status do MQL para o SQL.

>[!PREREQUISITES]
>
>* [Criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [Usar o filtro &quot;Valor de dados alterado&quot; em uma Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md)

>



1. Vá para **Marketing Activities**.

   ![](assets/ma-1.png)

1. Selecione a lista inteligente com um filtro ao qual você adicionará uma restrição e clique na guia **Smart List**.

   ![](assets/two-3.png)

1. Em **Adicionar restrição**, selecione **Valor anterior**.

   ![](assets/three-3.png)

1. Insira o **Valor anterior**. Neste exemplo, estamos usando MQL.

   ![](assets/four-2.png)

1. Em **Adicionar restrição**, selecione **Novo valor**.

   ![](assets/five.png)

1. Insira o **Novo Valor**. Neste exemplo, estamos usando SQL.

   ![](assets/six.png)

1. Muito bem! Clique na guia **People** para ver todas as pessoas que tiveram **Status** alterar de **MQL** para **SQL** nos últimos 30 dias.
