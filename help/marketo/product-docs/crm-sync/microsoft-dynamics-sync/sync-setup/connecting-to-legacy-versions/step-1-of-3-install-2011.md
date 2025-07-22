---
unique-page-id: 3571805
description: Etapa 1 de 3 - Instalar a solução da Marketo (2011 no local) - Documentação da Marketo - Documentação do produto
title: Etapa 1 de 3 - Instalar a solução da Marketo (2011 no local)
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Etapa 1 de 3: instalar a solução da Marketo (2011 no local) {#step-of-install-the-marketo-solution-on-premises}

Antes de sincronizar o [!DNL Microsoft Dynamics] no local e o Marketo, é necessário instalar a solução da Marketo no [!DNL Dynamics].

>[!NOTE]
>
>Após sincronizar o Marketo com um CRM, não é possível executar uma nova sincronização sem substituir a instância.

>[!PREREQUISITES]
>
>Você deve ter a [Implantação para a Internet](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/deploy/configure-an-internet-facing-deployment){target="_blank"} (IFD) com os [Serviços de Federação do Ative Diretory](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0, 2.1 ou 3.0 (ADFS) configurados. **Observação**: o documento IFD é baixado automaticamente quando você clica no link.
>
>[Baixe a Solução de Gerenciamento de Clientes Potenciais da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} antes de começar.

>[!NOTE]
>
>**[!DNL Dynamics]Permissões de Administrador necessárias.**
>
>Você precisa de privilégios de administrador do CRM para executar esta sincronização.

1. Faça logon em **[!DNL Dynamics]**, selecione **[!UICONTROL Configurações]** no menu inferior esquerdo.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Selecione **[!UICONTROL Soluções]** na árvore.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Clique em **[!UICONTROL Importar]**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Clique em **[!UICONTROL Procurar]**. Selecione a solução de gerenciamento de clientes potenciais da Marketo que você [baixou](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clique em **[!UICONTROL Avançar]**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Exiba as Informações da Solução e clique em **[!UICONTROL Exibir detalhes do pacote da solução]**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Quando terminar de verificar todos os detalhes, clique em **[!UICONTROL Fechar]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Na página Informações da solução, clique em **[!UICONTROL Avançar]**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Verifique se a caixa de seleção da opção de mensagem do SDK está marcada. Clique em **[!UICONTROL Avançar]**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Você precisará ativar os pop-ups no seu navegador para concluir o processo de instalação.

1. Agora aguarde a conclusão da importação. Levante-se e faça alguns alongamentos.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Clique em **[!UICONTROL Fechar]**.

   >[!NOTE]
   >
   >Você pode ver uma mensagem dizendo &quot;O Gerenciamento de clientes potenciais da Marketo foi concluído com aviso&quot;. Isso é totalmente esperado.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. O [!UICONTROL Marketo Lead Management] agora aparecerá na página **[!UICONTROL Todas as Soluções]**.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Selecione [!UICONTROL Marketo Lead Management] e clique em **[!UICONTROL Publicar todas as personalizações]**.

   ![](assets/image2015-4-2-11-3a48-3a21.png)

>[!CAUTION]
>
>Desativar qualquer um dos processos de mensagens do Marketo SDK resultará em uma instalação corrompida!

>[!MORELIKETHIS]
>
>[Etapa 2 de 3: Configurar o Usuário de Sincronização do Marketo em [!DNL Dynamics] (2011 no Local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md)
