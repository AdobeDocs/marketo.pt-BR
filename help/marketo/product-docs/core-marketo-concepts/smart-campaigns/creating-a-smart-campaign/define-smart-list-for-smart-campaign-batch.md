---
unique-page-id: 1146940
description: Definir lista inteligente para o Smart Campaign | Lote - Documentação do Marketo - Documentação do produto
title: Definir lista inteligente para o Smart Campaign | Lote
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Definir lista inteligente para o Smart Campaign | Lote {#define-smart-list-for-smart-campaign-batch}

As Smart Lists são o mecanismo usado no Marketo para definir &quot;quem&quot; (quais pessoas) incluir, seja um relatório, uma lista ou uma Campanha inteligente. Veja como definir uma Smart List para uma campanha em lote.

1. Escolha uma Campanha inteligente e clique em **Lista inteligente**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. Digite para procurar um filtro, arraste-o e solte-o na tela de desenho. Repita o processo para vários filtros.

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >Uma campanha inteligente com apenas filtros é executada no **Lote** modo. Ele encontra pessoas no banco de dados que se qualificam com base nos filtros e executa todas elas ao mesmo tempo pelo fluxo.

   >[!NOTE]
   >
   >Você pode fazer com que uma Campanha inteligente seja executada em uma pessoa de cada vez com base em eventos ao vivo adicionando acionadores, o que coloca a Campanha inteligente no estado **Acionador** modo.

1. Clique na lista suspensa e escolha um operador de filtro para o filtro escolhido.

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >Linhas vermelhas sinuosas indicam erros ou informações ausentes. Se não for corrigida, a campanha será inválida e não será executada.

1. Insira o valor do filtro.

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >Por padrão, as pessoas que atendem a TODAS as regras da Smart List são qualificadas. Isso pode ser modificado para atender às suas necessidades de campanha. Confira  [Regras da lista inteligente para lógica complexa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md) para saber mais.

   Para acionar em eventos ao vivo uma pessoa por vez, saiba como [Definir lista inteligente para o Smart Campaign | Acionador](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md).

   >[!MORELIKETHIS]
   >
   >* [Definir lista inteligente para o Smart Campaign | Acionador](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [Adicionar uma etapa de fluxo a uma campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
