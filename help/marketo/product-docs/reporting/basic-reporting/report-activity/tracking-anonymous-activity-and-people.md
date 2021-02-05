---
unique-page-id: 2360181
description: Rastreamento de Atividades e pessoas anônimas - Documentos de marketing - Documentação do produto
title: Rastrear Atividades e pessoas anônimas
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---


# Rastrear Atividade anônima e pessoas {#tracking-anonymous-activity-and-people}

Na primeira vez que alguém visita um Marketo [landing page](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (ou uma página no seu site que tenha o [código de rastreamento Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), o Marketo cria um *anônimo* *atividade* e usa um cookie de navegador para rastreá-lo. Depois que o visitante é identificado, ele se torna uma pessoa e o histórico associado ao cookie do navegador é mesclado.

1. Uma atividade anônima é criada quando alguém:

   * Visita seu Marketing [landing page](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) pela primeira vez.
   * Visita uma página do site que tem [o rastreamento Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Clique no link [Visualização como página da Web](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) em um email para marketing.

   >[!NOTE]
   >
   >Ao contrário de outros links em emails do Marketo, a Visualização como página da Web não é rastreada como um clique por email.

   Uma atividade anônima é fundida em uma pessoa nova ou existente quando alguém:

   * Clique em um link [em um email do Marketo](../../../../product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Preenche um formulário Marketo [form](http://docs.marketo.com/display/docs/forms).
   * Usa a API [REST API](http://developers.marketo.com/rest-api/lead-database/leads/) ou [Munchkin](http://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) do Marketo (para desenvolvedores) para associar uma atividade anônima a um registro conhecido.

   Um nome no banco de dados pode estar vinculado a muitos cookies, pois as pessoas geralmente usam dispositivos e navegadores diferentes para visitar seu site.

   >[!NOTE]
   >
   >Quando registros anônimos são mesclados em um registro de pessoa novo ou existente, os valores de campo personalizado **não** serão transferidos.

   >[!MORELIKETHIS]
   >
   >
   >    
   >    
   >    * [Exibir pessoas ou Visitantes anônimos em relatórios da Web](display-people-or-anonymous-visitors-in-web-reports.md)


   >[!NOTE]
   >
   >**Mergulho profundo**
   >
   >
   >Saiba mais sobre [Relatórios básico](http://docs.marketo.com/display/docs/basic+reporting).

