---
description: Configurar uma sandbox de ações do Sales Insight - Documentação do Marketo - Documentação do produto
title: Configurar uma sandbox de ações de insights de vendas
exl-id: 8bc3a8a6-7fbc-4cbe-99a7-21b066ec4f96
source-git-commit: 1f228323c18204149630a7cb77d6ae0a88b425e3
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Configurar uma sandbox de ações de insights de vendas {#set-up-a-sales-insight-actions-sandbox}

>[!NOTE]
>
>As Ações do Marketo Sales Insight são um aplicativo baseado na Web que se integra exclusivamente ao Salesforce CRM por meio do [pacote do Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. Às vezes, é chamado de &quot;Vendas do Marketo&quot; ou simplesmente &quot;Ações&quot;.

Se você tiver uma sandbox da Marketo, poderá ativar uma instância de Ações para ser usada com sua sandbox para fins de teste.

Ao configurar uma instância de Ações, você deve decidir se ela será configurada para funcionar com a Sandbox do Salesforce ou com a produção do Salesforce. Isso ocorre porque o Salesforce usa endpoints diferentes para cada um, e o Actions usa a conexão com o Salesforce para ativar e autenticar usuários.

Siga as etapas abaixo para configurar uma instância de Ações para funcionar com sua instância de sandbox do Salesforce.

>[!NOTE]
>
>Você pode saber mais sobre como os usuários [ativarão sua vaga Ações](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-checklist.md){target="_blank"}. Você também pode saber como os usuários [se autenticarão com o Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}. Além disso, se você preferir que os usuários se autentiquem por email e senha, poderá saber mais sobre isso em nosso [artigo de configurações de Gerenciamento de Logon](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

## Solicite o provisionamento de uma instância de ações para sua sandbox da Marketo {#request=an-actions-instance}

As Ações de Insight de vendas não estão habilitadas para instâncias de sandbox da Marketo, a menos que solicitado. Entre em contato com a equipe de conta do Adobe (seu gerente de conta) para enviar uma solicitação.

## Provisionar sua conta de ações para a sandbox da Marketo {#provision-your-actions-account}

Depois que as Ações forem ativadas para a sandbox da Marketo, será necessário seguir as etapas abaixo para ativar a nova instância.

1. Faça logon na instância da sandbox da Marketo.

1. Navegue até **Admin**.

1. Selecione **Sales Insight**.

1. Selecione **Configurações de Ações**.

   >[!IMPORTANT]
   >
   >Um endereço de email só pode ser usado para uma instância de Ações nas instâncias de Sandbox e Produção. Se você for um administrador que precisará acessar várias instâncias na Produção e na Sandbox, use um endereço de email diferente para cada uma.

1. No cartão de provisionamento, selecione o usuário que deseja convidar para a instância de Ações do Insight de vendas.

## Ativar a instância de ações {#activate-your-actions-instance}

Sua instância de Ações precisará ser ativada com uma conta de produção do Salesforce. Após a ativação, ele pode ser alternado para uma conta de sandbox do Salesforce.

1. Localize o convite enviado.

1. Clique no link **Introdução**.

1. Ative com sua instância de Produção do Salesforce.

1. Siga as instruções para configurar a conta. Para obter uma visão geral detalhada, consulte nosso [artigo sobre a integração de usuários](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}.

## Preparar sua instância de ações para ser compatível com sua instância de sandbox do Salesforce {#prepare-your-actions-instance}

As ações exigem que você ative uma nova instância com um usuário de produção do Salesforce primeiro. Depois de ativada, você pode usar as seguintes etapas para preparar sua instância para ser compatível com o Salesforce Sandbox.

1. Atualize as configurações de logon para &quot;Todos os métodos de logon&quot;, para que você possa fazer logon com um nome de usuário e senha, se necessário. Se preferir, isso poderá ser alternado de volta para &quot;Somente Salesforce&quot; depois que tudo estiver configurado. [Veja como fazer isso aqui](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

1. Desconecte-se da produção do Salesforce e conecte-se à sua sandbox do Salesforce. [Veja como se conectar aqui](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}. Para a etapa 3, selecione &quot;Sandbox&quot; em vez de &quot;Salesforce&quot;. Se já estiver conectado, você verá uma opção para desconectar na guia Conexões e personalizações do Salesforce.

>[!NOTE]
>
>Se você tiver um domínio personalizado para sua instância do Salesforce, recomendamos fazer logon na sua instância do Salesforce antes de se conectar ao Salesforce ou fazer logon no Actions.

## Solicite que a instância de suas ações seja convertida para ser compatível com sua sandbox do Salesforce {#request-your-actions-instance-be-converted}

1. Entre em contato com o [Suporte de Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} para solicitar que sua nova instância de Ações do Sales Insight seja configurada para ser compatível com a sandbox do Salesforce.

1. Para testar se tudo está configurado corretamente, tente fazer logon usando o botão &quot;Fazer logon no Salesforce&quot; na página toutapp.com/login.

   ![](assets/set-up-a-sales-insight-actions-sandbox-1.png)

   >[!TIP]
   >
   >Se você tiver problemas neste momento, poderá solicitar uma redefinição de senha e usar uma senha para recuperar o acesso à sua conta.

Agora, sua instância está pronta para ser usada com a instância de sandbox do Salesforce. Se você quiser usar o [logon automático do Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"} a partir do Salesforce, poderá voltar para &quot;Salesforce apenas&quot; nas [configurações de gerenciamento de logon](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

>[!NOTE]
>
>* [Conecte sua conta de ações do Sales Insight ao Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}
>* [Guia de integração do usuário de ações do Sales Insight](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}
>* [Logon automático do Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}
>* [Configurações de gerenciamento de logon](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}
