---
unique-page-id: 1147322
description: Entendendo atividades e pessoas anônimas - Documentação do Marketo - Documentação do produto
title: Compreender atividades anônimas e pessoas
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Compreender atividades anônimas e pessoas {#understanding-anonymous-activity-and-people}

A primeira vez que alguém visitar uma página de aterrissagem do Marketo (ou uma página em seu site que tenha o [Código de rastreamento do Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}), o Marketo cria uma *atividade anônima* e usa um cookie do navegador para rastreá-lo. Depois de identificado, ele se torna uma pessoa e o histórico associado ao cookie do navegador é mesclado no.

>[!IMPORTANT]
>
>Ativação do recurso beta **Atividade de repetição anônima do Munchkin V2 em conhecido** A garante que as campanhas acionadas pela promoção de leads anônimos sempre sejam repetidas depois que o lead anônimo for mesclado com êxito ao registro conhecido. Como resultado, os campos personalizados alterados pelas etapas Alterar valor dos dados em qualquer campanha repetida serão retidos no registro conhecido.

**Um Anônimo** A atividade é criada quando alguém:

* Visita a página de aterrissagem do Marketo pela primeira vez.
* Visita uma página do site que contém [Rastreamento do Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.
* Clica no ícone [Exibir como página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} em um email do Marketo.

>[!NOTE]
>
>Ao contrário de outros links em emails do Marketo, [Exibir como página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} não é rastreado como um clique de email.

Uma atividade anônima é mesclada em uma pessoa nova ou existente quando alguém:

* Cliques a [link em um email do Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}.
* Preenche uma Marketo [Formulário](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"}.
* Usa o Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md){target="_blank"} or [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} API (para desenvolvedores) para associar uma pessoa anônima a um registro conhecido.

Um nome no banco de dados pode estar vinculado a muitos cookies, pois as pessoas geralmente usam diferentes dispositivos e navegadores para visitar seu site.

>[!NOTE]
>
>Quando registros anônimos são mesclados em um registro de pessoa novo ou existente, os valores de campo personalizado *não* transferência concluída.
