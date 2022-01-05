---
description: Instale o Marketo para Microsoft Dynamics 2016/Dynamics 365 no local Etapa 2 de 3 - Documentos do Marketo - Documentação do produto
title: Instale o Marketo para Microsoft Dynamics 2016/Dynamics 365 no local Etapa 2 de 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
source-git-commit: 3fb93520a653109845c3b40aba20304c6163214f
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Etapa 2 de 3 Configurar o Marketo para Dynamics (2016 no local/Dynamics 365 no local){#step-of-set-up-for-marketo-on-premises-2016}

Excelente trabalho ao concluir as etapas anteriores. Vamos continuar a passar por isto.

>[!PREREQUISITES]
>
>[Instale o Marketo para Microsoft Dynamics 2016/Dynamics 365 no local Etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## Criar um novo usuário {#create-a-new-user}

1. Faça logon no Dynamics. Clique no ícone Configurações e selecione Configurações avançadas.

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. Clique em **Configurações** e selecione **Segurança**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. Clique em **Usuários**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. Clique em **Novo**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. Clique em **Adicionar e Licenciar Usuários**. Uma nova guia deve abrir.

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. Clique em **Administrador** na parte superior da página. Outra nova guia deve abrir.

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. Clique em **Adicionar um usuário**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. Insira todas as suas informações. Quando terminar, clique em **Adicionar**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >Esse nome deve ser um usuário de sincronização dedicado e não uma conta de usuário do CRM existente. Não precisa ser um endereço de email real.

1. Digite o email para receber as novas credenciais do usuário e clique em Enviar email e fechar.

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## Criar um novo aplicativo cliente {#create-a-new-client-application}

Siga as etapas em [este artigo do Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later) para criar um novo Aplicativo cliente e conceder permissões. Anote a ID/segredo do cliente do aplicativo cliente Dynamics.

## Atribuir Função de Usuário de Sincronização {#assign-sync-user-role}

Atribua a função Usuário de sincronização do Marketo somente ao usuário de sincronização do Marketo. Não é necessário atribuí-lo a nenhum outro usuário.

>[!NOTE]
>
>Isso se aplica ao Marketo versão 4.0.0.14 e posterior. Para versões anteriores, todos os usuários devem ter a função de sincronização do usuário. Para atualizar sua Marketo, consulte [Atualizar a solução Marketo para o Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>A configuração de idioma do Usuário de sincronização [deve ser definido como inglês](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. Em **Configurações**, clique em **Segurança**.

   ![](assets/assign1.png)

1. Clique em **Usuários**.

   ![](assets/assign2.png)

1. Você verá uma lista de usuários aqui. Selecione o usuário dedicado do Marketo Sync ou entre em contato com seu [Serviços de Federação do Ative Diretory](https://msdn.microsoft.com/en-us/library/bb897402.aspx)Administrador do (ADFS) para criar um usuário dedicado ao Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Selecione o usuário de sincronização. Clique em **Gerenciar funções**.

   ![](assets/assign4.png)

   Marque Marketo Sync User (Usuário de sincronização do) e clique em OK.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Se você não vir a função, volte para [etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) e importe a solução.

   >[!NOTE]
   >
   >Qualquer atualização feita em seu CRM pelo Usuário de sincronização **not** ser sincronizado de volta ao Marketo.

## Configurar a solução Marketo {#configure-marketo-solution}

Quase pronto! Temos apenas algumas últimas partes da configuração antes de passar para o próximo artigo.

1. Em **Configurações**, clique em **Configuração do Marketo**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Se a configuração do Marketo estiver ausente, tente atualizar a página. Se o problema persistir, [publicar a solução Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) ou tente sair e voltar.

1. Clique em **Padrão**.

   ![](assets/configure2.png)

1. Clique no botão **Usuário do Marketo** e selecione o usuário de sincronização.

   ![](assets/configure3.png)

1. Clique no ícone Save no canto inferior direito.

   ![](assets/configure4.png)

1. Clique em **Publicar todas as personalizações**.

   ![](assets/publish-all-customizations1.png)

## Antes de prosseguir para a Etapa 3 {#before-proceeding-to-step}

* Se quiser restringir o número de registros sincronizados, [configurar um filtro de sincronização personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) agora.
* Execute o [Validar a sincronização do Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) processo. Ele verifica se as configurações iniciais foram feitas corretamente.
* Faça logon no usuário do Marketo Sync no Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Instale o Marketo para Microsoft Dynamics 2016/Dynamics 365 no local Etapa 3 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
