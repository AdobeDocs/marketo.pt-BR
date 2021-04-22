---
description: Configuração do OAuth 2.0 - Documentos do Marketo - Documentação do produto
title: Configuração do OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Configuração do OAuth 2.0 {#setting-up-oauth-2-0}

O Salesforce usa o protocolo OAuth para permitir que os usuários de aplicativos acessem com segurança (autentiquem o aplicativo usando OAuth 2.0) os dados por meio de chamadas de API REST sem precisar revelar credenciais de logon. Abaixo estão as etapas a serem executadas para conectar e sincronizar o Marketo com o Salesforce de forma segura.

## Configurar o aplicativo conectado {#set-up-connected-app}

1. No Salesforce, em Configurar, nas Ferramentas da plataforma, navegue até Aplicativos, Gerenciador de aplicativos e clique em **Novo aplicativo conectado**.

   ![](assets/setting-up-oauth-2-1.png)

1. Preencha os detalhes e clique em **Save**.

   ![](assets/setting-up-oauth-2-2.png)

1. Clique na caixa de seleção **Ativar configurações OAuth**. Para URL de Retorno, insira `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. Selecione todos os escopos OAuth disponíveis e clique em **Adicionar**.

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


1. Na seção Marketo Admin , clique em **CRM** e em **Sincronizar com Salesforce**.

   ![](assets/setting-up-oauth-2-7.png)

1. Adicione as informações da Chave do consumidor e do Segredo do consumidor que você gravou anteriormente e clique em e **Salvar**.

   ![](assets/setting-up-oauth-2-8.png)

1. Na página de sincronização do Marketo Salesforce , clique no botão **Login with Salesforce** .

   ![](assets/setting-up-oauth-2-9.png)

1. Um pop-up com a página de logon do salesforce será exibido. Chave em suas credenciais de &quot;Usuário do Marketo Sync&quot; e faça logon.

   ![](assets/setting-up-oauth-2-10.png)

1. Insira o código de verificação recebido por email (enviado pelo Salesforce) e clique em **Verify**.

   ![](assets/setting-up-oauth-2-11.png)

1. Após a verificação bem-sucedida, a página de acesso será exibida solicitando o acesso. Clique em **Permitir**.

   ![](assets/setting-up-oauth-2-12.png)

1. Em alguns minutos, uma pop-up será exibida no Marketo. Clique em **Confirmar Credenciais**.

   ![](assets/setting-up-oauth-2-13.png)

1. Após a conclusão da Sincronização de Campo, clique em **Iniciar Sincronização do Salesforce**.

   ![](assets/setting-up-oauth-2-14.png)

1. Clique em **Iniciar Sincronização**.

   ![](assets/setting-up-oauth-2-15.png)

Sua sincronização entre o Marketo e o Salesforce está em andamento.

![](assets/setting-up-oauth-2-16.png)
