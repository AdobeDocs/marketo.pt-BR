---
description: Guia de configuração do administrador de ações do Sales Insight - Documentação do Marketo - Documentação do produto
title: Guia de configuração do administrador de ações do Sales Insight
exl-id: 339d518d-445b-4634-ab81-92c9d5541927
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 1%

---

# Guia de configuração do administrador de ações do Sales Insight {#sales-insight-actions-admin-setup-guide}

>[!NOTE]
>
>As Ações do Marketo Sales Insight são um aplicativo baseado na Web que se integra à interface do usuário do Salesforce por meio do [pacote do Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. Às vezes, é chamado de &quot;Vendas do Marketo&quot; ou simplesmente &quot;Ações&quot;.

>[!PREREQUISITES]
>
>* Confirme com a Equipe de Conta do Adobe (seu Gerente de Conta) que as Ações MSI foram habilitadas para sua Conta do Marketo Engage (se você não tiver um Gerente de Conta, contate o [Suporte da Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}).
>* A sincronização do Marketo/Salesforce deve ser configurada.

<table>
 <tr>
  <th>Persona</th>
  <th>Etapa</th>
 </tr>
 <tr>
  <td>Administrador do Marketo</td>
  <td>Configurar a conta de vendas do Marketo</td>
 </tr>
 <tr>
  <td>Administrador do Marketo ou <br/>Administrador do Salesforce</td>
  <td>Conectar a conta de vendas do Marketo ao Salesforce</td>
 </tr>
 <tr>
  <td>Administrador do Marketo</td>
  <td>Conectar a conta de vendas do Marketo à Marketo</td>
 </tr>
 <tr>
  <td>Administrador do Marketo</td>
  <td>Iniciar Sincronização de Dados do Marketo para a Conta de Vendas do Marketo</td>
 </tr>
 <tr>
  <td>Administrador do Marketo</td>
  <td>Convidar usuários para ações MSI</td>
 </tr>
 <tr>
  <td>Administrador do Salesforce</td>
  <td>Instalar/atualizar pacote MSI no Salesforce</td>
 </tr>
 <tr>
  <td>Administrador do Salesforce</td>
  <td>Configurar ações do MSI no Salesforce</td>
 </tr>
</table>

## Configurar Conta de Vendas do Marketo {#set-up-marketo-sales-account}

1. No Marketo, clique em **Admin**.

   ![](assets/msi-actions-admin-guide-1.png)

   >[!NOTE]
   >
   >Se você não estiver vendo uma ID do cliente e um Segredo do cliente no cartão de Informações de integração, ative a instância das Ações convidando o primeiro usuário e verá a ID do cliente e o Segredo do cliente aparecerem.

1. Clique em **Sales Insight** e depois em **Actions Config**. Selecione de uma lista de administradores do Marketo a convidar e clique em **Enviar Convite**.

   ![](assets/msi-actions-admin-guide-2.png)

O usuário receberá um email com etapas para obter acesso à conta.

>[!NOTE]
>
>Outros usuários não serão adicionados por meio do Marketo e serão adicionados por meio da página Gerenciamento de usuários da conta de vendas. [Clique aqui](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md){target="_blank"} para saber mais sobre como adicionar outros usuários.

## Conectar a Conta de Vendas da Marketo ao Salesforce {#connect-marketo-sales-account-to-salesforce}

1. Na sua conta do Marketo Sales, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/msi-actions-admin-guide-3.png)

1. Em Configurações do administrador, clique em **Salesforce**.

   ![](assets/msi-actions-admin-guide-4.png)

1. Na guia Conexões e Personalizações, clique em **Conectar**.

   ![](assets/msi-actions-admin-guide-5.png)

1. Clique em **OK**.

   ![](assets/msi-actions-admin-guide-6.png)

Se você já estiver conectado ao Salesforce, você será conectado. Caso não esteja, você será solicitado a fazer logon.

