---
unique-page-id: 4720151
description: Saiba mais sobre a implementação de rtp nas páginas de aterrissagem do Marketo no Marketo Engage, incluindo a implementação de rtp no Marketo. Use este guia para concluir a próxima etapa.
title: Implementação do RTP em páginas de destino do Marketo
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
TQID: https://experienceleague.adobe.com/scyZfbFBloPu8JRfJiMjm62AFCHM7WCxaats3qssq2A
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 213
ht-degree: 5%

---

# Implementação do RTP em páginas de destino do Marketo {#implementing-rtp-on-marketo-landing-pages}

Para implementar sua [!UICONTROL tag RTP], siga as instruções de instalação abaixo:

1. Vá para o **[!UICONTROL Design Studio].** Abra o item que deseja editar. Selecione **[!UICONTROL Ações do modelo]**, selecione **[!UICONTROL Editar rascunho]**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Faça alterações no modelo na guia **HTML Source**.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Na sua conta RTP, vá para **[!UICONTROL Configurações da Conta]**.

   a) Se você já tiver recebido sua tag do JavaScript do suporte, continue para a etapa 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. Em [!UICONTROL Domínio], localize o domínio relevante e clique em **[!UICONTROL Gerar Marca]**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copie a marca RTP JavaScript e cole-a em todos os modelos de página de aterrissagem entre as marcas **`<head> </head>`**.

1. Clique em **[!UICONTROL Salvar]** e **[!UICONTROL Fechar]** a janela.

1. De volta ao **[!UICONTROL Design Studio]**, aprove a página de aterrissagem de **[!UICONTROL Ações de Modelo]**, clique em **[!UICONTROL Aprovar]**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Finalmente, você precisará **reaprovar** qualquer landing page que use esse template para que as alterações do template entrem em vigor. Você pode aprová-las novamente de uma só vez na seção principal de [!UICONTROL Páginas de Aterrissagem].

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Verifique se ele aparece em todas as páginas, incluindo páginas de aterrissagem e subdomínios.

   Você pode fazer isso clicando com o botão direito do mouse na página do site. Ir para **[!UICONTROL Exibir Página Source].** Procure por **[!UICONTROL RTP]** para localizar a marca.
