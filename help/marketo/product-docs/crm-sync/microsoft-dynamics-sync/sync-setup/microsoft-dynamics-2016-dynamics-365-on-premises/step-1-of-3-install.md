---
description: Instalar o Marketo para Microsoft Dynamics 2016/Dynamics 365 no local 1 de 3 - Documentação do Marketo - Documentação do produto
title: Instalar o Marketo para Microsoft Dynamics 2016/Dynamics 365 no Local Etapa 1 de 3
exl-id: 0a494ae7-87da-4ff9-bb47-990b957533e1
feature: Microsoft Dynamics
source-git-commit: 15cb3ddcd82fa1ba60fae3aa1adaac3d5964a0fa
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Etapa 1 de 3: Configurar usuário de sincronização para o Marketo (2016 No local /Dynamics 365 No local) {#step-of-configure-sync-user-for-marketo-on-premises-2016}

Antes de sincronizar o Microsoft Dynamics 2016 no local/Dynamics 365 com o Marketo Engage, primeiro é necessário instalar a solução Marketo no Dynamics.

>[!NOTE]
>
>Depois de sincronizar o Marketo com um CRM, você não pode sincronizar um novo CRM com a instância existente do Marketo.

>[!PREREQUISITES]
>
>Se você estiver usando o Microsoft Dynamics No Local, deve ter o [Implantação para a Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) com os [Serviços de Federação do Ative Diretory](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0+ (ADFS) configurado. Observação: o documento IFD é baixado automaticamente quando você clica no link.
>
>[Baixe a Solução de Gerenciamento de Clientes Potenciais da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} antes de começar.

>[!NOTE]
>
>**Permissões de Administrador do Dynamics necessárias**.
>
>Você precisa de privilégios de administrador do CRM para executar esta sincronização.

1. Faça logon no Dynamics. Clique no menu suspenso **[!UICONTROL Microsoft Dynamics CRM]** e selecione **[!UICONTROL Configurações]**.

   ![](assets/image2015-3-19-8-33-29.png)

1. Em **[!UICONTROL Configurações]**, selecione **[!UICONTROL Soluções]**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Clique em **[!UICONTROL Importar]**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Clique em **[!UICONTROL Procurar]** e selecione a solução que você [baixou](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Clique em **Avançar**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Exiba as Informações da Solução e clique em **[!UICONTROL Exibir detalhes do pacote da solução]**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Quando terminar de verificar todos os detalhes, clique em **[!UICONTROL Fechar]**.

   ![](assets/step6.png)

1. Na página Informações da solução, clique em **[!UICONTROL Avançar]**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Verifique se a caixa de seleção da opção SDK está marcada. Clique em **[!UICONTROL Importar]**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Aguarde a conclusão da importação.

   >[!TIP]
   >
   >Você precisará ativar os pop-ups no seu navegador para concluir o processo de instalação.

   ![](assets/image2015-3-11-11-34-9.png)

1. Baixe um arquivo de log (se desejar) e clique em **[!UICONTROL Fechar]**.

   >[!NOTE]
   >
   >Você pode ver uma mensagem dizendo &quot;O Gerenciamento de clientes potenciais da Marketo foi concluído com aviso&quot;. Isso é totalmente esperado.

   ![](assets/image2015-3-13-9-54-39.png)

1. O Gerenciamento de Clientes Potenciais da Marketo agora aparecerá na página **[!UICONTROL Todas as Soluções]**.

   ![](assets/image2015-3-19-8-40-38.png)

1. Selecione a solução da Marketo e clique em **[!UICONTROL Todas as personalizações do Publish]**.

   ![](assets/image2015-3-19-8-41-21.png)

   Toque cinco! A instalação foi concluída.

   >[!CAUTION]
   >
   >Desativar qualquer um dos processos de mensagens do SDK do Marketo resultará em uma instalação corrompida!

   >[!MORELIKETHIS]
   >
   >[Instalar o Marketo para Dynamics 2015 no Local e 2016 365 no Local Etapa 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md){target="_blank"}
