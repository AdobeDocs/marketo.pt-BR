---
unique-page-id: 30081815
description: Configuração da integração do Adobe Experience Manager - Documentação do Marketo - Documentação do produto
title: Configuração da integração do Adobe Experience Manager
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
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
>* Atualmente, esse recurso é totalmente compatível apenas com o Firefox. Ele não é compatível com o Safari e pode não funcionar na versão mais recente do Chrome, dependendo das configurações de cookie do SameSite.

1. Navegue até a Adobe Experience Manager (o URL é específico da sua empresa).

   ![](assets/one.png)

1. Você pode fazer logon com o Adobe ou localmente. Neste exemplo, faremos logon localmente.

   ![](assets/two.png)

1. Entrada **Ferramentas**, clique em **Operações** e selecione **Console da Web**.

   ![](assets/2a.png)

1. Em seu navegador, pesquise (ctrl+f no Windows, cmd+f no Mac) por &quot;Política de compartilhamento de recursos entre origens do Adobe Granite&quot;.

   ![](assets/three.png)

1. Clique em **+** assine à direita.

   ![](assets/four.png)

1. No **Origens permitidas (Regexp)** caixa de texto, digite `https://.*\.marketo\.com` e clique em **Salvar**.

   ![](assets/five-psd.png)

1. No cabeçalho na parte superior da página, clique em **Console da Web** e selecione **Informações do sistema**.

   ![](assets/six.png)

1. Em Informações do servidor, clique na guia **Restart** botão.

   ![](assets/seven.png)

1. Clique em **OK** para confirmar.

   ![](assets/eight.png)

1. No Marketo Engage, clique em **Admin**.

   ![](assets/nine.png)

1. Em Integração, selecione **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Clique em **Editar**.

   ![](assets/eleven.png)

1. Insira o URL do AEM e clique em **OK**.

   ![](assets/twelve.png)
