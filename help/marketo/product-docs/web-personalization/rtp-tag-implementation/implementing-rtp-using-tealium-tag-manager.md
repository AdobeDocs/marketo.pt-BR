---
unique-page-id: 9437340
description: Implementação do RTP usando o Tealium Tag Manager - Documentação do Marketo - Documentação do produto
title: Implementação do RTP usando o Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 1%

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
