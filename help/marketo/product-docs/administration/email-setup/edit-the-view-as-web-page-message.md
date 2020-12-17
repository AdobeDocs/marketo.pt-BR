---
unique-page-id: 2360253
description: Editar a mensagem "Visualização como página da Web" - Documentos do Marketing - Documentação do produto
title: Editar a mensagem "Visualização como página da Web"
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Editar a mensagem &quot;Visualização como página da Web&quot; {#edit-the-view-as-web-page-message}

Se precisar editar a Visualização &quot; [como uma página da Web](../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;, veja como.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Editar a mensagem &quot;Visualização como página da Web&quot; {#edit-the-view-as-web-page-message-1}

1. Em **Admin**, clique em **Email**.

   ![](assets/image2014-9-18-17-3a13-3a2.png)

   >[!CAUTION]
   >
   >As variáveis a seguir são críticas. Não os apague!
   >
   >    
   >    
   >    * %mkt_webview_url%?mkt_tok=##MKT_TOK#
   >    
   >    
   >A segunda parte ##MKT_TOK## é o cookie de maschkin daquela pessoa. Certifique-se de que eles recebem cookies apropriadamente quando clicam no link.

1. Edite a **Visualização como HTML** e **Visualização como Texto da página da Web **versões de seu gosto e clique em **Salvar alterações**.

   ![](assets/image2016-8-26-14-3a40-3a29.png)

>[!CAUTION]
>
>Evite:
>
>* Adicionar URLs adicionais a qualquer uma das caixas HTML
>* Inserir HTML na versão de texto

>



Aí está. Envie emails de teste para garantir a formatação.

## Texto padrão &quot;Visualização como página da Web&quot; {#default-view-as-web-page-text}

Se precisar reverter para o sistema padrão &quot;Visualização como página da Web&quot;, copie/cole o seguinte:

**Visualização como HTML da página da Web:**
`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>` **Visualização como Texto da página da Web:**

Para visualização deste email como uma página da Web, vá para o seguinte endereço:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>` Boom! Você terminou.
