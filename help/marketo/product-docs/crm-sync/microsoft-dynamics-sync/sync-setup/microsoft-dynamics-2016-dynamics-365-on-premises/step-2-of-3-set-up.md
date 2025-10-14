---
description: Instalar o Marketo para  [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 No Local Etapa 2 de 3 - Documentação do Marketo - Documentação do Produto
title: Instalar o Marketo para  [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 No Local Etapa 2 de 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

# Etapa 2 de 3 Configurar Marketo para [!DNL Dynamics] (2016 No Local/[!DNL Dynamics] 365 No Local){#step-of-set-up-for-marketo-on-premises-2016}

Ótimo trabalho para concluir as etapas anteriores. Vamos continuar passando por isso.

>[!PREREQUISITES]
>
>[Instalar Marketo para [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 No Local Etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## Criar um novo usuário {#create-a-new-user}

1. Faça logon em [!DNL Dynamics]. Clique no ícone Configurações e selecione Configurações avançadas.

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. Clique em **[!UICONTROL Configurações]** e selecione **[!UICONTROL Segurança]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. Clique em **[!UICONTROL Usuários]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. Clique em **[!UICONTROL Novo]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. Clique em **[!UICONTROL Adicionar e licenciar usuários]**. Uma nova guia deve ser aberta.

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. Clique em **[!UICONTROL Administrador]** na parte superior da página. Outra nova guia deve ser aberta.

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. Clique em **[!UICONTROL Adicionar um usuário]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. Insira todas as suas informações. Quando terminar, clique em **[!UICONTROL Adicionar]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >Esse nome deve ser um usuário de sincronização dedicado e não uma conta existente de usuário do CRM. Não precisa ser um endereço de email real.

1. Insira o email para receber as novas credenciais de usuário, clique em Enviar email e fechar.

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## Criar um Novo Aplicativo Cliente {#create-a-new-client-application}

Siga as etapas em [este artigo do Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later) para criar um novo Aplicativo Cliente e conceder permissões. Anote a ID/Segredo do Cliente do aplicativo cliente [!DNL Dynamics].

## Atribuir Função de Usuário de Sincronização {#assign-sync-user-role}

Atribua a função de Usuário de sincronização do Marketo somente ao usuário de sincronização do Marketo. Você não precisa atribuí-lo a nenhum outro usuário.

>[!NOTE]
>
>Isso se aplica à versão 4.0.0.14 e posterior do Marketo. Para versões anteriores, todos os usuários devem ter a função de usuário sincronizar. Para atualizar sua Marketo, consulte [Atualizar a Solução da Marketo para [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>A configuração de idioma do Usuário de Sincronização [&#x200B; deve ser definida como Inglês](https://learn.microsoft.com/en-us/power-platform/admin/enable-languages){target="_blank"}.

1. Em **[!UICONTROL Configurações]**, clique em **[!UICONTROL Segurança]**.

   ![](assets/assign1.png)

1. Clique em **[!UICONTROL Usuários]**.

   ![](assets/assign2.png)

1. Você verá uma lista de usuários aqui. Selecione o usuário dedicado do Marketo Sync ou contate o administrador do [Ative Diretory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} (ADFS) para criar um usuário dedicado para o Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Selecione o usuário de sincronização. Clique em **[!UICONTROL Gerenciar Funções]**.

   ![](assets/assign4.png)

1. Verifique o usuário de sincronização do Marketo e clique em **[!UICONTROL OK]**.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Se você não vir a função, volte para a [etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) e importe a solução.

   >[!NOTE]
   >
   >Quaisquer atualizações feitas em seu CRM pelo Usuário da Sincronização _não_ serão sincronizadas com o Marketo novamente.

## Configurar a solução da Marketo {#configure-marketo-solution}

Quase pronto! Temos apenas algumas últimas configurações antes de passar para o próximo artigo.

1. Em **[!UICONTROL Configurações]**, clique em **[!UICONTROL Configuração do Marketo]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Se a Configuração do Marketo estiver ausente, tente atualizar a página. Se o problema persistir, [publique a Solução da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"} ou tente fazer logoff e logon novamente.

1. Clique em **[!UICONTROL Padrão]**.

   ![](assets/configure2.png)

1. Clique no campo **[!UICONTROL Usuário do Marketo]** e selecione o usuário de sincronização.

   ![](assets/configure3.png)

1. Clique no ícone de salvar no canto inferior direito.

   ![](assets/configure4.png)

1. Clique em **[!UICONTROL Publicar todas as personalizações]**.

   ![](assets/publish-all-customizations1.png)

## Antes de prosseguir para a Etapa 3 {#before-proceeding-to-step}

* Se quiser restringir o número de registros sincronizados, [configure um filtro de sincronização personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) agora.
* Execute o processo [Validate [!DNL Microsoft Dynamics] Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Ele verifica se as configurações iniciais foram feitas corretamente.
* Faça logon no Usuário de Sincronização do Marketo no [!DNL Microsoft Dynamics] CRM.

>[!MORELIKETHIS]
>
>[Instalar Marketo para [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 No Local Etapa 3 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
