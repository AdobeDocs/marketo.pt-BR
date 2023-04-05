---
unique-page-id: 1146940
description: Definir Smart List para Smart Campaign | Em lote - Documentos da Marketo - Documentação do produto
title: Definir Smart List para Smart Campaign | Lote
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
source-git-commit: 56d3d05d5462c79f32f507655266e3bfa0cc6846
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Definir Smart List para Smart Campaign | Lote {#define-smart-list-for-smart-campaign-batch}

As Smart Lists são o mecanismo em todo o Marketo para definir &quot;quem&quot; (quais pessoas) para incluir, seja um relatório, uma lista ou uma Campanha inteligente. Aqui está como definir uma Smart List para uma campanha em lote.

1. Escolha uma Campanha Inteligente e clique em **Lista inteligente**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. Digite para procurar um filtro e arrastar e soltar na tela. Repita o procedimento para vários filtros.

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >Uma Campanha Inteligente com apenas filtros é executada em **Em lote** modo. Ele encontra pessoas no banco de dados que se qualificam com base nos filtros e executa todas elas pelo fluxo ao mesmo tempo.

   >[!NOTE]
   >
   >Você pode fazer com que uma Campanha inteligente seja executada em uma pessoa de cada vez com base em eventos ao vivo, adicionando acionadores, que colocam a Campanha inteligente em **Acionador** modo.

1. Clique na lista suspensa e escolha um operador de filtro para o filtro escolhido.

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >Linhas vermelhas roxas indicam erros ou informações ausentes. Se não for corrigida, a campanha será inválida e não será executada.

1. Insira o valor do filtro.

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >Por padrão, as pessoas que atendem A TODAS as regras da Smart List são qualificadas. Isso pode ser modificado para atender às suas necessidades de campanha. Veja  [Regras de Lista Inteligente para Lógica Complexa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md) para saber mais.

   Para acionar eventos ao vivo uma pessoa de cada vez, aprenda a [Definir Smart List para Smart Campaign | Acionador](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md).

   >[!MORELIKETHIS]
   >
   >* [Definir Smart List para Smart Campaign | Acionador](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [Adicionar uma etapa de fluxo a uma campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

