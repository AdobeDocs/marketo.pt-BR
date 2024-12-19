---
description: Etapa 2 de 3 - Criar um usuário do Salesforce para Marketo (Enterprise/Unlimited) - Documentação do Marketo - Documentação do produto
title: Etapa 2 de 3 - Criar um usuário do Salesforce para Marketo (Enterprise/Unlimited)
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 2%

---

# Etapa 2 de 3: Criar um usuário do Salesforce para Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Essas etapas devem ser concluídas por um administrador do Salesforce

>[!PREREQUISITES]
>
>[Etapa 1 de 3: Adicionar Campos do Marketo à Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}

Neste artigo, você configurará as permissões do usuário no perfil do Salesforce e criará uma conta de integração Marketo-Salesforce.

## Criar um perfil {#create-a-profile}

1. Clique em **[!UICONTROL Instalação]**.

   CAPTURA DE TELA

1. Digite &quot;perfis&quot; na barra de pesquisa de navegação e clique no link Perfis.

   CAPTURA DE TELA

1. Clique em Novo perfil.

   CAPTURA DE TELA

1. Selecione Usuário padrão, nomeie o perfil como &quot;Sincronização Marketo-Salesforce&quot; e clique em Salvar.

   CAPTURA DE TELA

## Definir permissões de perfil {#set-profile-permissions}

1. Clique em Editar para definir as permissões de segurança.

   CAPTURA DE TELA

1. Na seção Permissões administrativas, verifique se as seguintes caixas estão marcadas:

   * API habilitada
   * Editar modelos de HTML
   * Gerenciar Documentos Públicos
   * Gerenciar modelos públicos

   >[!TIP]
   >
   >Certifique-se de marcar a caixa A senha nunca expira.

1. Na seção Permissões gerais de usuário, verifique se as seguintes caixas estão marcadas:

   * Converter clientes potenciais
   * Editar eventos
   * Editar Tarefas

1. Na seção Permissões de objeto padrão, verifique se as permissões Ler, Criar, Editar e Excluir estão marcadas para:

   * Contas
   * Campanhas
   * Contatos
   * Leads
   * Oportunidades

   >[!NOTE]
   >
   >Conceda permissões para as Campanhas, se você planeja usar a Sincronização de campanha.

   CAPTURA DE TELA

1. Quando terminar, clique em Salvar na parte inferior da página.

   CAPTURA DE TELA

## Definir permissões de campo {#set-field-permissions}

1. Converse com seus profissionais de marketing para descobrir quais campos personalizados são necessários para a sincronização.

   >[!NOTE]
   >
   >Essa etapa impedirá que campos desnecessários sejam exibidos no Marketo, o que reduzirá a desordem e acelerará a sincronização.

1. Na página de detalhes do perfil, vá para a seção Segurança em nível de campo. Clique em Exibir para editar a acessibilidade dos objetos:

   * Lead
   * Contato
   * Conta
   * Oportunidade

   >[!TIP]
   >
   >Você pode configurar outros objetos de acordo com as necessidades de sua organização.

1. Para cada objeto, clique em Editar.

   CAPTURA DE TELA

1. Localize os campos desnecessários e verifique se as opções Acesso de leitura e Acesso de edição estão desmarcadas. Clique em Salvar ao concluir.

   >[!NOTE]
   >
   >Edite somente a acessibilidade para os campos personalizados.

   CAPTURA DE TELA

1. Depois de terminar de desativar todos os campos desnecessários, você deve verificar o Acesso de leitura e o Acesso de edição para os seguintes campos de objeto. Clique em Salvar ao concluir.

   TABELA

   CAPTURA DE TELA

## Criar conta de sincronização Marketo-Salesforce {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Crie uma conta dedicada do Salesforce (por exemplo, `marketo@yourcompany.com`) para distinguir as alterações feitas pelo Marketo de outros usuários do Salesforce.

1. Digite &quot;Gerenciar usuários&quot; na barra de pesquisa de navegação e clique em Usuários. Clique em Novo usuário.

   CAPTURA DE TELA

   CAPTURA DE TELA

1. Preencha os campos obrigatórios. Em seguida, selecione a Licença de usuário: Salesforce e o Perfil criado anteriormente. Clique em Salvar ao concluir.

   CAPTURA DE TELA

A etapa 2 de 3 foi concluída.
