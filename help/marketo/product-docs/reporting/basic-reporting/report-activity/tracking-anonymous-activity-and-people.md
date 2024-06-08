---
unique-page-id: 2360181
description: Rastreamento de atividades e pessoas anônimas - Documentação do Marketo - Documentação do produto
title: Rastreamento de atividades anônimas e pessoas
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Rastreamento de atividades anônimas e pessoas {#tracking-anonymous-activity-and-people}

A primeira vez que alguém visita um Marketo [landing page](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (ou uma página no seu site que tenha o [Código de rastreamento do Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), o Marketo cria uma _atividade anônima_ e usa um cookie do navegador para rastreá-lo. Uma vez identificado, o visitante se torna uma pessoa e o histórico associado ao cookie do navegador é mesclado no.

1. Uma atividade anônima é criada quando alguém:

   * Visita a sua Marketo [landing page](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) pela primeira vez.
   * Visita uma página do site que contém [Rastreamento do Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Clica no ícone [Exibir como página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) em um email do Marketo.

   >[!NOTE]
   >
   >Ao contrário de outros links em emails do Marketo, Exibir como página da Web não é rastreado como um clique de email.

   Uma atividade anônima é mesclada em uma pessoa nova ou existente quando alguém:

   * Cliques a [link em um email do Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Preenche uma Marketo [formulário](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * Usa o Marketo [REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads) ou [Munchkin](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/lead-tracking) API (para desenvolvedores) para associar uma atividade anônima a um registro conhecido.

   Um nome no banco de dados pode estar vinculado a muitos cookies, pois as pessoas geralmente usam diferentes dispositivos e navegadores para visitar seu site.

   >[!NOTE]
   >
   >Quando registros anônimos são mesclados em um registro de pessoa novo ou existente, os valores de campo personalizado **não** transferência concluída.

   >[!MORELIKETHIS]
   >
   >[Exibir pessoas ou visitantes anônimos em relatórios da Web](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
