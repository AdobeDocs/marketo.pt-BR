---
unique-page-id: 30081815
description: Configuração da integração do Adobe Experience Manager - Documentos do Marketo - Documentação do produto
title: Configuração da integração do Adobe Experience Manager
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
source-git-commit: 2a94e4b3b034eac821a82a84db65c09e503c52f4
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Configuração da integração do Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configure o Adobe Experience Manager (AEM) para que você possa acessar, selecionar e importar AEM ativos no Marketo Engage Design Studio.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!IMPORTANT]
>
>* Essa integração só funciona com implementações locais de AEM e não é compatível com implementações do AEM Cloud Service.
>
>* No momento, esse recurso é totalmente compatível com o Firefox. Ele não é compatível com o Safari e pode não funcionar na versão mais recente do Chrome, dependendo das configurações de cookie do SameSite.


1. Navegue até a Adobe Experience Manager (o URL é específico para sua empresa).

   ![](assets/one.png)

1. Você pode fazer logon com o Adobe ou fazer logon localmente. Neste exemplo, entraremos localmente.

   ![](assets/two.png)

1. Em **Ferramentas**, clique em **Operações** e selecione **Console da Web**.

   ![](assets/2a.png)

1. No seu navegador, pesquise (ctrl+f no Windows, cmd+f no Mac) por &quot;Política de compartilhamento de recursos entre origens do Adobe Granite&quot;.

   ![](assets/three.png)

1. Clique no botão **+** assine à direita.

   ![](assets/four.png)

1. No **Origens Permitidas (Regexp)** caixa de texto, digite `https://.*\.marketo\.com` e clique em **Salvar**.

   ![](assets/five-psd.png)

1. No cabeçalho na parte superior da página, clique em **Console da Web** e selecione **Informações do sistema**.

   ![](assets/six.png)

1. Em Informações do servidor, clique no botão **Reiniciar** botão.

   ![](assets/seven.png)

1. Clique em **OK** para confirmar.

   ![](assets/eight.png)

1. No Marketo Engage, clique em **Administrador**.

   ![](assets/nine.png)

1. Em Integração, selecione **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Clique em **Editar**.

   ![](assets/eleven.png)

1. Insira o URL do AEM e clique em **OK**.

   ![](assets/twelve.png)
