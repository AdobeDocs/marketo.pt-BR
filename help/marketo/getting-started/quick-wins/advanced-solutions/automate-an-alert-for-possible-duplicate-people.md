---
unique-page-id: 7513680
description: Automatizar um alerta para possíveis pessoas duplicadas - Documentos do Marketo - Documentação do produto
title: Automatizar um alerta para possíveis pessoas duplicadas
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
source-git-commit: 50fc46312d2c7c25556994fad4e118c01cf92fc0
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Automatizar um alerta para possíveis pessoas duplicadas {#automate-an-alert-for-possible-duplicate-people}

Deseja um alerta sempre que possível que uma pessoa duplicada seja criada? Veja como configurar uma Campanha inteligente para fazer isso.

1. [Criar uma nova campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target=&quot;_blank&quot;}. Defina a seguinte lista inteligente:

* Acionador: **A pessoa é criada**
* Filtro: **Duplicar campos.** Nome do campo **é Nome Completo**

   ![](assets/automate-an-alert-1.png)

   >[!TIP]
   >
   >Seja criativo. Experimente com campos diferentes para obter melhores resultados de filtragem.

1. Na etapa de fluxo, escolha [Enviar alerta](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md)Ação de fluxo {target=&quot;_blank&quot;}.

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >Usar o [Enviar token de Informações de Alerta](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;} para incluir um link para a pessoa em seu CRM.

   >[!CAUTION]
   >
   >Se você importar uma lista grande, poderá receber vários desses alertas ao mesmo tempo!
   >
   >Além disso, duas pessoas com o mesmo nome não significam automaticamente que sejam a mesma pessoa.

1. Ative a campanha no **Agendar** guia .

   ![](assets/automate-an-alert-3.png)

Pronto! Essa campanha inteligente será acionada sempre que uma nova pessoa com um nome completo existente for criada no Marketo.

>[!MORELIKETHIS]
>
>[Localizar e mesclar pessoas duplicadas](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target=&quot;_blank&quot;}
