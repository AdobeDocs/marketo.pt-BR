---
unique-page-id: 2360253
description: Editar a mensagem "Exibir como página da Web" - Documentos do Marketo - Documentação do produto
title: Editar a mensagem "Exibir como página da Web"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 5%

---

# Editar a mensagem &quot;Exibir como página da Web&quot; {#edit-the-view-as-web-page-message}

Se precisar editar o texto &quot;[Exibir como uma página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;, veja como.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Editar a mensagem &quot;Exibir como página da Web&quot; {#edit-the-view-as-web-page-message-1}

1. Em **Admin**, clique em **Email**.

   ![](assets/image2014-9-18-17-3a13-3a2.png)

   >[!CAUTION]
   >
   >As variáveis a seguir são críticas. Não exclua!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >A segunda parte `##MKT_TOK##` é o cookie de maschkin dessa pessoa. Isso garante que eles fiquem com cookies adequadamente ao clicar no link.

1. Edite as versões **Exibir como página da Web HTML** e **Exibir como texto da página da Web** de acordo com sua preferência e clique em **Salvar alterações**.

   ![](assets/image2016-8-26-14-3a40-3a29.png)

>[!CAUTION]
>
>Certifique-se de evitar:
>
>* Adicionar URLs adicionais a uma das caixas HTML
>* Inserção de HTML na versão de texto


Aí está. Envie emails de teste para garantir a formatação.

## Texto padrão &quot;Exibir como página da Web&quot; {#default-view-as-web-page-text}

Se você precisar reverter para o sistema padrão &quot;Exibir como página da Web&quot;, copie/cole o seguinte:

**Exibir como HTML da página da Web:**

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**Exibir como texto da página da Web:**

Para exibir este email como uma página da Web, vá para o seguinte endereço:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>` Boom! Você terminou.
