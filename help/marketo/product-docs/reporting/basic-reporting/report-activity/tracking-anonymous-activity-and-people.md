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

Na primeira vez que alguém visitar uma [página de aterrissagem](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) do Marketo (ou uma página em seu site que tenha o [código de rastreamento Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), o Marketo criará uma _atividade anônima_ e usará um cookie de navegador para rastreá-la. Uma vez identificado, o visitante se torna uma pessoa e o histórico associado ao cookie do navegador é mesclado no.

1. Uma atividade anônima é criada quando alguém:

   * Visita sua [página de aterrissagem](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) do Marketo pela primeira vez.
   * Visita uma página do seu site que tem [rastreamento de Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Clica no link [Exibir como Página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) em um email do Marketo.

   >[!NOTE]
   >
   >Ao contrário de outros links em emails do Marketo, Exibir como página da Web não é rastreado como um clique de email.

   Uma atividade anônima é mesclada em uma pessoa nova ou existente quando alguém:

   * Clica em um [link em um email do Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Preenche um [formulário](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) do Marketo.
   * Usa a [REST API](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/leads) ou a [Munchkin](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/lead-tracking) API da Marketo (para desenvolvedores) para associar uma atividade anônima a um registro conhecido.

   Um nome no banco de dados pode estar vinculado a muitos cookies, pois as pessoas geralmente usam diferentes dispositivos e navegadores para visitar seu site.

   >[!NOTE]
   >
   >Quando registros anônimos são mesclados em um registro de pessoa novo ou existente, os valores de campo personalizado **não** são transferidos.

   >[!MORELIKETHIS]
   >
   >[Exibir Pessoas ou Visitantes Anônimos em Relatórios da Web](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
