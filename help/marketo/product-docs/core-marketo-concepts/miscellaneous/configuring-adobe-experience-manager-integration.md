---
unique-page-id: 30081815
description: Configuração da integração do Adobe Experience Manager - Documentos do Marketing - Documentação do produto
title: Configuração da integração Adobe Experience Manager
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Configuração da integração Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configure AEM para que você possa acessar, selecionar e importar ativos AEM no Design Studio do Marketo.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!CAUTION]
>
>Atualmente, esse recurso é totalmente compatível apenas com o Firefox. Ele não é suportado no Safari e pode não funcionar na versão mais recente do Chrome (v. 80), dependendo das configurações de cookie do SameSite.

1. Navegue até o Adobe Experience Manager (o URL é específico para a sua empresa).

   ![](assets/one.png)

1. Você pode fazer logon com Adobe ou fazer logon localmente. Neste exemplo, entraremos localmente.

   ![](assets/two.png)

1. Em **Ferramentas**, clique em **Operações** e selecione Console **da Web**.

   ![](assets/2a.png)

1. No seu navegador, procure &quot;Adobe Granite Cross-Origem Resource Sharing Policy&quot; (Política de compartilhamento de recursos entre  do) (ctrl+f no Windows, cmd+f no Mac).

   ![](assets/three.png)

1. Clique no **+** sinal à direita.

   ![](assets/four.png)

1. Na caixa de texto Origens **permitidas (Regexp)** , digite &quot;https://.*\.marketo\.com&quot; (sem as aspas) e clique em **Salvar**.

   ![](assets/five-psd.png)

1. No cabeçalho na parte superior da página, clique em Console **da** Web e selecione Informações **** do sistema.

   ![](assets/six.png)

1. Em Informações do servidor, clique no botão **Reiniciar** .

   ![](assets/seven.png)

1. Clique em **OK** para confirmar.

   ![](assets/eight.png)

1. No Marketo Classic, clique em **Admin**.

   ![](assets/nine.png)

1. Em Integração, selecione **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Clique em **Editar**.

   ![](assets/eleven.png)

1. Insira seu URL AEM e clique em **OK**.

   ![](assets/twelve.png)

   Vocês estão prontos! Agora você pode [importar ativos AEM para o Design Studio no Marketo Sky](http://help.marketo.com/hc/en-us/articles/360036765993).