## Conectar o Marketo à sua conta de aplicativos de vendas {#connect-marketo-to-your-sales-apps-account}

1. Na sua conta do Marketo Sales, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/msi-actions-admin-guide-7.png)

1. Em Configurações do Administrador, clique em **Marketo**.

   ![](assets/msi-actions-admin-guide-8.png)

1. Clique em **conectar**. Sua conta será conectada.

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>Se ele não se conectar, copie as credenciais da guia &quot;Configuração de ações&quot; do Marketo Sales Insight e cole-as na guia Configurar.

## Iniciar Sincronização de Dados {#initiate-data-sync}

A sincronização de campo de unificação de dados para Ações do Sales Insight permite que o sistema envie informações de pessoas do banco de dados do Marketo Engage para o banco de dados de Ações do Sales Insight, mantendo os dados de suas pessoas atualizados e garantindo que as atividades sejam registradas nos registros certos no Marketo e no Salesforce.

>[!CAUTION]
>
>Depois de iniciar a sincronização de dados, você deve **não** remover o usuário original na instância das Ações do Insight de vendas. Este é o usuário para o qual o primeiro convite foi enviado.

1. No Marketo, clique em **Admin**.

   ![](assets/msi-actions-admin-guide-10.png)

1. Clique em **Sales Insight**.

   ![](assets/msi-actions-admin-guide-11.png)

1. Clique na guia **Configurações de ações**. No cartão Sincronização de Campo de Ação, clique em **Sincronizar**.

   ![](assets/msi-actions-admin-guide-12.png)

1. Você verá uma pré-visualização dos campos que serão sincronizados. Clique em **Iniciar sincronização**.

   ![](assets/msi-actions-admin-guide-13.png)

Os registros de pessoa que existem no Marketo e no Salesforce serão sincronizados com sua conta do Marketo Sales Apps.

>[!NOTE]
>
>Para saber mais sobre como as pessoas e os dados de atividade são sincronizados entre as Ações do Sales Insight, Marketo e Salesforce, [clique aqui](/help/marketo/product-docs/marketo-sales-insight/actions/admin/sync-sales-action-data-with-marketo-and-salesforce.md){target="_blank"}.

## Convidar usuários individuais para ações do MSI {#invite-individual-users-to-msi-actions}

1. Na sua conta do Marketo Sales, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/msi-actions-admin-guide-14.png)

1. Em Configurações de administração, selecione **Gerenciamento de usuários**.

   ![](assets/msi-actions-admin-guide-15.png)

1. Clique em **Ações** e selecione **Convidar Usuários**.

   ![](assets/msi-actions-admin-guide-16.png)

1. Insira o(s) endereço(s) de email e clique em **Convidar**.

   ![](assets/msi-actions-admin-guide-17.png)

>[!NOTE]
>
>Por padrão, todos os novos membros serão adicionados à equipe Todos.

Você receberá uma mensagem de confirmação.

## Convidar usuários via CSV para ações MSI {#invite-users-via-csv-to-msi-actions}

1. Na sua conta do Marketo Sales, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/msi-actions-admin-guide-18.png)

1. Em Configurações de administração, selecione **Gerenciamento de usuários**.

   ![](assets/msi-actions-admin-guide-19.png)

1. Clique em **Ações** e selecione **Convidar usuários via CSV**.

   ![](assets/msi-actions-admin-guide-20.png)

1. Procure o CSV no computador, selecione-o e clique em **Avançar**.

   ![](assets/msi-actions-admin-guide-21.png)

1. Confirme se os campos estão mapeados corretamente e clique em **Convidar**.

   ![](assets/msi-actions-admin-guide-22.png)

Você receberá uma mensagem de confirmação assim que os convites forem enviados.

>[!NOTE]
>
>Depois disso, você poderá atualizar seu pacote MSI existente ou instalar um novo e seguir para [configuração de Ações MSI no Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/sales-insight-actions-configuration-in-salesforce.md){target="_blank"}.
