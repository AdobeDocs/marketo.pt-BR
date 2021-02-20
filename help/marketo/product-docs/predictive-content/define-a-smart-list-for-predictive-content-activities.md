---
unique-page-id: 10097873
description: Definir uma Lista inteligente para Atividades de conteúdo preditivo - Documentos do Marketing - Documentação do produto
title: Definir uma Lista inteligente para Atividades de conteúdo preditivo
translation-type: tm+mt
source-git-commit: f1d7b270454ba41db5197a069e0dcc2caebdec63
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---


# Definir uma Lista inteligente para Atividades de conteúdo preditivo {#define-a-smart-list-for-predictive-content-activities}

Você pode usar atividades de conteúdo preditivo em acionadores e filtros ao definir uma lista inteligente em uma campanha inteligente. Você pode acionar uma ação para qualquer pessoa que clicar em conteúdo preditivo por meio do [modelo Rich Media](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md), da [Barra de recomendação de conteúdo](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md) ou em um [email](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md).

1. Na sua campanha inteligente, navegue até a guia **Lista inteligente**.

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >Listas inteligentes podem fazer coisas incríveis. Saiba mais no mergulho profundo [lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. Procure o acionador e arraste e solte-o na tela.

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >Uma campanha inteligente com acionadores é executada no modo Acionador. Ele é executado em uma pessoa de cada vez com base nos eventos acionados e nos filtros adicionados.

1. Clique no menu suspenso **Name** e selecione um operador.

   ![](assets/smart-list-dropdown-hands.png)

1. Defina o acionador.

   ![](assets/smart-lislt-select-content-hands.png)

1. Adicione a restrição **Type**.

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. Selecione a fonte necessária para a sua lista inteligente.

   ![](assets/pc-add-constraint.png)

1. Se você estiver usando a fonte de email para seu conteúdo preditivo, adicione o acionador **Clicks Link em Email**. Selecione seu email e adicione a restrição **Is Predictive**, definida como **true**.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. Adicione outros filtros, conforme necessário.

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >Em uma campanha inteligente com filtros e acionadores, os acionadores ficam no topo. Quando acionado, somente as pessoas que atendem aos critérios de filtragem passam pelo fluxo.

   >[!NOTE]
   >
   >Com vários acionadores, uma pessoa passa pelo fluxo se QUALQUER um dos acionadores for ativado.

   Para executar a campanha em um conjunto de pessoas ao mesmo tempo, aprenda a [definir uma lista inteligente para uma campanha inteligente em lote](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

   >[!MORELIKETHIS]
   >
   >* [Definir Lista inteligente para Campanhas inteligentes | Lote](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [Adicionar uma Etapa de fluxo a uma Campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [Definir uma Lista inteligente para Atividades de personalização da Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [Ativar conteúdo preditivo para mídias avançadas da Web](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [Ativar a barra de recomendação de conteúdo](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)

