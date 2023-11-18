---
unique-page-id: 2360364
description: Etapa 2 de 3 - Criar um usuário do Salesforce para Marketo (Enterprise/Unlimited) - Documentação do Marketo - Documentação do produto
title: Etapa 2 de 3 - Criar um usuário do Salesforce para Marketo (Enterprise/Unlimited)
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 4%

---

# Etapa 2 de 3: Criar um usuário do Salesforce para Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Essas etapas devem ser concluídas por um administrador do Salesforce

>[!PREREQUISITES]
>
>[Etapa 1 de 3: Adicionar campos do Marketo ao Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}

Neste artigo, você configurará as permissões do usuário no perfil do Salesforce e criará uma conta de integração Marketo-Salesforce.

## Criar um perfil {#create-a-profile}

1. Clique em **[!UICONTROL Configuração]**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Digite &quot;perfis&quot; na barra de pesquisa de navegação e clique no link **[!UICONTROL Perfis]** link.

   ![](assets/sfdc-profiles-hands.png)

1. Clique em **[!UICONTROL Novo]**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Selecionar **[!UICONTROL Usuário padrão]**, nomeie o perfil como &quot;Marketo-Salesforce Sync&quot; e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Definir permissões de perfil {#set-profile-permissions}

1. Clique em **[!UICONTROL Editar]** para definir as permissões de segurança.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. No **[!UICONTROL Permissões administrativas]** verifique se as seguintes caixas estão marcadas:

   * API habilitada
   * Editar modelos de HTML
   * Gerenciar Documentos Públicos
   * Gerenciar modelos públicos

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Certifique-se de verificar a **[!UICONTROL A senha nunca expira]** caixa.

1. Na seção Permissões gerais de usuário, verifique se as seguintes caixas estão marcadas:

   * Converter clientes potenciais
   * Editar eventos
   * Editar Tarefas

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. Na seção Permissões de objeto padrão, verifique se as permissões Ler, Criar, Editar e Excluir estão marcadas para:

   * Contas
   * Campanhas
   * Contatos
   * Leads
   * Oportunidades

   >[!NOTE]
   >
   >Conceda permissões para as Campanhas, se você planeja usar a Sincronização de campanha.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Quando terminar, clique em **[!UICONTROL Salvar]** na parte inferior da página.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Definir permissões de campo {#set-field-permissions}

1. Converse com seus profissionais de marketing para descobrir quais campos personalizados são necessários para a sincronização.

   >[!NOTE]
   >
   >Essa etapa impedirá que campos desnecessários sejam exibidos no Marketo, o que reduzirá a desordem e acelerará a sincronização.

1. Na página de detalhes do perfil, acesse **[!UICONTROL Segurança em nível de campo]** seção. Clique em **[!UICONTROL Exibir]** para editar a acessibilidade dos objetos:

   * Lead
   * Contato
   * Conta
   * Oportunidade

   >[!TIP]
   >
   >Você pode configurar outros objetos de acordo com as necessidades de sua organização.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Para cada objeto, clique em **[!UICONTROL Editar]**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Localize os campos desnecessários, verifique se **[!UICONTROL Acesso de leitura]** e **[!UICONTROL Editar Acesso]** estão desmarcadas. Clique em **[!UICONTROL Salvar]** quando terminar.

   >[!NOTE]
   >
   >Edite somente a acessibilidade para os campos personalizados.

   ![](assets/sfdc-sync-field-edit2.png)

1. Depois de terminar de desabilitar todos os campos desnecessários, você deve marcar **[!UICONTROL Acesso de leitura e acesso de edição]** para os seguintes campos de objeto. Clique em **[!UICONTROL Salvar]** quando terminar.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1"><p>Objeto</p></th> 
   <th colspan="1" rowspan="1"><p>Campos</p></th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Conta</p></td> 
   <td colspan="1" rowspan="1"><p>Campo de tipo</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Evento</p></td> 
   <td colspan="1" rowspan="1"><p>Todos os campos</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Tarefa</p></td> 
   <td colspan="1" rowspan="1"><p>Todos os campos</p></td> 
  </tr> 
 </tbody> 
</table>

![](assets/sfdc-check-the-boxes.png)

## Criar conta de sincronização do Marketo-Salesforce {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Crie uma conta dedicada do Salesforce (por exemplo, `marketo@yourcompany.com`) para distinguir as alterações feitas pelo Marketo de outros usuários do Salesforce.

1. Digite &quot;Gerenciar usuários&quot; na barra de pesquisa de navegação e clique em **[!UICONTROL Usuários]**. Clique em **[!UICONTROL Novo usuário]**.

   ![](assets/sfdc-new-users.png)

1. Preencha os campos obrigatórios. Em seguida, selecione o **[!UICONTROL Licença de usuário: Salesforce]** e o Perfil criado anteriormente. Clique em **[!UICONTROL Salvar]** quando terminar.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

A etapa 2 de 2 foi concluída.

>[!NOTE]
>
>[Etapa 3 de 3: Conectar o Marketo e o Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md){target="_blank"}
