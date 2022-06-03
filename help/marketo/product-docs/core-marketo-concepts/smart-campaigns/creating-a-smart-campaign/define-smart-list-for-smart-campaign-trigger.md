---
unique-page-id: 1146942
description: Definir Smart List para Smart Campaign | Acionador - Documentação da Marketo - Documentação do produto
title: Definir Smart List para Smart Campaign | Acionador
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
source-git-commit: a15a4b9bccb069b51186aac7b913008d15aa645e
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# Definir Smart List para Smart Campaign | Acionador {#define-smart-list-for-smart-campaign-trigger}

Faça uma campanha inteligente ser executada em uma pessoa de cada vez com base em eventos ao vivo, adicionando acionadores.

1. Na campanha inteligente, clique no botão **Lista inteligente** guia .

   ![](assets/image2014-9-19-16-3a22-3a55.png)

1. Procure o acionador e arraste e solte o acionador na tela.

   ![](assets/image2014-9-19-16-3a23-3a24.png)

   >[!NOTE]
   >
   >Uma campanha inteligente com acionadores é executada em **Acionador** modo. Ele é executado em uma pessoa de cada vez com base nos eventos acionados e em qualquer filtro adicional.

   >[!IMPORTANT]
   >
   >Ao usar um campo booleano em uma lista inteligente de campanha de acionador, você deve defini-lo explicitamente como &quot;false&quot; para que o campo seja avaliado adequadamente durante a execução da campanha.

1. Clique no menu suspenso e escolha um operador.

   ![](assets/image2014-9-19-16-3a23-3a29.png)

   >[!CAUTION]
   >
   >Linhas vermelhas roxas indicam erros ou informações ausentes. Se não for corrigida, a campanha será inválida e não será executada.

   >[!TIP]
   >
   >Em uma campanha inteligente com acionadores e filtros, os acionadores ficam na parte superior e, quando acionados, somente as pessoas que atendem aos critérios de filtragem passam pelo fluxo.

1. Defina o acionador.

   ![](assets/image2014-9-19-16-3a24-3a36.png)

   >[!NOTE]
   >
   >Com vários acionadores, uma pessoa passa pelo fluxo se **ANY** um dos acionadores é ativado.

Para executar a campanha em um conjunto de pessoas ao mesmo tempo, aprenda a [Definir Smart List para Smart Campaign | Lote](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

>[!MORELIKETHIS]
>
>[Adicionar uma etapa de fluxo a uma campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
