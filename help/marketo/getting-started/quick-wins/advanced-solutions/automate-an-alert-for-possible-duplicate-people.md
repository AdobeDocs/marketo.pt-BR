---
unique-page-id: 7513680
description: Automatizar um alerta para possíveis pessoas duplicadas - Documentação do Marketo - Documentação do produto
title: Automatizar um Alerta para Possíveis Pessoas Duplicadas
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Automatizar um Alerta para Possíveis Pessoas Duplicadas {#automate-an-alert-for-possible-duplicate-people}

Deseja receber um alerta sempre que uma pessoa duplicada possível for criada? Veja como configurar uma Campanha inteligente para fazer isso.

1. [Criar uma nova campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}. Defina a seguinte lista inteligente:

* Acionador: **[!UICONTROL A pessoa foi criada]**
* Filtro: **[!UICONTROL Duplicar campos]**. Nome do campo **[!UICONTROL é] [!UICONTROL Nome completo]**

  ![](assets/automate-an-alert-1.png)

  >[!TIP]
  >
  >Seja criativo. Experimente com campos diferentes para obter melhores resultados de filtragem.

1. Na etapa de fluxo, escolha [[!UICONTROL Enviar alerta]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target="_blank"} ação de fluxo.

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >Usar o [Enviar token de informações de alerta](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"} para incluir um link para a pessoa em seu CRM.

   >[!CAUTION]
   >
   >Se você importar uma lista grande, poderá receber vários desses alertas de uma só vez!
   >
   >Além disso, duas pessoas com o mesmo nome não significa automaticamente que são a mesma pessoa.

1. Ativar a campanha no **[!UICONTROL Agendar]** guia.

   ![](assets/automate-an-alert-3.png)

Pronto! Esta campanha inteligente será acionada sempre que uma nova pessoa com um nome completo existente for criada no Marketo.

>[!MORELIKETHIS]
>
>[Localizar e Mesclar Pessoas Duplicadas](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}
