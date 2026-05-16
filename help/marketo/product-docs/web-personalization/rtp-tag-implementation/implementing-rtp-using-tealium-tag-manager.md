---
unique-page-id: 9437340
description: Saiba mais sobre como implementar o rtp usando o gerenciador de tags do télio no Marketo Engage, incluindo como implementar o rtp usando dnl. Use este guia para concluir a próxima etapa.
title: Implementação do RTP usando o gerenciador de tags do Tealium
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
TQID: https://experienceleague.adobe.com/zMs2Dii5RERdH8tKb86a6EhxXUx2IpbZkDOCklUvvY4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 233
ht-degree: 3%

---

# Implementando o RTP usando o [!DNL Tealium] Tag Manager {#implementing-rtp-using-tealium-tag-manager}

Para implementar sua tag RTP, siga as instruções de instalação abaixo.

1. Faça logon em sua conta do [!DNL Tealium] Tag Manager.

1. Navegue até a guia [!UICONTROL Marcas] e adicione a [!UICONTROL Marca de Contêiner Personalizado de Tealium], localizada na guia [!UICONTROL Misc] do marketplace de Marcas.

1. No campo [!UICONTROL Título], digite **Marketo RTP** e clique em **[!UICONTROL Concluir]**.

1. Salve as alterações.

   >[!NOTE]
   >
   >Não há necessidade de publicar o novo contêiner ainda.

1. Depois que o perfil for salvo, clique em seu nome/endereço de email no canto superior direito do console iQ do Tealium.

1. No menu [!UICONTROL Administrador], clique em **[!UICONTROL Gerenciar modelos]** em [!UICONTROL Administrador da conta].

1. Selecione **[!UICONTROL Contêiner Personalizado de Tealium]: Marketo RTP** na lista suspensa para abrir o Modelo de Marca.

1. Efetue login em sua conta RTP.

1. Vá para [!UICONTROL Configurações da conta].

   >[!NOTE]
   >
   >Se você já recebeu a tag do JavaScript do suporte, continue para a Etapa 11.

1. Em Domínio, localize o domínio relevante e clique em **[!UICONTROL Gerar Marca]**.

1. Copie a marca RTP JavaScript e cole-a entre [!UICONTROL Iniciar código da biblioteca de marcas] e [!UICONTROL Finalizar código da biblioteca de marcas] no seu modelo de perfil do Tálium.

   >[!NOTE]
   >
   >**Etapas importantes**
   >
   >Remova as marcas `<!-- RTP tag -->` e `<!-- End of RTP tag -->` do código que você insere neste arquivo.
   >
   >Remova qualquer marca de `<script type='text/javascript'>` e `</script>` do código que você colocar neste arquivo.

1. Clique em **[!UICONTROL Salvar modelo de perfil]** e publique seu novo perfil.
