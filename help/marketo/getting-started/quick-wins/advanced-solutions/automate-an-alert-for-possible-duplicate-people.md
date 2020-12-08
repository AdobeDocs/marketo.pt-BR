---
unique-page-id: 7513680
description: Automatize um alerta para possíveis Duplicados - Documentos do Marketing Cloud - Documentação do produto
title: Automatizar um alerta para possíveis pessoas do Duplicado
translation-type: tm+mt
source-git-commit: 3c24395e55c756184615941327e15e050fa7d0ac
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---


# Automatizar um alerta para possíveis pessoas do Duplicado {#automate-an-alert-for-possible-duplicate-people}

Deseja um alerta sempre que um duplicado for criado? Veja como configurar uma Campanha inteligente para fazer isso.

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

1. [Crie uma nova campanha](../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)inteligente. Defina a seguinte lista inteligente:

   * Acionador: **A pessoa foi criada**
   * Filtro: **Campos de Duplicado. **Nome do campo **é** Nome **** completo.

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Seja criativo. Experimente campos diferentes para obter melhores resultados de filtragem.

1. Na etapa de fluxo, escolha [Enviar fluxo de alerta](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) .

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >Usar o token [](../../../product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) Enviar informações de alerta para incluir um link para a pessoa em seu CRM.

   >[!CAUTION]
   >
   >Se você importar uma lista grande, você pode receber vários desses alertas ao mesmo tempo!
   >
   >
   >Além disso, duas pessoas com o mesmo nome não significa automaticamente que elas sejam a mesma pessoa.

1. Ative a campanha na guia **Agendamento** .

   ![](assets/image2017-3-27-8-3a24-3a37.png)

É isso! Essa campanha inteligente será acionada toda vez que uma nova pessoa com um nome completo existente for criada no Marketo.

>[!MORELIKETHIS]
>
>* [Localizar e mesclar pessoas do Duplicado](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)

