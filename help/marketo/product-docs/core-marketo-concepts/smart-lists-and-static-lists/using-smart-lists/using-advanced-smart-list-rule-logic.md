---
unique-page-id: 1146901
description: Usar a lógica de regra da Smart List avançada - Documentos do Marketo - Documentação do produto
title: Usando a Lógica de Regra de Smart List Avançada
exl-id: fc41b6fd-c65e-4c44-b0ee-7bb5c77c51fb
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Usando a Lógica de Regra de Smart List Avançada {#using-advanced-smart-list-rule-logic}

Você pode encontrar as pessoas exatas de que precisa ao aplicar a lógica da regra da lista inteligente a vários filtros em uma lista inteligente. Veja como.

>[!PREREQUISITES]
>
>* [Localizar e adicionar filtros a uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [Definir Filtros da Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)


>[!NOTE]
>
>A lógica de filtro avançada só estará disponível se houver três ou mais filtros em sua lista inteligente.

## Adicionar lógica a uma lista inteligente {#add-logic-to-a-smart-list}

Por padrão, sua lista inteligente encontrará as pessoas que correspondem aos filtros **ALL** (filtros 1 _e_ 2 _e_ 3). Você pode alterar a lógica da regra para encontrar pessoas que correspondam a **ANY** dos filtros definidos (filtros 1 _ou_ 2 _ou_ 3) ou usar filtros avançados (filtros 1 _e_ 2 _ou_ 3).

Neste exemplo, digamos que você queira encontrar pessoas na Califórnia _e_ com uma pontuação de pelo menos 50 pontos _ou_ com um status de &quot;Vendas qualificadas&quot;.

1. Selecione **Usar filtros avançados** no menu suspenso.

   ![](assets/one.png)

   >[!NOTE]
   >
   >Usar filtros **Avançado** reduz a necessidade de criar listas inteligentes com o filtro Membro da Lista inteligente . Isso ajuda a otimizar o desempenho.

1. A caixa de texto **Advanced filters** exibirá &quot;e&quot; como o valor padrão entre todos os seus filtros.

   ![](assets/two-2.png)

1. Digite um par de parênteses em torno de &quot;2 e 3&quot;.

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >Você deve usar &quot;e&quot; antes de &quot;ou&quot; ao inserir a lógica da regra.

1. Altere o &quot;e&quot; entre &quot;2 e 3&quot; para &quot;ou&quot;.

   ![](assets/four-1.png)

## Use parênteses ao misturar &quot;And&quot; e &quot;Or {#use-parentheses-when-mixing-and-and-or}

Misturar a lógica &quot;e&quot; e &quot;ou&quot; requer parênteses para esclarecer sua intenção.

![](assets/advancedfilters-parent.png)

## Use parênteses aninhados para quatro ou mais filtros se necessário {#use-nested-parentheses-for-four-or-more-filters-if-needed}

Dependendo da sua intenção, talvez seja necessário adicionar parênteses aninhados ao usar quatro ou mais filtros.

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>Se você inserir uma regra inválida, verá uma linha vermelha sendo exibida na regra. Role sobre o texto para ver a mensagem de erro relacionada.
