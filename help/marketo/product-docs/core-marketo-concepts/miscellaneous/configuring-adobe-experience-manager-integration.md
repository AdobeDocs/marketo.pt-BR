---
unique-page-id: 30081815
description: Configuração da integração do Adobe Experience Manager - Documentação do Marketo - Documentação do produto
title: Configuração da integração do Adobe Experience Manager
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
source-git-commit: 0abb315be0f9cb5f42fa41d72b446de8c2f62c1e
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Configuração da integração do Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configure o Adobe Experience Manager (AEM) para poder acessar, selecionar e importar ativos do AEM no Marketo Engage Design Studio.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!IMPORTANT]
>
>* Essa integração só funciona com implementações locais do AEM e não é compatível com implementações do AEM Cloud Service.
>
>* Atualmente, esse recurso é totalmente compatível apenas com o Firefox. Ele não é compatível com o Safari e pode não funcionar na versão mais recente do Chrome, dependendo das configurações de cookie SameSite.

1. Navegue até a Adobe Experience Manager (o URL é específico da sua empresa).

   ![](assets/one.png)

1. Você pode fazer logon com o Adobe ou localmente. Neste exemplo, faremos logon localmente.

   ![](assets/two.png)

1. Em **[!UICONTROL Ferramentas]**, clique em **[!UICONTROL Operações]** e selecione **[!UICONTROL Console da Web]**.

   ![](assets/2a.png)

1. Em seu navegador, pesquise (ctrl+f no Windows, cmd+f no Mac) por &quot;Política de compartilhamento de recursos entre origens do Adobe Granite&quot;.

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

1. Clique em **[!UICONTROL Editar]**.

   ![](assets/eleven.png)

1. Insira a URL do AEM e clique em **[!UICONTROL OK]**.

   ![](assets/twelve.png)
