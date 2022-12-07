---
unique-page-id: 2360253
description: Editar a mensagem "Exibir como página da Web" - Documentos do Marketo - Documentação do produto
title: Editar a mensagem "Exibir como página da Web"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Editar a mensagem &quot;Exibir como página da Web&quot; {#edit-the-view-as-web-page-message}

Se precisar editar o &quot;[Exibir como uma página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;texto, veja como.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Editar a mensagem &quot;Exibir como página da Web&quot; {#edit-the-view-as-web-page-message-1}

1. Vá para o **Administrador** área.

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Clique em **Email**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >As variáveis a seguir são críticas. Não exclua!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >Segunda parte `##MKT_TOK##` é o cookie da pessoa. Isso garante que eles fiquem com cookies adequadamente ao clicar no link.

1. Edite o **Exibir como HTML da página da Web** e **Exibir como texto da página da Web** versões ao seu gosto e clique em **Salvar alterações**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Certifique-se de evitar:
>
>* Adicionar URLs adicionais a uma das HTML boxes
>* Colocando HTML na versão de texto


Aí está. Envie emails de teste para garantir a formatação.

## Texto padrão &quot;Exibir como página da Web&quot; {#default-view-as-web-page-text}

Se você precisar reverter para o sistema padrão &quot;Exibir como página da Web&quot;, copie/cole o seguinte:

**Exibir como HTML da página da Web:**

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**Exibir como texto da página da Web:**

Para exibir este email como uma página da Web, vá para o seguinte endereço:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`

Pronto!
