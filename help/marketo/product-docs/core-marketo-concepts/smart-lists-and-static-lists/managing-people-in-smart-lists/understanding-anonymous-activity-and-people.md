---
unique-page-id: 1147322
description: Compreensão da Atividade anônima e das pessoas - Documentos do Marketing - Documentação do produto
title: Entendendo Atividades anônimas e pessoas
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---


# Compreensão da Atividade anônima e das pessoas {#understanding-anonymous-activity-and-people}

Na primeira vez que alguém visita uma landing page de marketing (ou uma página em seu site que tenha o [Código de rastreamento Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), o Marketo cria uma _atividade anônima_ e usa um cookie de navegador para rastreá-la. Depois de identificado, ele se torna uma pessoa e o histórico associado ao cookie do navegador é mesclado.

**Uma atividade** Anônima é criada quando alguém:

* Visita sua landing page de marketing pela primeira vez.
* Visita uma página do site que tem [o rastreamento Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* Clique no link [Visualização como página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) em um email para marketing.

>[!NOTE]
>
>Ao contrário de outros links em emails do Marketo, [Visualização como página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) não é rastreada como um clique de email.

Uma atividade anônima é fundida em uma pessoa nova ou existente quando alguém:

* Clique em um link [em um email do Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Preenche um campo de marketing [Formulário](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* Usa a API [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) ou [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) do Marketo (para desenvolvedores) para associar uma pessoa anônima a um registro conhecido.

Um nome no banco de dados pode estar vinculado a muitos cookies, pois as pessoas geralmente usam dispositivos e navegadores diferentes para visitar seu site.

>[!NOTE]
>
>Quando registros anônimos são mesclados em um registro de pessoa novo ou existente, os valores de campo personalizado **não** serão transferidos.
