---
unique-page-id: 1147322
description: Compreensão da Atividade anônima e das pessoas - Documentos do Marketing - Documentação do produto
title: Entendendo Atividades anônimas e pessoas
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Entendendo Atividades anônimas e pessoas {#understanding-anonymous-activity-and-people}

Na primeira vez que alguém visita um Marketo [l `anding page`](http://docs.marketo.com/display/DOCS/Personalizing+Landing+Pages) (ou uma página em seu site que tem o Código [de rastreamento](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)Munchkin), o Marketo cria uma **atividade* *anônima e usa um cookie de navegador para rastreá-la. Depois de identificado, ele se torna uma pessoa e o histórico associado ao cookie do navegador é mesclado.

**Uma atividade Anônima** é criada quando alguém:

* Visita sua landing page de marketing pela primeira vez.

* Visita uma página do site que tem o rastreamento [de](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)Munchkin.

* Clique no link [Visualização como página](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) da Web em um email para Marketo.

>[!NOTE]
>
>Ao contrário de outros links em emails do Marketo, a [Visualização como página](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) da Web não é rastreada como um clique por email.

Uma atividade anônima é fundida em uma pessoa nova ou existente quando alguém:

* Clique em um [link em um email](../../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)do Marketo.
* Preenche um [formulário](../../../../product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md)de marketing.
* Usa a API [SOAP](http://docs.marketo.com/pages/viewpage.action?pageid=7509846) ou [Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) do Marketo (para desenvolvedores) para associar uma pessoa anônima a um registro conhecido.

Um nome no banco de dados pode estar vinculado a muitos cookies, pois as pessoas geralmente usam dispositivos e navegadores diferentes para visitar seu site.

>[!NOTE]
>
>Quando registros anônimos são mesclados em um registro de pessoa novo ou existente, os valores de campo personalizado **não** são transferidos.

