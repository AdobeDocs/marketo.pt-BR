---
unique-page-id: 1147322
description: Entendendo atividades e pessoas anônimas - Documentação do Marketo - Documentação do produto
title: Compreender atividades anônimas e pessoas
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Compreender atividades anônimas e pessoas {#understanding-anonymous-activity-and-people}

Na primeira vez que alguém visitar uma página de aterrissagem do Marketo (ou uma página em seu site que tenha o [Código de rastreamento do Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}), o Marketo criará uma *atividade anônima* e usará um cookie de navegador para rastreá-la. Depois de identificado, ele se torna uma pessoa e o histórico associado ao cookie do navegador é mesclado no.

>[!IMPORTANT]
>
>Habilitar o Recurso do Beta **Munchkin V2 Atividade de Repetição Anônima em Conhecido** garante que as campanhas acionadas pela promoção de cliente potencial anônimo sempre serão repetidas depois que o cliente potencial anônimo for mesclado com êxito no registro conhecido. Como resultado, os campos personalizados alterados pelas etapas Alterar valor dos dados em qualquer campanha repetida serão retidos no registro conhecido.

**Uma atividade Anônima** é criada quando alguém:

* Visita a página de aterrissagem do Marketo pela primeira vez.
* Visita uma página do seu site que tem [rastreamento de Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.
* Clica no link [Exibir como Página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} em um email do Marketo.

>[!NOTE]
>
>Ao contrário de outros links em emails do Marketo, a [Exibir como Página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} não é rastreada como um clique de email.

Uma atividade anônima é mesclada em uma pessoa nova ou existente quando alguém:

* Clica em um [link em um email do Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}.
* Preenche um [Formulário](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"} do Marketo.
* Usa a API [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md){target="_blank"} ou [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} do Marketo (para desenvolvedores) para associar uma pessoa anônima a um registro conhecido.

Um nome no banco de dados pode estar vinculado a muitos cookies, pois as pessoas geralmente usam diferentes dispositivos e navegadores para visitar seu site.

>[!NOTE]
>
>Quando registros anônimos são mesclados em um registro de pessoa novo ou existente, os valores de campo personalizado *não* são transferidos.
