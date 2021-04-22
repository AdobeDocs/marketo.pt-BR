---
unique-page-id: 30081815
description: Configuração da integração do Adobe Experience Manager - Documentos do Marketo - Documentação do produto
title: Configuração da integração do Adobe Experience Manager
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Configurar a integração do Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configure AEM para que você possa acessar, selecionar e importar ativos AEM no Marketo Design Studio.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!CAUTION]
>
>No momento, esse recurso é totalmente compatível com o Firefox. Ele não é compatível com o Safari e pode não funcionar na versão mais recente do Chrome (v. 80), dependendo das configurações de cookie do SameSite.

1. Navegue até a Adobe Experience Manager (o URL é específico para sua empresa).

   ![](assets/one.png)

1. Você pode fazer logon com o Adobe ou fazer logon localmente. Neste exemplo, entraremos localmente.

   ![](assets/two.png)

1. Em **Ferramentas**, clique em **Operações** e selecione **Console da Web**.

   ![](assets/2a.png)

1. No seu navegador, pesquise (ctrl+f no Windows, cmd+f no Mac) por &quot;Política de compartilhamento de recursos entre origens do Adobe Granite&quot;.

   ![](assets/three.png)

1. Clique no sinal **+** à direita.

   ![](assets/four.png)

1. Na caixa de texto **Origens permitidas (Regexp)**, digite `https://.*\.marketo\.com` e clique em **Salvar**.

   ![](assets/five-psd.png)

1. No cabeçalho na parte superior da página, clique em **Console da Web** e selecione **Informações do Sistema**.

   ![](assets/six.png)

1. Em Informações do servidor, clique no botão **Reiniciar**.

   ![](assets/seven.png)

1. Clique em **OK** para confirmar.

   ![](assets/eight.png)

1. No Marketo Classic, clique em **Admin**.

   ![](assets/nine.png)

1. Em Integração, selecione **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Clique em **Editar**.

   ![](assets/eleven.png)

1. Insira o URL do AEM e clique em **OK**.

   ![](assets/twelve.png)

   Está tudo pronto! Agora você pode [importar ativos AEM para o Design Studio no Marketo Sky](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/importing-assets-with-adobe-experience-manager.html?lang=en#design-studio).
