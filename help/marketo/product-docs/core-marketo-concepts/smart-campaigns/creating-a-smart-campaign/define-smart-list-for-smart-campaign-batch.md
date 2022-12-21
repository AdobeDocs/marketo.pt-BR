---
unique-page-id: 1146940
description: Definir Smart List para Smart Campaign | Em lote - Documentos da Marketo - Documentação do produto
title: Definir Smart List para Smart Campaign | Lote
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Definir Smart List para Smart Campaign | Lote {#define-smart-list-for-smart-campaign-batch}

As listas inteligentes são o mecanismo em todo o Marketo para definir &quot;quem&quot; (quais pessoas) a serem incluídas, seja um relatório, uma lista ou uma campanha inteligente. Veja como definir uma lista inteligente para uma campanha em lote.

1. Escolha uma campanha inteligente e clique em **Lista inteligente**.

   ![](assets/campaignchoose-hand.png)

1. Digite para procurar um filtro e, em seguida, arraste e solte na tela. Repita o procedimento para vários filtros.

   ![](assets/dragin.png)

   >[!NOTE]
   >
   >Uma campanha inteligente com somente filtros é executada em **Em lote** modo. Ele encontra pessoas no banco de dados que se qualificam com base nos filtros e executa todas elas pelo fluxo ao mesmo tempo.

   >[!NOTE]
   >
   >Você pode fazer uma campanha inteligente ser executada em uma pessoa de cada vez com base em eventos ao vivo, adicionando acionadores, que colocam a campanha inteligente em **Acionador** modo.

1. Clique na lista suspensa e escolha um operador de filtro para o filtro escolhido.

   ![](assets/programdropdown-hands.png)

   >[!CAUTION]
   >
   >Linhas vermelhas roxas indicam erros ou informações ausentes. Se não for corrigida, a campanha será inválida e não será executada.

1. Insira o valor do filtro.

   ![](assets/chooseprogram.png)

   >[!NOTE]
   >
   >Por padrão, as pessoas que atendem TODAS as regras da lista inteligente são qualificadas. Isso pode ser modificado para atender às suas necessidades de campanha. Veja  [Regras de Lista Inteligente para Lógica Complexa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md) para saber mais.

   Para acionar eventos ao vivo uma pessoa de cada vez, aprenda a [Definir Smart List para Smart Campaign | Acionador](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md).

   >[!MORELIKETHIS]
   >
   >* [Definir Smart List para Smart Campaign | Acionador](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [Adicionar uma etapa de fluxo a uma campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

