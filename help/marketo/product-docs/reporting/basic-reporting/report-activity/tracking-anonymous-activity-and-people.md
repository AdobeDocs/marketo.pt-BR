---
unique-page-id: 2360181
description: Rastreamento de atividades anônimas e pessoas - Documentos do Marketo - Documentação do produto
title: Rastreamento de atividades anônimas e pessoas
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# Rastreamento de atividades anônimas e pessoas {#tracking-anonymous-activity-and-people}

A primeira vez que alguém visita uma Marketo [página de aterrissagem](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (ou uma página do seu site que tenha a variável [Código de rastreamento do Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), o Marketo cria um _atividade anônima_ e usa um cookie do navegador para rastreá-lo. Depois que o visitante é identificado, ele se torna uma pessoa e o histórico associado ao cookie do navegador é mesclado.

1. Uma atividade anônima é criada quando alguém:

   * Visita sua Marketo [página de aterrissagem](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) pela primeira vez.
   * Visita uma página do site que tem [Rastreamento do Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Clica no botão [Exibir como página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) em um email do Marketo.

   >[!NOTE]
   >
   >Ao contrário de outros links nos emails do Marketo, a opção Exibir como página da Web não é acompanhada como um clique por email.

   Uma atividade anônima é mesclada em uma pessoa nova ou existente quando alguém:

   * Cliques em um [link em um email do Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Preenche um Marketo [formulário](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * Usa Marketo [REST API](https://developers.marketo.com/rest-api/lead-database/leads/) ou [Munchkin](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) API (para desenvolvedores) para associar uma atividade anônima a um registro conhecido.

   Um nome no banco de dados pode estar vinculado a muitos cookies, pois as pessoas geralmente usam dispositivos e navegadores diferentes para visitar seu site.

   >[!NOTE]
   >
   >Quando registros anônimos são mesclados em um registro de pessoa novo ou existente, os valores de campo personalizado serão **not** transferência.

   >[!MORELIKETHIS]
   >
   >[Exibir pessoas ou visitantes anônimos em relatórios da Web](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
