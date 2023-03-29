---
description: Faça logon usando o OAuth 2.0 - Documentos do Marketo - Documentação do produto
title: Fazer logon usando o OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Fazer logon usando o OAuth 2.0 {#log-in-using-oauth-2-0}

O Salesforce usa o protocolo OAuth para permitir que os usuários de aplicativos acessem com segurança (autentiquem o aplicativo usando OAuth 2.0) sem precisar revelar credenciais de logon. Abaixo estão as etapas a serem executadas para conectar e sincronizar o Marketo com o Salesforce de forma segura.

>[!IMPORTANT]
>
>Para conectar o Marketo e o Salesforce usando o OAuth, faça logon no Marketo via navegador privado (incógnito) para evitar se conectar ao Salesforce com o nome de usuário errado.

## Configurar Aplicativo Conectado {#set-up-connected-app}

1. No Salesforce, em Configurar, nas Ferramentas da plataforma, navegue até Aplicativos, Gerenciador de aplicativos e clique em **Novo Aplicativo Conectado**.

   ![](assets/setting-up-oauth-2-1.png)

1. Preencha os detalhes e clique em **Salvar**.

   ![](assets/setting-up-oauth-2-2.png)

1. Clique no botão **Ativar as configurações do OAuth** caixa de seleção. Para URL de retorno, insira `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. Selecione todos os escopos OAuth disponíveis e clique em **Adicionar**.

   ![](assets/setting-up-oauth-2-3.png)

1. Clique em **Salvar**.

   ![](assets/setting-up-oauth-2-4.png)

1. Clique em **Continuar**.

   ![](assets/setting-up-oauth-2-5.png)

1. Copie a chave do consumidor e o segredo do consumidor.

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>Salve as informações da Chave do consumidor e do Segredo do consumidor para uso posterior no Marketo.

## Configurar Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* O acesso à API deve ser ativado para o Usuário de Sincronização do Salesforce (se você for um usuário do Salesforce Professional Edition, esse acesso não estará disponível por padrão - entre em contato com seu Executivo de contas do Salesforce).
>* O usuário do Marketo Sync deve ser criado no Salesforce.
>* Para clientes existentes, o recurso para &quot;Habilitar OAuth para sincronização SFDC&quot; é ativado na assinatura do cliente.
>* Bloqueadores de pop-up estão desativados.
>* O aplicativo conectado é criado e temos a chave do consumidor e o segredo do consumidor disponíveis para uso.


>[!CAUTION]
>
>Certifique-se de ocultar todos os campos que você não precisa no Marketo do usuário de sincronização antes de clicar **Sincronizar campos**. Depois de clicar em Sincronizar campos, todos os campos que o usuário pode ver no SFDC serão criados no Marketo permanentemente e não poderão ser excluídos.

1. Na seção Marketo Admin , clique em **CRM**, em seguida **Sincronizar com o Salesforce**.

   ![](assets/setting-up-oauth-2-7.png)

1. Adicione as informações da chave do consumidor e do segredo do consumidor que você gravou anteriormente e clique em e **Salvar**.

   ![](assets/setting-up-oauth-2-8.png)

1. Na página de sincronização do Marketo Salesforce , clique no link **Logon com o Salesforce** botão.

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >Se você estiver vendo campos Nome de usuário/Senha/Token e não um botão &quot;Logon com Salesforce&quot;, sua assinatura do Marketo será ativada para Autenticação básica. Consulte [Configurar o Marketo com autenticação básica](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md). Depois que a sincronização começar a usar um conjunto de credenciais, não haverá alternância de credenciais ou assinaturas do Salesforce. Se quiser usar o Oauth 2.0, entre em contato com a Equipe de conta do Adobe (seu Gerente de conta).

1. Um pop-up com a página de logon do salesforce será exibido. Chave em suas credenciais de &quot;Usuário do Marketo Sync&quot; e faça logon.

   ![](assets/setting-up-oauth-2-10.png)

1. Insira o código de verificação recebido por email (enviado pelo Salesforce) e clique em **Verificar**.

   ![](assets/setting-up-oauth-2-11.png)

1. Após a verificação bem-sucedida, a página de acesso será exibida solicitando o acesso. Clique em **Permitir**.

   ![](assets/setting-up-oauth-2-12.png)

1. Em alguns minutos, uma pop-up será exibida no Marketo. Clique em **Confirmar Credenciais**.

   ![](assets/setting-up-oauth-2-13.png)

1. Após concluir a sincronização do campo, clique em **Iniciar Sincronização do Salesforce**.

   ![](assets/setting-up-oauth-2-14.png)

1. Clique em **Iniciar Sincronização**.

   ![](assets/setting-up-oauth-2-15.png)

Sua sincronização entre o Marketo e o Salesforce está em andamento.

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [Etapa 1 de 3: Adicionar campos do Marketo ao Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Etapa 2 de 3: Criar um usuário do Salesforce para Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Instalar o pacote de informações de vendas da Marketo no Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configurar o Marketo Sales Insight no Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

