---
unique-page-id: 557316
description: Definir filtros de Smart List - Documentos Marketo - Documentação do produto
title: Definir Filtros da Smart List
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
source-git-commit: 4b1b91a933a7a6d103fe0d44ece9ea95759edc5f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 1%

---

# Definir Filtros da Smart List {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Criar uma lista inteligente](create-a-smart-list.md)
>* [Localizar e Adicionar Filtros às Smart Lists](find-and-add-filters-to-a-smart-list.md)


Agora que você [criou uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) e [filtros adicionados](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md) para isso, vamos definir os filtros. Veja como.

Continuando com nosso exemplo, vamos definir esses filtros para encontrar todas as pessoas na Califórnia com uma pontuação acima de 50.

1. Ir para **Atividades de marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Selecione a lista inteligente e clique no botão **Lista inteligente** guia .

   ![](assets/smarlist-choosefilters.png)

1. Localizar e selecionar **CA** para **Estado** filtro.

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >Você pode armazenar ambos **Califórnia** e **CA**. Para filtrar por ambos os valores e incluir _all_ pessoas da Califórnia, aprendam como  [adicionar vários valores a um filtro de lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md).

1. Escolha a **maior que** e insira **50º**.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>Se você acha que pode ter alguns registros no seu banco de dados que contêm endereços de email incompletos (por exemplo, apenas &quot;@adobe.com&quot;), use **two** Filtros de endereço de email ao usar o operador &quot;contém&quot;. Um filtro com &quot;contém @adobe.com&quot; e um filtro separado com &quot;contém adobe.com&quot; (deixando o símbolo @).

Agora você sabe como criar uma lista inteligente e adicionar/definir filtros.
