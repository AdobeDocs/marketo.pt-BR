---
unique-page-id: 2360253
description: Personalize o texto do link Exibir como página da Web e o HTML no email do administrador, mantendo as variáveis necessárias intactas.
title: Edite a mensagem "Exibir como página da Web"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
TQID: https://experienceleague.adobe.com/mREJHheKv7c16atJ17pv8S9ZGUoLnD8jd5jyk6QtgR8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 182
ht-degree: 0%

---

# Edite a mensagem &quot;Exibir como página da Web&quot; {#edit-the-view-as-web-page-message}

Saiba como editar o texto &quot;[Exibir como página da Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;.

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
   >A segunda parte `##MKT_TOK##` é o cookie [!UICONTROL Munchkin] dessa pessoa. Isso garante que eles sejam rastreados adequadamente ao clicar no link.

1. Edite as versões **[!UICONTROL Exibir como HTML da Página da Web]** e **[!UICONTROL Exibir como Texto da Página da Web]** de sua preferência e clique em **[!UICONTROL Salvar Alterações]**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Evite:
>
>* Adicionar URLs adicionais a qualquer uma das caixas do HTML
>* Inserção do HTML na versão de texto

Envie emails de teste para verificar a formatação.

## Texto padrão &quot;Exibir como página da Web&quot; {#default-view-as-web-page-text}

Se você precisar reverter para o sistema padrão &quot;[!UICONTROL Exibir como Página da Web]&quot;, copie/cole o seguinte:

**[!UICONTROL Exibir como HTML da Página da Web]**:

`<div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div>`

**[!UICONTROL Exibir como texto da página da Web]**:

Para exibir esse email como uma página da Web, vá para o seguinte endereço:
`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
