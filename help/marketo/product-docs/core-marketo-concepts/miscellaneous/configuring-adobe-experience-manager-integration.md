---
unique-page-id: 30081815
description: Saiba como configurar a integração do Adobe Experience Manager com o Marketo. Configure o AEM para poder acessar e importar ativos para o Design Studio.
title: Configuração da integração ao Adobe Experience Manager
hide: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
TQID: https://experienceleague.adobe.com/nJBydVi8mRwVf1vAIFuI1S3nEuX0FGiztp8fhRHq6RM
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e2290edd-b061-4880-9d79-dee306cf5aa9
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 229
ht-degree: 8%

---

# Configuração da integração ao Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configure o Adobe Experience Manager (AEM) para poder acessar, selecionar e importar ativos do AEM para o Marketo Engage Design Studio.

>[!NOTE]
>
>**Permissões de administrador são necessárias**

>[!IMPORTANT]
>
>* Essa integração funciona somente com implementações no local do AEM e não é compatível com implementações do AEM Cloud Service.
>
>* Atualmente, esse recurso é totalmente compatível apenas com o Firefox. Ele não é compatível com o Safari e pode não funcionar na versão mais recente do Chrome, dependendo das configurações de cookie SameSite.

1. Navegue até a Adobe Experience Manager (o URL é específico da sua empresa).

   ![](assets/one.png)

1. Você pode fazer logon com a Adobe ou localmente. Este exemplo usa logon local.

   ![](assets/two.png)

1. Em **[!UICONTROL Ferramentas]**, clique em **[!UICONTROL Operações]** e selecione **[!UICONTROL Console da Web]**.

   ![](assets/2a.png)

1. Em seu navegador, pesquise (ctrl+f no Windows, cmd+f no Mac) por &quot;[!UICONTROL Política de Compartilhamento de Recursos entre Origens do Adobe Granite].&quot;

   ![](assets/three.png)

1. Clique no sinal **+** à direita.

   ![](assets/four.png)

1. Na caixa de texto **[!UICONTROL Origens permitidas (Regexp)]**, digite `https://.*\.marketo\.com` e clique em **[!UICONTROL Salvar]**.

   ![](assets/five-psd.png)

1. No cabeçalho na parte superior da página, clique em **[!UICONTROL Console da Web]** e selecione **[!UICONTROL Informações do Sistema]**.

   ![](assets/six.png)

1. Em Informações do Servidor, clique no botão **[!UICONTROL Reiniciar]**.

   ![](assets/seven.png)

1. Clique em **[!UICONTROL OK]** para confirmar.

   ![](assets/eight.png)

1. No Marketo Engage, clique em **[!UICONTROL Admin]**.

   ![](assets/nine.png)

1. Em Integração, selecione **[!UICONTROL Adobe Experience Manager]**.

   ![](assets/ten.png)

1. Clique em **[!UICONTROL Editar]**.

   ![](assets/eleven.png)

1. Insira sua URL do AEM e clique em **[!UICONTROL OK]**.

   ![](assets/twelve.png)
