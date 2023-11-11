---
description: Instalar o Marketo para Microsoft Dynamics 2016/Dynamics 365 no local Etapa 2 de 3 - Documentação do Marketo - Documentação do produto
title: Instalar o Marketo para Microsoft Dynamics 2016/Dynamics 365 no Local Etapa 2 de 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
feature: Microsoft Dynamics
source-git-commit: 15cb3ddcd82fa1ba60fae3aa1adaac3d5964a0fa
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Etapa 2 de 3 Configurar o Marketo para Dynamics (2016 no local/Dynamics 365 no local){#step-of-set-up-for-marketo-on-premises-2016}

Ótimo trabalho para concluir as etapas anteriores. Vamos continuar passando por isso.

>[!PREREQUISITES]
>
>[Instalar o Marketo para Microsoft Dynamics 2016/Dynamics 365 no Local Etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"}

## Criar um novo usuário {#create-a-new-user}

1. Faça logon no Dynamics. Clique no ícone Configurações e selecione Configurações avançadas.

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. Clique em **[!UICONTROL Configurações]** e selecione **[!UICONTROL Segurança]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. Clique em **[!UICONTROL Usuários]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. Clique em **[!UICONTROL Novo]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. Clique em **[!UICONTROL Adicionar e licenciar usuários]**. Uma nova guia deve ser aberta.

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. Clique em **[!UICONTROL Admin]** na parte superior da página. Outra nova guia deve ser aberta.

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

Siga as etapas em [este artigo do Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later){target="_blank"} para criar um novo Aplicativo Cliente e conceder permissões. Anote a ID/segredo do cliente do aplicativo cliente Dynamics.

## Atribuir Função de Usuário de Sincronização {#assign-sync-user-role}

Atribua a função de Usuário de sincronização do Marketo somente ao usuário de sincronização do Marketo. Você não precisa atribuí-lo a nenhum outro usuário.

>[!NOTE]
>
>Isso se aplica à versão 4.0.0.14 e posterior do Marketo. Para versões anteriores, todos os usuários devem ter a função de usuário sincronizar. Para atualizar o Marketo, consulte [Atualizar a solução Marketo para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>A configuração de idioma do Usuário de sincronização [deve ser definido como inglês](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. Em **[!UICONTROL Configurações]**, clique em **[!UICONTROL Segurança]**.

   ![](assets/assign1.png)

1. Clique em **[!UICONTROL Usuários]**.

   ![](assets/assign2.png)

1. Você verá uma lista de usuários aqui. Selecione o usuário Marketo Sync dedicado ou entre em contato com [Serviços de Federação do Ative Diretory](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} (ADFS) para criar um usuário dedicado para o Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Selecione o usuário de sincronização. Clique em **[!UICONTROL Gerenciar Funções]**.

   ![](assets/assign4.png)

1. Marque Marketo Sync User e clique em **[!UICONTROL OK]**.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Se você não vir a função, volte para [etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) e importe a solução.

   >[!NOTE]
   >
   >Quaisquer atualizações feitas em seu CRM pelo Usuário do Sync _não_ ser sincronizado com o Marketo.

## Configurar a solução da Marketo {#configure-marketo-solution}

Quase pronto! Temos apenas algumas últimas configurações antes de passar para o próximo artigo.

1. Em **[!UICONTROL Configurações]**, clique em **[!UICONTROL Configuração do Marketo]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Se a Configuração do Marketo estiver ausente, tente atualizar a página. Se o problema persistir, [publicar a solução da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"} ou tente fazer logout e login novamente.

1. Clique em **[!UICONTROL Padrão]**.

   ![](assets/configure2.png)

1. Clique em **[!UICONTROL Usuário do Marketo]** e selecione o usuário de sincronização.

   ![](assets/configure3.png)

1. Clique no ícone de salvar no canto inferior direito.

   ![](assets/configure4.png)

1. Clique em **[!UICONTROL Publicar todas as personalizações]**.

   ![](assets/publish-all-customizations1.png)

## Antes de prosseguir para a Etapa 3 {#before-proceeding-to-step}

* Se quiser restringir o número de registros sincronizados, [configurar um filtro de sincronização personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} agora.
* Execute o [Validar a sincronização do Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} processo. Ele verifica se as configurações iniciais foram feitas corretamente.
* Faça logon no Usuário do Marketo Sync no Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Instalar o Marketo para Microsoft Dynamics 2016/Dynamics 365 no Local Etapa 3 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md){target="_blank"}
