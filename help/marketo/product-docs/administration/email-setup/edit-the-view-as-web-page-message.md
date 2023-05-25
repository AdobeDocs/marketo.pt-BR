---
unique-page-id: 2360253
description: Edite a mensagem "Exibir como página da Web" - Documentação do Marketo - Documentação do produto
title: Edite a mensagem "Exibir como página da Web"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
source-git-commit: 81ee349dbbe48c70b040751cae750c3684b71c78
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 5%

---

# Edite a mensagem &quot;Exibir como página da Web&quot; {#edit-the-view-as-web-page-message}

Se precisar editar o &quot;[Visualizar como página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;texto, veja como.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Edite a mensagem &quot;Exibir como página da Web&quot; {#edit-the-view-as-web-page-message-1}

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Clique em **[!UICONTROL E-mail]**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >As variáveis a seguir são críticas. Não os exclua!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >Quanto à segunda parte `##MKT_TOK##` é o [!UICONTROL munchkin] cookie dessa pessoa. Ele garante que sejam corretamente guiados ao clicar no link.

1. Edite o **[!UICONTROL Exibir como HTML da página da Web]** e **[!UICONTROL Exibir como texto da página da Web]** de acordo com sua preferência e clique em **[!UICONTROL Salvar alterações]**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Evite:
>
>* Adicionar URLs adicionais a qualquer uma das caixas HTML
>* Inserção do HTML na versão de texto


É isso aí. Envie emails de teste para garantir a formatação.

## Texto padrão &quot;Exibir como página da Web&quot; {#default-view-as-web-page-text}

Se você precisar reverter para o sistema padrão &quot;[!UICONTROL Exibir como página da Web]&quot;, copie/cole o seguinte:

**[!UICONTROL Exibir como HTML da página da Web]**:

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**[!UICONTROL Exibir como texto da página da Web]**:

Para exibir esse email como uma página da Web, vá para o seguinte endereço:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`

Pronto!
