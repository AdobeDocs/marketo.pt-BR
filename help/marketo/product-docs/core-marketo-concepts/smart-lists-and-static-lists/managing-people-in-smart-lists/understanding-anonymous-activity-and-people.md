---
unique-page-id: 1147322
description: Noções básicas sobre atividade anônima e pessoas - Documentos do Marketo - Documentação do produto
title: Entendendo a atividade anônima e as pessoas
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
source-git-commit: cc66f4ff2e3e0e6ddfabab91215e3ad31f3b9226
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Entendendo a atividade anônima e as pessoas {#understanding-anonymous-activity-and-people}

A primeira vez que alguém visita uma página de aterrissagem do Marketo (ou uma página de seu site que tem a variável [Código de rastreamento do Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), o Marketo cria um _atividade anônima_ e usa um cookie do navegador para rastreá-lo. Depois de identificado, ele se torna uma pessoa e o histórico associado ao cookie do navegador é mesclado.

>[!IMPORTANT]
>
>Ativação do recurso Beta **Atividade de Reprodução Anônima do Munchkin V2 em Conhecido** garante que campanhas acionadas por promoção de lead anônima sejam sempre repetidas depois que o lead anônimo for mesclado com êxito ao registro conhecido. Como resultado, campos personalizados alterados pelas etapas Alterar valor de dados em qualquer campanha repetida serão retidos no registro conhecido.

**Um Anônimo** é criada quando alguém:

* Visita a página de aterrissagem do Marketo pela primeira vez.
* Visita uma página do site que tem [Rastreamento do Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* Clica no botão [Exibir como página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) em um email do Marketo.

>[!NOTE]
>
>Diferente de outros links em emails do Marketo, [Exibir como página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) não é acompanhado como um clique de email.

Uma atividade anônima é mesclada em uma pessoa nova ou existente quando alguém:

* Cliques em um [link em um email do Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Preenche um Marketo [Formulário](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* Usa Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) ou [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) API (para desenvolvedores) para associar uma pessoa anônima a um registro conhecido.

Um nome no banco de dados pode estar vinculado a muitos cookies, pois as pessoas geralmente usam dispositivos e navegadores diferentes para visitar seu site.

>[!NOTE]
>
>Quando registros anônimos são mesclados em um registro de pessoa novo ou existente, os valores de campo personalizado serão **not** transferência.
