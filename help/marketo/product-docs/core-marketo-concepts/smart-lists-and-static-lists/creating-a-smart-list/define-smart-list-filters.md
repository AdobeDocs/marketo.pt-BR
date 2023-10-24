---
unique-page-id: 557316
description: Definir Filtros De Smart List - Documentação Do Marketo - Documentação Do Produto
title: Definir filtros da lista inteligente
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 198d7d7fd4c1c312aeb30fa922fd89863ac87f81
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 1%

---

# Definir filtros da lista inteligente {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Localizar e adicionar filtros a Smart Lists](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

Agora que você já [criou uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} and [added filters](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"} para isso, vamos definir os filtros. Veja como.

Continuando nosso exemplo, vamos definir esses filtros para encontrar todas as pessoas na Califórnia com uma pontuação acima de 50.

1. Ir para **[!UICONTROL Atividades de marketing]**.

   ![](assets/login-marketing-activities-1.png)

1. Selecione a Smart List e clique no botão **[!UICONTROL Lista inteligente]** guia.

   ![](assets/smarlist-choosefilters.png)

1. Localize e selecione &quot;CA&quot; para a variável **[!UICONTROL Estado]** filtro.

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >Você pode estar armazenando &quot;Califórnia&quot; e &quot;CA&quot;. Para filtrar por valores e incluir _all_ pessoas da Califórnia, aprendam a  [adicionar vários valores a um filtro Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}.

1. Escolha o **[!UICONTROL maior que]** e digite &quot;50&quot;.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>Se você acha que pode ter alguns registros no banco de dados que contêm endereços de email incompletos (por exemplo, apenas &quot;@adobe.com&quot;), use dois filtros de Endereço de email quando estiver usando o operador &quot;contains&quot;. Um filtro com &quot;contém @adobe.com&quot; e um filtro separado com &quot;contém adobe.com&quot; (deixando de fora o símbolo @).

Agora você sabe como criar uma Smart List e adicionar/definir filtros.
