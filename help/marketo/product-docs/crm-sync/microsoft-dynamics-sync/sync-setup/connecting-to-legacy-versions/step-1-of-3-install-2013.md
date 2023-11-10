---
unique-page-id: 3571813
description: Etapa 1 de 3 - Instalar a solução da Marketo no Dynamics (2013 no local) - Documentação da Marketo - Documentação do produto
title: Etapa 1 de 3 - Instalar a solução da Marketo no Dynamics (2013 no local)
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Etapa 1 de 3: instalar a solução da Marketo no Dynamics (2013 no local) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Antes de sincronizar o Microsoft Dynamics no local e o Marketo Engage, é necessário instalar a solução Marketo no Dynamics.

>[!NOTE]
>
>Após sincronizar o Marketo com um CRM, não é possível executar uma nova sincronização sem substituir a instância.

>[!PREREQUISITES]
>
>Você deve ter [Implantação voltada para a Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) with [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0, 2.1 ou 3.0 (ADFS) configurado. Observação: o documento IFD é baixado automaticamente quando você clica no link.
>
>[Baixar a solução da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} antes de começar.

>[!NOTE]
>
>**Permissões de administrador do Dynamics necessárias**.
>
>Você precisa de privilégios de administrador do CRM para executar esta sincronização.

1. Faça logon no Dynamics. Clique em **[!UICONTROL Microsoft Dynamics CRM]** e selecione **[!UICONTROL Configurações]**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. Em **[!UICONTROL Configurações]**, selecione **[!UICONTROL Soluções]**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Clique em **[!UICONTROL Importar]**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Clique em **[!UICONTROL Procurar]** e selecione o [solução baixada](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Clique em **[!UICONTROL Próximo]**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Exiba as Informações da Solução e clique em **[!UICONTROL Exibir detalhes do pacote de soluções]**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Quando terminar de verificar todos os detalhes, clique em **[!UICONTROL Fechar]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Na página Informações da solução, clique em **[!UICONTROL Próxima]**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Verifique se a opção SDK está marcada. Clique em **[!UICONTROL Importar]**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Aguarde a conclusão da importação.

   >[!TIP]
   >
   >Você precisará ativar os pop-ups no seu navegador para concluir o processo de instalação.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Baixe um arquivo de log (se desejar) e clique em **[!UICONTROL Fechar]**.

   >[!NOTE]
   >
   >Você pode ver uma mensagem dizendo &quot;O Gerenciamento de clientes potenciais da Marketo foi concluído com aviso&quot;. Isso é totalmente esperado.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. O Gerenciamento de clientes potenciais da Marketo agora aparecerá no **[!UICONTROL Todas as soluções]** página.

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Selecione a solução da Marketo e clique em **[!UICONTROL Publicar todas as personalizações]**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

>[!CAUTION]
>
>Desativar qualquer um dos processos de mensagens do SDK do Marketo resultará em uma instalação corrompida!

>[!MORELIKETHIS]
>
>[Etapa 2 de 3: Configurar usuário de sincronização para o Marketo (2013 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md){target="_blank"}
