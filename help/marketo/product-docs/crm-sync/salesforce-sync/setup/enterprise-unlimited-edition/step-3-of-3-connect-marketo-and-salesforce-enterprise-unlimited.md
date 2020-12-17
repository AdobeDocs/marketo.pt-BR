---
unique-page-id: 2360366
description: Etapa 3 de 3 - Connect Marketing e Salesforce (Enterprise/Unlimited) - Documentação do produto - Documentação do produto
title: Etapa 3 de 3 - Connect Marketing e Salesforce (Enterprise/Unlimited)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---


# Etapa 3 de 3: Connect Marketo e Salesforce (Enterprise/Unlimited) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

Neste artigo, você configurará o Marketo para sincronizar com a instância configurada do Salesforce.

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: Adicionar campos de marketing ao Salesforce (Enterprise/Unlimited)](step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Etapa 2 de 3: Criar um usuário do Salesforce para o Marketing (Enterprise/Unlimited)](../../../../../product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md) [](https://community.marketo.com/MarketoTutorial?id=kA250000000Kz5rCAC)

>



## Recuperar o token de segurança do usuário de sincronização {#retrieve-sync-user-security-token}

>[!TIP]
>
>Se você já tiver o token de segurança, prossiga diretamente para Definir as credenciais de sincronização do usuário e os kudos para preparação!

1. Faça logon no Salesforce com o usuário de sincronização de marketing, clique no nome do usuário de sincronização e **Minhas configurações**.

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. Na localização rápida, digite &quot;reset&quot; e clique em **Redefinir meu token de segurança**.

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. Clique em **Redefinir token de segurança**.

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   O token de segurança será enviado a você por email.

## Definir as credenciais de sincronização do usuário {#set-sync-user-credentials}

1. No Marketo, vá para **Admin**, selecione **CRM** e clique em **Sincronizar com [Salesforce.com](http://Salesforce.com)**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >**Lembrete**
   >
   >
   >Certifique-se de [ocultar todos os campos de que você não precisa](../../../../../product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync/hide-a-salesforce-field-from-the-marketo-sync.md) no Marketo do usuário de sincronização antes de clicar em **Sincronizar campos**. Após clicar em Sincronizar campos, todos os campos que o usuário pode ver serão criados permanentemente no Marketo e não poderão ser excluídos.

1. Digite as credenciais do Usuário de Sincronização do Salesforce criadas na parte 2 da configuração do Salesforce ([Professional](https://community.marketo.com/MarketoArticle?id=kA050000000LJ3QCAW), [Enterprise](https://community.marketo.com/MarketoArticle?id=kA050000000LIwKCAW)) e clique em **Sincronizar campos**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Marque **Sandbox** se você estiver sincronizando uma Marketo Sandbox com uma Salesforce Sandbox.

1. Leia o aviso e clique em **Confirmar credenciais**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Se você quiser olhar por cima dos [mapeamentos e personalizá-los](https://docs.marketo.com/display/public/DOCS/Edit+Initial+Field+Mappings), esta é sua única chance de fazer isso! Quando você clica em Sincronização do Salesforce de Start, está pronto.

## Start Salesforce Sync {#start-salesforce-sync}

1. Clique em **Sincronização do Salesforce do Start** para iniciar a sincronização persistente do Marketo-Salesforce.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >O Marketo não eliminará a duplicação automaticamente em relação a uma sincronização do Salesforce ou quando você inserir vendas manualmente.

1. Clique em **SYNC** START.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >O tempo para concluir a sincronização inicial varia dependendo do tamanho e da complexidade do banco de dados.

## Verificar sincronização {#verify-sync}

O Marketo fornece mensagens de status para a sincronização do Salesforce na área de Administração. Para verificar se a sincronização está funcionando corretamente, siga estas etapas.

1. No Marketo, clique em **Admin** e, em seguida, em **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. O status de sincronização está visível no canto superior direito. Ele mostrará uma de três mensagens: **Última sincronização**, **Sincronização em andamento** ou **Falha**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Nossa, você acabou de configurar um dos recursos mais poderosos do Marketo, vá lá!

>[!NOTE]
>
>**Artigos relacionados**
>
>* [Etapa 1 de 3: Adicionar campos de marketing ao Salesforce (Enterprise/Unlimited)](step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Etapa 2 de 3: Criar um usuário do Salesforce para o Marketing (Enterprise/Unlimited)](step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Instalar o pacote de insight de vendas do Marketing Cloud na AppExchange do Salesforce](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configurar o Marketing to Sales Insight no Salesforce Enterprise/Unlimited](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>* [Etapas opcionais](http://docs.marketo.com/display/docs/optional+steps)

>



