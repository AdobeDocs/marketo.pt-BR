---
unique-page-id: 3571800
description: Etapa 3 de 3 - Conectar o Marketo e o Salesforce (Professional) - Documentação do Marketo - Documentação do produto
title: Etapa 3 de 3 - Conectar o Marketo e o Salesforce (Professional)
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Etapa 3 de 3: Conectar o Marketo e o Salesforce (Professional) {#step-of-connect-marketo-and-salesforce-professional}

Neste artigo, você configurará o Marketo para sincronizar com sua instância do Salesforce configurada.

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: Adicionar campos do Marketo ao Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)
>* [Etapa 2 de 3: Criar um usuário do Salesforce para Marketo (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)

## Recuperar Token de Segurança do Usuário de Sincronização {#retrieve-sync-user-security-token}

>[!TIP]
>
>Se você já tiver o token de segurança, prossiga diretamente para Definir credenciais de usuário de sincronização e kudos para a preparação!

1. Faça logon no Salesforce com o Usuário de sincronização do Marketo, clique no nome do usuário de sincronização e **Minhas configurações**.

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. Na barra de pesquisa de navegação, digite &quot;redefinir&quot; e clique em **Redefinir meu token de segurança**.

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. Clique em **Redefinir token de segurança**.

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   O token de segurança será enviado a você por email.

## Definir Credenciais de Usuário de Sincronização {#set-sync-user-credentials}

1. No Marketo, acesse **Admin**, selecione **CRM** e clique em **Sincronizar com [Salesforce.com](https://Salesforce.com)**.

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Certifique-se de [ocultar todos os campos desnecessários](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md) no Marketo do usuário de sincronização antes de clicar em **Sincronizar campos**. Depois de clicar em Sincronizar campos, todos os campos que o usuário puder ver serão criados no Marketo permanentemente e não poderão ser excluídos.

1. Insira as credenciais do usuário da sincronização do Salesforce criadas na parte 2 da configuração do Salesforce ([Profissional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md), [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) e clique em **Sincronizar campos**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Marcar **Sandbox** se estiver sincronizando uma sandbox da Marketo com uma sandbox do Salesforce.

1. Leia o aviso e clique em **Confirmar credenciais**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Se você quiser ver o [mapeamentos e personalizá-los](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md)Esta é a sua única chance! Depois de clicar em Iniciar sincronização do Salesforce, isso estará concluído.

## Iniciar sincronização com Salesforce {#start-salesforce-sync}

1. Clique em **Iniciar a sincronização do Salesforce** para iniciar a sincronização persistente entre o Marketo e o Salesforce.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >A Marketo não eliminará automaticamente a duplicação em relação a uma sincronização do Salesforce ou ao inserir leads manualmente.

1. Clique em **Iniciar sincronização**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >O tempo para concluir a sincronização inicial varia dependendo do tamanho e da complexidade do banco de dados.

## Verificar sincronização {#verify-sync}

O Marketo fornece mensagens de status para a sincronização do Salesforce na área de Administração. Você pode verificar se a sincronização está funcionando corretamente seguindo estas etapas.

1. No Marketo, clique em **Admin**, depois **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. O status da sincronização está visível no canto superior direito. Ele mostrará uma das três mensagens: **Última sincronização**, **Sincronização em andamento** ou **Failed**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Uau, você acabou de configurar um dos recursos mais eficientes do Marketo, vá você!

>[!MORELIKETHIS]
>
>* [Instalar o pacote Marketo Sales Insight no Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configurar o Marketo Sales Insight no Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
