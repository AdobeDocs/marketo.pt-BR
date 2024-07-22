---
unique-page-id: 2360253
description: Edite a mensagem "Exibir como página da Web" - Documentação do Marketo - Documentação do produto
title: Edite a mensagem "Exibir como página da Web"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# Edite a mensagem &quot;Exibir como página da Web&quot; {#edit-the-view-as-web-page-message}

Se você precisar editar o texto &quot;[Exibir como uma página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;, veja como.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Edite a mensagem &quot;Exibir como página da Web&quot; {#edit-the-view-as-web-page-message-1}

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Clique em **[!UICONTROL Email]**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >As variáveis a seguir são críticas. Não os exclua!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >A segunda parte `##MKT_TOK##` é o cookie [!UICONTROL munchkin] dessa pessoa. Ele garante que sejam corretamente guiados ao clicar no link.

1. Edite as versões **[!UICONTROL Exibir como HTML da Página da Web]** e **[!UICONTROL Exibir como Texto da Página da Web]** de sua preferência e clique em **[!UICONTROL Salvar Alterações]**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Evite:
>
>* Adicionar URLs adicionais a qualquer uma das caixas HTML
>* Inserção do HTML na versão de texto

É isso aí. Envie emails de teste para garantir a formatação.

## Texto padrão &quot;Exibir como página da Web&quot; {#default-view-as-web-page-text}

Se você precisar reverter para o sistema padrão &quot;[!UICONTROL Exibir como Página da Web]&quot;, copie/cole o seguinte:

**[!UICONTROL Exibir como HTML da página da Web]**:

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**[!UICONTROL Exibir como texto da página da Web]**:

Para exibir esse email como uma página da Web, vá para o seguinte endereço:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`

Pronto!
