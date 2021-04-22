---
unique-page-id: 7513680
description: Automatizar um alerta para possíveis pessoas duplicadas - Documentos do Marketo - Documentação do produto
title: Automatizar um alerta para possíveis pessoas duplicadas
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Automatizar um alerta para possíveis pessoas duplicadas {#automate-an-alert-for-possible-duplicate-people}

Deseja um alerta sempre que possível que uma pessoa duplicada seja criada? Veja como configurar uma Campanha inteligente para fazer isso.

1. [Crie uma nova campanha](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) inteligente. Defina a seguinte lista inteligente:

* Acionador: **A pessoa é criada**
* Filtro: **Duplicar Campos.** Nome do campo  **é Nome completo**

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Seja criativo. Experimente com campos diferentes para obter melhores resultados de filtragem.

1. Na etapa do fluxo, escolha [Enviar alerta](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) ação do fluxo.

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >Usar o [Enviar token de informações de alerta](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) para incluir um link para a pessoa em seu CRM.

   >[!CAUTION]
   >
   >Se você importar uma lista grande, poderá receber vários desses alertas ao mesmo tempo!
   >
   >Além disso, duas pessoas com o mesmo nome não significam automaticamente que sejam a mesma pessoa.

1. Ative a campanha na guia **Schedule** .

   ![](assets/image2017-3-27-8-3a24-3a37.png)

Pronto! Essa campanha inteligente será acionada sempre que uma nova pessoa com um nome completo existente for criada no Marketo.

>[!MORELIKETHIS]
>
>[Localizar e mesclar pessoas duplicadas](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)
