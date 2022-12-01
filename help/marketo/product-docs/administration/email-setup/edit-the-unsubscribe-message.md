---
unique-page-id: 2360251
description: Editar a mensagem de cancelamento de inscrição - Documentos do Marketo - Documentação do produto
title: Editar a mensagem de cancelamento de inscrição
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
source-git-commit: aeaf1f55b81da70ac8415cab265165a3848b5a0e
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 1%

---

# Editar a mensagem de cancelamento de inscrição {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Permissões de administrador necessárias**

Ao enviar emails de marketing (não[operacional](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), o texto de cancelamento de assinatura e os links são anexados à parte inferior. Você pode alterar os padrões. Veja como.

## Onde fazer a edição {#where-to-make-the-edit}

1. Vá para o **Administrador** seção.

   ![](assets/edit-the-unsubscribe-message-1.png)

1. Clique em **Email**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >As variáveis a seguir são críticas. Não exclua!
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`


1. Edite o **Cancelar inscrição no HTML** e **Cancelar assinatura do texto** versões ao seu gosto e clique em **Salvar alterações**.

   ![](assets/edit-the-unsubscribe-message-3.png)

   Aí está. _Certifique-se de testar!_ Você não quer que seus emails de marketing tenham links de cancelamento de inscrição quebrados.

>[!TIP]
>
>Você pode personalizar a posição do HTML de cancelamento de inscrição no seu email usando [tokens](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Texto padrão para cancelar a assinatura {#default-unsubscribe-text}

Se você precisar reverter para o cancelamento de assinatura do sistema padrão, copie/cole o seguinte:

Cancelar inscrição no HTML:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` Cancelar assinatura do texto:
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[Editar a mensagem &quot;Exibir como página da Web&quot;](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
