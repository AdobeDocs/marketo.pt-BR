---
unique-page-id: 2360251
description: Editar a mensagem de cancelamento de inscrição - Documentação do Marketo - Documentação do produto
title: Editar a mensagem de cancelamento de inscrição
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 1%

---

# Editar a mensagem de cancelamento de inscrição {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Permissões de administrador necessárias**

Ao enviar emails de marketing (não-[operacionais](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), o texto de cancelamento de inscrição e os links são anexados à parte inferior. Você pode alterar os padrões. Veja como.

## Onde fazer a edição {#where-to-make-the-edit}

1. Vá para a seção **[!UICONTROL Admin]**.

   ![](assets/edit-the-unsubscribe-message-1.png)

1. Clique em **[!UICONTROL Email]**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >As variáveis a seguir são críticas. Não os exclua!
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

1. Edite as versões de **[!UICONTROL Cancelar inscrição do HTML]** e **[!UICONTROL Cancelar inscrição do texto]** de sua preferência e clique em **[!UICONTROL Salvar alterações]**.

   ![](assets/edit-the-unsubscribe-message-3.png)

   É isso aí. _Não deixe de testar!_ Você não quer que seus emails de marketing tenham links de cancelamento de inscrição desfeitos.

>[!TIP]
>
>Você pode personalizar a posição do HTML de cancelamento de inscrição no seu email usando [tokens](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Texto de cancelamento de inscrição padrão {#default-unsubscribe-text}

Se precisar reverter para o cancelamento de inscrição padrão do sistema, copie/cole o seguinte:

[!UICONTROL Cancelar inscrição do HTML]:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` [!UICONTROL Cancelar Assinatura Do Texto]:
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[Editar a Mensagem &quot;Exibir como Página da Web&quot;](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
