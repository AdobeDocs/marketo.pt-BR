---
unique-page-id: 2360181
description: Saiba mais sobre o rastreamento de atividades anônimas e pessoas no Marketo Engage, incluindo o rastreamento de atividades anônimas e. Use este guia para concluir a próxima etapa.
title: Rastreamento de atividades anônimas e pessoas
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
TQID: https://experienceleague.adobe.com/BZakQFVtQystRyrlzo81s-p8N65LXHUJ2ZoSAzeTG6Q
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 255
ht-degree: 8%

---

# Rastreamento de atividades anônimas e pessoas {#tracking-anonymous-activity-and-people}

Na primeira vez que alguém visitar uma [página de aterrissagem](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) do Marketo (ou uma página do seu site que tenha o [código de rastreamento do Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), o Marketo criará uma _atividade anônima_ e usará um cookie de navegador para rastreá-la. Uma vez identificado, o visitante se torna uma pessoa e o histórico associado ao cookie do navegador é mesclado no.

1. Uma atividade anônima é criada quando alguém:

   * Visita sua [página de aterrissagem](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) do Marketo pela primeira vez.
   * Visita uma página do seu site que tem [rastreamento do Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Clica no link [Exibir como Página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) em um email do Marketo.

   >[!NOTE]
   >
   >Ao contrário de outros links em emails do Marketo, Exibir como página da Web não é rastreado como um clique de email.

   Uma atividade anônima é mesclada em uma pessoa nova ou existente quando alguém:

   * Clica em um [link em um email do Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Preenche um [formulário](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) do Marketo.
   * Usa a [REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads) ou a [Munchkin](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking) API da Marketo (para desenvolvedores) para associar uma atividade anônima a um registro conhecido.

   Um nome no banco de dados pode estar vinculado a muitos cookies, pois as pessoas geralmente usam diferentes dispositivos e navegadores para visitar seu site.

   >[!NOTE]
   >
   >Quando registros anônimos são mesclados em um registro de pessoa novo ou existente, os valores de campo personalizado **não** são transferidos.

   >[!MORELIKETHIS]
   >
   >[Exibir Pessoas ou Visitantes Anônimos em Relatórios da Web](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
