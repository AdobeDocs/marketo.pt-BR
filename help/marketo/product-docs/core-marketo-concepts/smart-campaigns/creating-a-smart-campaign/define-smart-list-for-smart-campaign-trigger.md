---
unique-page-id: 1146942
description: Definir lista inteligente para o Smart Campaign | Acionador - Documentação do Marketo - Documentação do produto
title: Definir lista inteligente para campanha inteligente | Acionável
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 5%

---

# Definir lista inteligente para campanha inteligente | Acionável {#define-smart-list-for-smart-campaign-trigger}

Faça uma Campanha inteligente ser executada em uma pessoa por vez com base em eventos ao vivo adicionando acionadores.

>[!CAUTION]
>
>Fazer edições de Smart List ou Etapa de fluxo em uma campanha ativa pode quebrar sua funcionalidade. Se você optar por fazer isso, continue com cuidado.

1. Na Campanha inteligente, clique na guia **[!UICONTROL Lista inteligente]**.

   ![](assets/define-smart-list-for-smart-campaign-trigger-1.png)

1. Procure o acionador desejado e arraste-o e solte-o na tela.

   ![](assets/define-smart-list-for-smart-campaign-trigger-2.png)

   >[!NOTE]
   >
   >Uma Campanha Inteligente com acionadores é executada no modo _Acionador_. Ele é executado em uma pessoa por vez com base em eventos acionados e em filtros adicionais.

   >[!IMPORTANT]
   >
   >Ao usar um campo booleano em uma Smart List de campanha de acionador, você deve defini-lo explicitamente como &quot;false&quot; para que o campo seja avaliado corretamente durante a execução da campanha.

1. Clique na lista suspensa e escolha um operador.

   ![](assets/define-smart-list-for-smart-campaign-trigger-3.png)

   >[!CAUTION]
   >
   >Linhas vermelhas sinuosas indicam erros ou informações ausentes. Se não for corrigida, a campanha será inválida e não será executada.

   >[!TIP]
   >
   >Em uma Campanha inteligente com acionadores e filtros, os acionadores vão para a parte superior e, quando acionados, somente as pessoas que atendem aos critérios do filtro passam pelo fluxo.

1. Defina o acionador.

   ![](assets/define-smart-list-for-smart-campaign-trigger-4.png)

   >[!NOTE]
   >
   >Com vários acionadores, uma pessoa passa pelo fluxo se _QUALQUER UM_ dos acionadores for ativado.

Para executar a campanha em um conjunto de pessoas ao mesmo tempo, saiba como [Definir a lista inteligente para a campanha inteligente | Lote](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}.

>[!MORELIKETHIS]
>
>[Adicionar uma Etapa de Fluxo a uma Campanha Inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
