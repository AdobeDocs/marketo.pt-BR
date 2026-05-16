---
unique-page-id: 11385053
description: Saiba como gerar e colocar a tag RTP Web Personalization para Conteúdo preditivo. Copie-o no cabeçalho da página, verifique a cobertura e confirme se o botão permanece ativado.
title: Implantar o JavaScript para IA de conteúdo
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
TQID: https://experienceleague.adobe.com/LHzl0KuIoJvZ99eFWGFE6RdDW1xRxBS4LG3XU9ujj4U
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 162
ht-degree: 0%

---

# Implantar o JavaScript para IA de conteúdo {#deploy-the-javascript-for-content-ai}

Para usar o Predictive Content, você precisa gerar e configurar a tag RTP (Web Personalization).

## Gerar tag {#generate-tag}

1. Faça logon na sua conta de conteúdo preditivo. Vá para **[!UICONTROL Configurações da conta]**.

   ![](assets/settings-dropdown-account-hands.png)

1. Em **[!UICONTROL Configuração de Domínio]**, localize o domínio relevante e clique em **[!UICONTROL Gerar Marca]**.

   ![](assets/generate-tag.png)

1. Copie e cole a tag do Web Personalization na HTML do site.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copie a marca JavaScript do Web Personalization e cole-a como o primeiro script no cabeçalho de suas páginas, entre as marcas `<head> </head>`. Veja mais [instruções de implementação detalhadas aqui](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Verifique se a tag é exibida em todas as páginas, incluindo páginas de aterrissagem e subdomínios. Verifique isso clicando com o botão direito do mouse na página do site. Vá para **[!UICONTROL Exibir Página Source]** em um navegador da Web. Pesquisa: &quot;RTP&quot;.

1. Confirme se o botão de alternância de Marca está definido como **[!UICONTROL ON]**.
