---
unique-page-id: 2360181
description: Rastreamento de Atividades e pessoas anônimas - Documentos de marketing - Documentação do produto
title: Rastrear Atividades e pessoas anônimas
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---


# Rastrear Atividades e pessoas anônimas {#tracking-anonymous-activity-and-people}

Na primeira vez que alguém visita uma [landing page](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) de marketing (ou uma página em seu site que tenha o código [de rastreamento](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)Munchkin), o Marketo cria uma *atividade* anônima ** e usa um cookie de navegador para rastreá-la. Depois que o visitante é identificado, ele se torna uma pessoa e o histórico associado ao cookie do navegador é mesclado.

1. Uma atividade anônima é criada quando alguém:

   * Visita sua [landing page](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) de marketing pela primeira vez.
   * Visita uma página do site que tem o rastreamento [de](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)Munchkin.
   * Clique no link [Visualização como página](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) da Web em um email para Marketo.

   >[!NOTE]
   >
   >Ao contrário de outros links em emails do Marketo, a Visualização como página da Web não é rastreada como um clique por email.

   Uma atividade anônima é fundida em uma pessoa nova ou existente quando alguém:

   * Clique em um [link em um email](../../../../product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md)do Marketo.
   * Preenche um [formulário](http://docs.marketo.com/display/docs/forms)Marketo.
   * Usa a API [](http://developers.marketo.com/rest-api/lead-database/leads/) REST do Marketo ou a API [Munchkin](http://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) (para desenvolvedores) para associar uma atividade anônima a um registro conhecido.

   Um nome no banco de dados pode estar vinculado a muitos cookies, pois as pessoas geralmente usam dispositivos e navegadores diferentes para visitar seu site.

   >[!NOTE]
   >
   >Quando registros anônimos são mesclados em um registro de pessoa novo ou existente, os valores de campo personalizado **não** são transferidos.

   >[!NOTE]
   >
   >**Artigos relacionados**
   >
   >    
   >    
   >    * [Exibir pessoas ou Visitantes anônimos em relatórios da Web](display-people-or-anonymous-visitors-in-web-reports.md)


   >[!NOTE]
   >
   >**Mergulho profundo**
   >
   >
   >Saiba mais sobre o Relatórios [](http://docs.marketo.com/display/docs/basic+reporting)básico.

