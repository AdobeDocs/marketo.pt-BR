---
unique-page-id: 2360366
description: Etapa 3 de 3 - Conectar o Marketo e o Salesforce (Enterprise/Unlimited) - Documentação do Marketo - Documentação do produto
title: Etapa 3 de 3 - Conectar o Marketo e o Salesforce (Enterprise/Unlimited)
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Etapa 3 de 3: Conectar o Marketo e [!DNL Salesforce] (Empresa/Ilimitado) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

Neste artigo, você configurará o Marketo para sincronizar com a instância [!DNL Salesforce] configurada.

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: Adicionar Campos do Marketo a [!DNL Salesforce] (Empresarial/Ilimitada)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Etapa 2 de 3: Criar um [!DNL Salesforce] Usuário para Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)

## Recuperar Token de Segurança do Usuário de Sincronização {#retrieve-sync-user-security-token}

>[!TIP]
>
>Se você já tiver o token de segurança, prossiga diretamente para Definir credenciais de usuário de sincronização e kudos para a preparação!

1. Faça logon em [!DNL Salesforce] com o Usuário de sincronização do Marketo, clique no nome do usuário de sincronização e em **[!UICONTROL Minhas configurações]**.

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. Na localização rápida, digite &quot;redefinir&quot; e clique em **[!UICONTROL Redefinir Meu Token de Segurança]**.

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. Clique em **[!UICONTROL Redefinir token de segurança]**.

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   O token de segurança será enviado a você por email.

## Definir Credenciais de Usuário de Sincronização {#set-sync-user-credentials}

1. No Marketo, vá para **[!UICONTROL Admin]**, selecione **CRM** e clique em **[!UICONTROL Sincronizar com o Salesforce.com]**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Certifique-se de [ocultar todos os campos desnecessários](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md) no Marketo do usuário de sincronização antes de clicar em **[!UICONTROL Sincronizar Campos]**. Depois de clicar em [!UICONTROL Sincronizar Campos], todos os campos que o usuário puder ver serão criados permanentemente no Marketo e não poderão ser excluídos.

1. Insira as credenciais do Usuário de Sincronização [!DNL Salesforce] criadas na parte 2 da configuração [!DNL Salesforce] ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md) ou [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) e clique em **[!UICONTROL Sincronizar Campos]** (marque **[!UICONTROL Sandbox]** somente se estiver sincronizando uma Sandbox da Marketo com uma Sandbox do [!DNL Salesforce]).

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >Se você vir um Botão &quot;Logon no [!DNL Salesforce]&quot; em vez dos campos Nome de usuário/Senha/Token, sua Assinatura do Marketo será habilitada para OAuth. [Consulte este artigo](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md). Assim que a sincronização começar a usar um conjunto de Credenciais, **não haverá alternância de [!DNL Salesforce] credenciais ou assinatura**. Se quiser usar a Autenticação básica, entre em contato com o Gerente de sucesso do cliente.

1. Leia o aviso e clique em **[!UICONTROL Confirmar Credenciais]**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Se você quiser examinar os [mapeamentos e personalizá-los](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md), esta é sua única chance! Depois de clicar em [!UICONTROL Iniciar Sincronização com o Salesforce], isso estará concluído.

## Iniciar Sincronização de [!DNL Salesforce] {#start-salesforce-sync}

1. Clique em **[!UICONTROL Iniciar Sincronização do Salesforce]** para iniciar a sincronização persistente do Marketo-[!DNL Salesforce].

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >A Marketo não desduplicará automaticamente em uma sincronização [!DNL Salesforce] ou ao inserir clientes em potencial manualmente.

1. Clique em **[!UICONTROL Iniciar sincronização]**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >O tempo para concluir a sincronização inicial varia dependendo do tamanho e da complexidade do banco de dados.

## Verificar sincronização {#verify-sync}

O Marketo fornece mensagens de status para a sincronização [!DNL Salesforce] na área de Administração. Você pode verificar se a sincronização está funcionando corretamente seguindo estas etapas.

1. No Marketo, clique em **[!UICONTROL Admin]** e depois em **[!UICONTROL Salesforce]**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. O status da sincronização está visível no canto superior direito. Ele mostrará uma das três mensagens: **[!UICONTROL Última Sincronização]**, **[!UICONTROL Sincronização em Andamento]** ou **[!UICONTROL Falha]**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Você acabou de configurar um dos recursos mais avançados do Marketo, clique!

>[!MORELIKETHIS]
>
>* [Etapa 1 de 3: Adicionar Campos do Marketo a [!DNL Salesforce] (Empresarial/Ilimitada)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Etapa 2 de 3: Criar um [!DNL Salesforce] Usuário para Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Instalar o Pacote Marketo Sales Insight em [!DNL Salesforce] AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configurar o Marketo Sales Insight em [!DNL Salesforce] Empresa/Ilimitado](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
