---
unique-page-id: 4720145
description: Saiba mais sobre como implementar o rtp usando o google tag manager na Marketo Engage, incluindo como implementar o rtp usando dnl do google. Use este guia para concluir a próxima etapa.
title: Implementação do RTP usando o gerenciador de tags do Google
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
TQID: https://experienceleague.adobe.com/XesXGBf2aDsnsbS2Ro1RLdd1EVrj-mBdCiv8C0dj8NU
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 173
ht-degree: 3%

---

# Implementando RTP usando [!DNL Google Tag Manager] {#implementing-rtp-using-google-tag-manager}

Para implementar sua tag RTP, siga as instruções de instalação abaixo.

1. Faça logon em sua conta do [!DNL Google Tag Manager].

1. Adicionar uma nova **[!UICONTROL Marca]** > **[!UICONTROL Configurações de Marca]** > **[!UICONTROL Marca Personalizada do HTML].** Chame de **RTP**.

1. Faça logon em sua **conta RTP**.

1. Vá para **[!UICONTROL Configurações da conta]**.

   a) Se você já recebeu a tag do JavaScript do suporte, continue para a Etapa 6.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. Em [!UICONTROL Domínio], localize o domínio relevante e clique em **[!UICONTROL Gerar Marca]**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Copie a tag RTP JavaScript e cole-a na nova **Tag personalizada de HTML** que você criou (Etapa 1).

1. Clique em **[!UICONTROL Adicionar regra para acionar a marca]**. Selecione **[!UICONTROL Todas as páginas]**.

1. Clique em **[!UICONTROL Salvar]** e [publicar a nova versão](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Verifique se ele aparece em todas as páginas, incluindo páginas de aterrissagem e subdomínios.

   a) Você pode fazer isso clicando com o botão direito do mouse na página do seu site. Vá para **[!UICONTROL Inspecionar Elemento]**, Pesquisar por **RTP** para localizar a marca.
