---
unique-page-id: 557322
description: Execute uma etapa de fluxo único em uma Smart List - Marketo Docs - Documentação do produto
title: Executar uma única etapa de fluxo a partir de uma Smart List
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 1%

---

# Executar uma única etapa de fluxo a partir de uma Smart List {#run-a-single-flow-step-from-a-smart-list}

Se quiser executar uma etapa de fluxo única, use uma única etapa de fluxo em uma lista inteligente em vez de criar uma campanha inteligente inteira.

>[!PREREQUISITES]
>
>[Criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Ir para **Atividades de marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Selecione uma lista ou lista inteligente com pessoas nela, em seguida, vá para a **Pessoas** guia .

   ![](assets/smartlistpeopletab-hands.png)

   >[!TIP]
   >
   >As listas estáticas e inteligentes têm essa funcionalidade.

1. Clique em **Selecionar tudo**. Você também pode usar **Ctrl/Cmd** e clique em para selecionar alguns registros manualmente.

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >Se os resultados se estenderem por várias páginas, clique em **Selecionar tudo** selecionará todas as pessoas em todas as páginas.

1. Em **Pessoa** **Ações**, selecione a etapa de fluxo de sua escolha. Neste exemplo, usaremos [Alterar valor de dados](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

   ![](assets/personactions-hands.png)

1. Encontre e selecione um **Atributo**. Neste exemplo, pegaremos todas as pessoas que têm o estado &quot;Califórnia&quot; e o mudaremos para &quot;CA&quot;.

   ![](assets/runaction-hands.png)

1. Inserir um novo valor. Clique em **Executar agora**.

   ![](assets/runactionnewvalue-hands.png)

1. Se você estiver alterando valores de dados para um grande número de pessoas, talvez precise confirmar a alteração digitando o número. Clique em **Ir para ele**.

   ![](assets/changedatavalue.jpg)

Trabalho incrível! Você verá o status da etapa de fluxo único no canto superior direito.

![](assets/completesingleflowaction.jpg)

Quando terminar, atualize a lista e você verá as informações atualizadas.
