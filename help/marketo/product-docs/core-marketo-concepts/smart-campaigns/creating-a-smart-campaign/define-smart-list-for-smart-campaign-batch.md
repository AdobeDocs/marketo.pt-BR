---
unique-page-id: 1146940
description: Definir lista inteligente para o Smart Campaign | Lote - Documentação do Marketo - Documentação do produto
title: Definir lista inteligente para o Smart Campaign | Lote
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Definir lista inteligente para o Smart Campaign | Lote {#define-smart-list-for-smart-campaign-batch}

As Smart Lists são o mecanismo usado no Marketo Engage para definir &quot;quem&quot; (quais pessoas) incluir, seja um relatório, uma lista ou uma Campanha inteligente. Veja como definir uma Smart List para uma campanha em lote.

>[!CAUTION]
>
>Fazer edições de Smart List ou Etapa de fluxo em uma campanha ativa pode quebrar sua funcionalidade. Se você optar por fazer isso, continue com cuidado.

1. Escolha uma Campanha inteligente e clique em **[!UICONTROL Lista inteligente]**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. Digite para procurar um filtro, arraste-o e solte-o na tela de desenho. Repita o processo para vários filtros.

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >Uma Campanha inteligente com apenas filtros é executada no modo _Lote_. Ele encontra pessoas no banco de dados que se qualificam com base nos filtros e executa todas elas pelo fluxo de uma vez.

   >[!NOTE]
   >
   >Você pode fazer com que uma Campanha Inteligente seja executada em uma pessoa de cada vez com base em eventos ao vivo adicionando acionadores, o que coloca a Campanha Inteligente no modo _Acionador_.

1. Clique na lista suspensa e escolha um operador de filtro para o filtro escolhido.

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >Linhas vermelhas sinuosas indicam erros ou informações ausentes. Se não for corrigida, a campanha será inválida e não será executada.

1. Insira o valor do filtro.

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >Por padrão, as pessoas que atendem a TODAS as regras da Smart List são qualificadas. Isso pode ser modificado para atender às suas necessidades de campanha. Confira as [Regras da Smart List para Lógica Complexa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"} para saber mais.

   Para acionar em eventos ao vivo uma pessoa por vez, saiba como [Definir a lista inteligente para o Smart Campaign | Gatilho](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}.

   >[!MORELIKETHIS]
   >
   >* [Definir lista inteligente para campanha inteligente | Acionador](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
   >* [Adicionar uma Etapa de Fluxo a uma Campanha Inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
