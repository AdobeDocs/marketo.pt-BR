---
unique-page-id: 557316
description: Definir Filtros De Smart List - Documentação Do Marketo - Documentação Do Produto
title: Definir filtros de lista inteligente
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 5%

---

# Definir filtros de lista inteligente {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Localizar e Adicionar Filtros às Listas Inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

Agora que você [criou uma Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} e [adicionou filtros](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"} a ela, vamos definir os filtros. Veja como.

Continuando nosso exemplo, vamos definir esses filtros para encontrar todas as pessoas na Califórnia com uma pontuação acima de 50.

1. Vá para **[!UICONTROL Atividades de marketing]**.

   ![](assets/define-smart-list-filters-1.png)

1. Selecione a Smart List desejada e clique na guia **[!UICONTROL Smart List]**.

   ![](assets/define-smart-list-filters-2.png)

1. Localize e selecione &quot;CA&quot; para o filtro **[!UICONTROL Estado]**.

   ![](assets/define-smart-list-filters-3.png)

   >[!NOTE]
   >
   >Você pode estar armazenando &quot;Califórnia&quot; e &quot;CA&quot;. Para filtrar ambos os valores e incluir _todos_ pessoas da Califórnia, saiba como [adicionar vários valores a um filtro de Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}.

1. Escolha o operador **[!UICONTROL maior que]** e digite &quot;50&quot;.

   ![](assets/define-smart-list-filters-4.png)

>[!TIP]
>
>Se você acha que pode ter alguns registros no banco de dados que contêm endereços de email incompletos (por exemplo, apenas &quot;@adobe.com&quot;), use dois filtros de Endereço de email quando estiver usando o operador &quot;contains&quot;. Um filtro com &quot;contém @adobe.com&quot; e um filtro separado com &quot;contém adobe.com&quot; (deixando de fora o símbolo @).

Agora você sabe como criar uma Smart List e adicionar/definir filtros.
