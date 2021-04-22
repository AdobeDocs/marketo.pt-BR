---
unique-page-id: 1147322
description: Noções básicas sobre atividade anônima e pessoas - Documentos do Marketo - Documentação do produto
title: Entendendo a atividade anônima e as pessoas
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---

# Como entender a atividade anônima e as pessoas {#understanding-anonymous-activity-and-people}

Na primeira vez que alguém visita uma página de aterrissagem do Marketo (ou uma página em seu site que tem o [Código de rastreamento do Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), o Marketo cria um _atividade anônima_ e usa um cookie de navegador para rastreá-lo. Depois de identificado, ele se torna uma pessoa e o histórico associado ao cookie do navegador é mesclado.

**Uma atividade** Anônima é criada quando alguém:

* Visita a página de aterrissagem do Marketo pela primeira vez.
* Visita uma página em seu site que tem [Munchkin tracking](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* Clica no link [Exibir como página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) em um email do Marketo.

>[!NOTE]
>
>Ao contrário de outros links nos emails do Marketo, [Exibir como página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) não é rastreado como um clique de email.

Uma atividade anônima é mesclada em uma pessoa nova ou existente quando alguém:

* Clica em um link [em um email do Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Preenche um Marketo [Form](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* Usa a API Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) ou [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) (para desenvolvedores) para associar uma pessoa anônima a um registro conhecido.

Um nome no banco de dados pode estar vinculado a muitos cookies, pois as pessoas geralmente usam dispositivos e navegadores diferentes para visitar seu site.

>[!NOTE]
>
>Quando registros anônimos são mesclados em um registro de pessoa novo ou existente, os valores de campo personalizado **not** são transferidos.
