---
unique-page-id: 2360251
description: Edite a mensagem de cancelamento de inscrição - Documentos de marketing - Documentação do produto
title: Editar a mensagem de cancelamento de inscrição
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---


# Editar a mensagem de cancelamento de inscrição {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Permissões de administrador necessárias**

Ao enviar emails de marketing (não [operacionais](../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), o texto de cancelamento de inscrição e os links são anexados na parte inferior. Você pode alterar os padrões. Veja como.

## Editar a mensagem de cancelamento de inscrição {#edit-the-unsubscribe-message-1}

1. Em **Admin**, clique em **Email**.

   ![](assets/image2014-9-18-16-3a52-3a1.png)

   >[!CAUTION]
   >
   >
   >As variáveis a seguir são críticas. Não os apague!
   >
   >    
   >    
   >    * **%mkt_opt_out_prefix%**
   >    * **mkt_unsubscribe=1&amp;mkt_tok=##MKT_TOK##**


1. Edite as versões **Cancele a assinatura de HTML** e **Cancele a assinatura das versões de Texto** ao seu gosto e clique em **Salvar alterações**.

   ![](assets/image2016-8-26-13-3a40-3a55.png)

   Aí está. **Certifique-se de testar!** Você não quer que seus e-mails de marketing tenham links cancelados de cancelamento de inscrição.

>[!TIP]
>
>Você pode personalizar a posição do HTML de cancelamento de assinatura em seu email usando [tokens](../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Texto padrão de cancelamento de assinatura {#default-unsubscribe-text}

Se você precisar reverter para o cancelamento de assinatura padrão do sistema, copie/cole o seguinte:

Cancelar assinatura do HTML:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` Cancelar assinatura do texto:
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>* [Editar a mensagem &quot;Visualização como página da Web&quot;](edit-the-view-as-web-page-message.md)

>



