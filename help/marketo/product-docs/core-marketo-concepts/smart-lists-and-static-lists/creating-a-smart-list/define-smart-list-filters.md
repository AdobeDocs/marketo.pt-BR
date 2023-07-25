---
unique-page-id: 557316
description: Definir Filtros De Smart List - Documentação Do Marketo - Documentação Do Produto
title: Definir filtros da lista inteligente
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 1%

---

# Definir filtros da lista inteligente {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Criar uma lista inteligente](create-a-smart-list.md)
>* [Localizar e adicionar filtros a Smart Lists](find-and-add-filters-to-a-smart-list.md)

Agora que você já [criou uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) e [filtros adicionados](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md) para isso, vamos definir os filtros. Veja como.

Continuando nosso exemplo, vamos definir esses filtros para encontrar todas as pessoas na Califórnia com uma pontuação acima de 50.

1. Ir para **Atividades de marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Selecione a lista inteligente e clique no botão **Lista inteligente** guia.

   ![](assets/smarlist-choosefilters.png)

1. Localizar e selecionar **CA** para o **Estado** filtro.

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >Você pode estar armazenando ambos **Califórnia** e **CA**. Para filtrar por valores e incluir _all_ pessoas da Califórnia, aprendam a  [adicionar vários valores a um filtro de lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md).

1. Escolha o **maior que** operador e insira **50**.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>Se você acha que pode ter alguns registros no banco de dados que contêm endereços de email incompletos (por exemplo, apenas &quot;@adobe.com&quot;), use **dois** O endereço de email é filtrado quando você usa o operador &quot;contém&quot;. Um filtro com &quot;contém @adobe.com&quot; e um filtro separado com &quot;contém adobe.com&quot; (deixando de fora o símbolo @).

Agora você sabe como criar uma lista inteligente e adicionar/definir filtros.
