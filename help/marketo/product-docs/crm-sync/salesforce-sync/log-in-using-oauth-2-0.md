---
description: Faça logon usando o OAuth 2.0 - Documentação do Marketo - Documentação do produto
title: Faça logon usando o OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# Faça logon usando o OAuth 2.0 {#log-in-using-oauth-2-0}

O Salesforce usa o protocolo OAuth para permitir que os usuários de aplicativos acessem com segurança (autentique o aplicativo usando o OAuth 2.0) os dados sem precisar revelar credenciais de logon. Abaixo estão as etapas a serem executadas para conectar e sincronizar com segurança o Marketo Engage com o Salesforce.

>[!IMPORTANT]
>
>Para conectar o Marketo e o [!DNL Salesforce] usando OAuth, faça logon no Marketo via navegador privado (incógnito) para evitar a conexão com [!DNL Salesforce] com o nome de usuário errado.

## Configurar o aplicativo conectado {#set-up-connected-app}

1. No Salesforce, em Configuração, nas Ferramentas da plataforma, navegue até Aplicativos, Gerenciador de aplicativos e clique em **[!UICONTROL Novo aplicativo conectado]**.

   ![](assets/setting-up-oauth-2-1.png)

1. Preencha os detalhes e clique em **[!UICONTROL Salvar]**.

   ![](assets/setting-up-oauth-2-2.png)

1. Clique na caixa de seleção **[!UICONTROL Habilitar configurações do OAuth]**. Para a URL de Retorno, digite `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. Selecione todos os Escopos OAuth disponíveis e clique em **[!UICONTROL Adicionar]**.

   ![](assets/setting-up-oauth-2-3.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/setting-up-oauth-2-4.png)

1. Clique em **[!UICONTROL Continuar]**.

   ![](assets/setting-up-oauth-2-5.png)

1. Copie a chave do consumidor e o segredo do consumidor (você precisará deles mais tarde para usar no Marketo Engage).

   ![](assets/setting-up-oauth-2-6.png)

>[!CAUTION]
>
>Enquanto ainda estiver na página Novo aplicativo conectado, role para baixo e verifique se a caixa de seleção &quot;Exigir chave de prova para troca de código (PKCE)&quot; está _NÃO_ marcada, pois isso interferiria na configuração.

## Configurar o Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* O acesso à API deve ser ativado para o usuário do Salesforce Sync (se você for um usuário do Salesforce Professional Edition, esse acesso não estará disponível por padrão. Entre em contato com o executivo da conta da Salesforce).
>* O usuário do Marketo Sync deve ser criado no Salesforce.
>* Para clientes existentes, o recurso para &quot;Habilitar OAuth para sincronização do SFDC&quot; está habilitado na assinatura do cliente.
>* Os bloqueadores de pop-ups estão desativados.
>* O Aplicativo Conectado foi criado e temos a [!UICONTROL Chave do Consumidor] e o [!UICONTROL Segredo do Consumidor] disponíveis para uso.

>[!CAUTION]
>
>Oculte todos os campos desnecessários no Marketo do usuário de sincronização antes de clicar em **[!UICONTROL Sincronizar campos]**. Depois de clicar em Sincronizar campos, todos os campos que o usuário puder ver no SFDC serão criados no Marketo permanentemente e não poderão ser excluídos.

1. Na seção Administrador do Marketo, clique em **[!UICONTROL CRM]** e em **[!UICONTROL Sincronizar com o Salesforce]**.

   ![](assets/setting-up-oauth-2-7.png)

1. Adicione as informações da Chave do consumidor e do Segredo do consumidor gravadas anteriormente e clique em e **[!UICONTROL Salvar]**.

   ![](assets/setting-up-oauth-2-8.png)

1. Na página de sincronização do Marketo Salesforce, clique no botão **[!UICONTROL Fazer logon com o Salesforce]**.

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >Se você estiver vendo os campos Nome de usuário/Senha/Token e não um botão &quot;Logon com o Salesforce&quot;, sua Assinatura do Marketo será habilitada para a Autenticação básica. Consulte [Configurar o Marketo com Autenticação Básica](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md){target="_blank"}. Quando a sincronização começar a usar um conjunto de credenciais, não haverá alternância de credenciais ou assinatura da Salesforce. Se quiser usar o Oauth 2.0, entre em contato com a Equipe de conta da Adobe (seu Gerente de conta).

1. Um pop-up com a página de logon do salesforce será exibido. Insira suas credenciais de &quot;Usuário da sincronização do Marketo&quot; e faça logon.

   ![](assets/setting-up-oauth-2-10.png)

1. Insira o código de verificação recebido por email (enviado pela Salesforce) e clique em **[!UICONTROL Verificar]**.

   ![](assets/setting-up-oauth-2-11.png)

1. Após a verificação bem-sucedida, a página de acesso será exibida solicitando acesso. Clique em **[!UICONTROL Permitir]**.

   ![](assets/setting-up-oauth-2-12.png)

1. Em alguns minutos, uma janela pop-up será exibida no Marketo. Clique em **[!UICONTROL Confirmar Credenciais]**.

   ![](assets/setting-up-oauth-2-13.png)

1. Após a conclusão da Sincronização de Campo, clique em **[!UICONTROL Iniciar Sincronização do Salesforce]**.

   ![](assets/setting-up-oauth-2-14.png)

1. Clique em **[!UICONTROL Iniciar sincronização]**.

   ![](assets/setting-up-oauth-2-15.png)

A sincronização entre o Marketo e o [!DNL Salesforce] está em andamento.

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [Etapa 1 de 3: Adicionar Campos do Marketo à Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [Etapa 2 de 3: Criar um Usuário do Salesforce para Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}
>* [Instalar o pacote Marketo Sales Insight no Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [Configurar o Marketo Sales Insight no Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md){target="_blank"}
