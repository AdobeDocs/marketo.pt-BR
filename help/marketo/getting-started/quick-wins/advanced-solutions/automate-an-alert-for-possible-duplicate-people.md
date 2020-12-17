---
unique-page-id: 7513680
description: Automatize um alerta para possíveis Duplicados - Documentos do Marketing Cloud - Documentação do produto
title: Automatizar um alerta para possíveis pessoas do Duplicado
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---


# Automatizar um alerta para possíveis pessoas do Duplicado {#automate-an-alert-for-possible-duplicate-people}

Deseja um alerta sempre que um duplicado for criado? Veja como configurar uma Campanha inteligente para fazer isso.

1. [Crie uma nova campanha](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) inteligente. Defina a seguinte lista inteligente:

* Acionador: **A pessoa foi criada**
* Filtro: **Campos de Duplicado.** Nome completo  **do campo**

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Seja criativo. Experimente campos diferentes para obter melhores resultados de filtragem.

1. Na etapa de fluxo, escolha [Enviar alerta](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) ação de fluxo.

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >Usar o token [Enviar informações de alerta](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) para incluir um link para a pessoa em seu CRM.

   >[!CAUTION]
   >
   >Se você importar uma lista grande, você pode receber vários desses alertas ao mesmo tempo!
   >
   >Além disso, duas pessoas com o mesmo nome não significa automaticamente que elas sejam a mesma pessoa.

1. Ative a campanha na guia **Schedule**.

   ![](assets/image2017-3-27-8-3a24-3a37.png)

É isso! Essa campanha inteligente será acionada toda vez que uma nova pessoa com um nome completo existente for criada no Marketo.

>[!MORELIKETHIS]
>
>[Localizar e mesclar pessoas do Duplicado](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)
