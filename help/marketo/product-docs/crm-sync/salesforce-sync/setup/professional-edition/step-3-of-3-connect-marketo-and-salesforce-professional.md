---
unique-page-id: 3571800
description: Etapa 3 de 3 - Conectar o Marketo e o Salesforce (Professional) - Documentos da Marketo - Documentação do produto
title: Etapa 3 de 3 - Conectar o Marketo e o Salesforce (Professional)
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Etapa 3 de 3: Conecte o Marketo e o Salesforce (Professional) {#step-of-connect-marketo-and-salesforce-professional}

Neste artigo, você configurará o Marketo para sincronizar com a instância configurada do Salesforce.

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: Adicionar campos do Marketo ao Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)
>* [Etapa 2 de 3: Criar um usuário do Salesforce para Marketo (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)


## Recuperar o token de segurança do usuário de sincronização {#retrieve-sync-user-security-token}

>[!TIP]
>
>Se você já tiver o token de segurança, continue diretamente para Definir as credenciais do usuário de sincronização e os kudos para preparação!

1. Faça logon no Salesforce com o Usuário do Marketo Sync, clique no nome do usuário de sincronização e, em seguida, em **Minhas configurações**.

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. Na barra de pesquisa Navegação, digite &quot;redefinir&quot; e clique em **Redefinir meu token de segurança**.

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. Clique em **Redefinir token de segurança**.

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   O token de segurança será enviado a você por email.

## Definir as credenciais do usuário de sincronização {#set-sync-user-credentials}

1. No Marketo, vá para **Admin**, selecione **CRM** e clique em **Sincronizar com [Salesforce.com](https://Salesforce.com)**.

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Certifique-se de [ocultar todos os campos que você não precisa](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync/hide-a-salesforce-field-from-the-marketo-sync.md) no Marketo do usuário de sincronização antes de clicar em **Sincronizar campos**. Depois de clicar em Sincronizar campos, todos os campos que o usuário pode ver serão criados no Marketo permanentemente e não poderão ser excluídos.

1. Insira as credenciais do Usuário de Sincronização do Salesforce criadas na parte 2 da configuração do Salesforce ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md), [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) e clique em **Sincronizar Campos**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Marque **Sandbox** se estiver sincronizando uma Sandbox do Marketo com uma Sandbox do Salesforce.

1. Leia o aviso e clique em **Confirmar Credenciais**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Se quiser examinar os [mapeamentos e personalizá-los](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md), esta é sua única chance de fazer isso! Depois de clicar em Iniciar Sincronização do Salesforce, está pronto.

## Iniciar sincronização com Salesforce {#start-salesforce-sync}

1. Clique em **Iniciar Sincronização do Salesforce** para iniciar a sincronização persistente do Marketo-Salesforce.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >A Marketo não deduplicará automaticamente uma sincronização do Salesforce ou quando você inserir leads manualmente.

1. Clique em **Iniciar Sincronização**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >O tempo para concluir a sincronização inicial varia dependendo do tamanho e da complexidade do banco de dados.

## Verificar Sincronização {#verify-sync}

O Marketo fornece mensagens de status para a sincronização do Salesforce na área de Administração. É possível verificar se a sincronização está funcionando corretamente seguindo essas etapas.

1. No Marketo, clique em **Admin** e, em seguida, em **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. O status de sincronização é visível no canto superior direito. Ele mostrará uma das três mensagens: **Última Sincronização**, **Sincronização em Andamento** ou **Falha**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Acabou de configurar um dos recursos mais poderosos do Marketo, vai!

>[!MORELIKETHIS]
>
>* [Instalar o pacote de informações de vendas da Marketo no Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configurar o Marketo Sales Insight no Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)

