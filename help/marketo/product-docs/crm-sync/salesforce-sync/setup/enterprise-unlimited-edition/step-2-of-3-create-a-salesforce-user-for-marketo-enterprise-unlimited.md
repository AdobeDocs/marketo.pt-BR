---
unique-page-id: 2360364
description: Etapa 2 de 3 - Criar um usuário do Salesforce para Marketo (Enterprise/Unlimited) - Documentação do Marketo - Documentação do produto
title: Etapa 2 de 3 - Criar um usuário do Salesforce para Marketo (Enterprise/Unlimited)
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
feature: Salesforce Integration
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 3%

---

# Etapa 2 de 3: Criar um Usuário [!DNL Salesforce] para Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Estas etapas devem ser completadas por um administrador [!DNL Salesforce]

>[!PREREQUISITES]
>
>[Etapa 1 de 3: Adicionar Campos do Marketo a [!DNL Salesforce] (Empresarial/Ilimitada)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

Neste artigo, você configurará as permissões de usuário no perfil [!DNL Salesforce] e criará uma conta de integração Marketo-[!DNL Salesforce].

## Criar um perfil {#create-a-profile}

1. Clique em **[!UICONTROL Instalação]**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Digite &quot;profiles&quot; na barra de pesquisa de navegação e clique no link **[!UICONTROL Profiles]**.

   ![](assets/sfdc-profiles-hands.png)

1. Clique em **[!UICONTROL Novo]**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Selecione **[!UICONTROL Usuário padrão]**, nomeie o perfil como &quot;Sincronização Marketo-Salesforce&quot; e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Definir permissões de perfil {#set-profile-permissions}

1. Clique em **[!UICONTROL Editar]** para definir as permissões de segurança.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. Na seção **[!UICONTROL Permissões administrativas]**, verifique se as seguintes caixas estão marcadas:

   * [!UICONTROL API Habilitada]
   * [!UICONTROL Editar Modelos do HTML]
   * [!UICONTROL Gerenciar Documentos Públicos]
   * [!UICONTROL Gerenciar Modelos Públicos]

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Certifique-se de marcar a caixa **[!UICONTROL Senha nunca expira]**.

1. Na seção [!UICONTROL Permissões gerais de usuário], verifique se as seguintes caixas estão marcadas:

   * [!UICONTROL Converter clientes em potencial]
   * [!UICONTROL Editar Eventos]
   * [!UICONTROL Editar Tarefas]

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. Na seção [!UICONTROL Permissões de Objeto Padrão], verifique se as permissões [!UICONTROL Ler, Criar, Editar e Excluir] estão marcadas para:

   * [!UICONTROL Contas]
   * [!UICONTROL Campanhas]
   * [!UICONTROL Contatos]
   * [!UICONTROL Clientes Potenciais]
   * [!UICONTROL Oportunidades]

   >[!NOTE]
   >
   >Conceda permissões para as [!UICONTROL Campanhas], se você planeja usar a Sincronização de Campanha.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Quando terminar, clique em **[!UICONTROL Salvar]** na parte inferior da página.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Definir permissões de campo {#set-field-permissions}

1. Converse com seus profissionais de marketing para descobrir quais campos personalizados são necessários para a sincronização.

   >[!NOTE]
   >
   >Essa etapa impedirá que campos desnecessários sejam exibidos no Marketo, o que reduzirá a desordem e acelerará a sincronização.

1. Na página de detalhes do perfil, vá para a seção **[!UICONTROL Segurança em Nível de Campo]**. Clique em **[!UICONTROL Exibir]** para editar a acessibilidade dos objetos:

   * [!UICONTROL Lead]
   * [!UICONTROL Contato]
   * [!UICONTROL Conta]
   * [!UICONTROL Oportunidade]

   >[!TIP]
   >
   >Você pode configurar outros objetos de acordo com as necessidades de sua organização.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Para cada objeto, clique em **[!UICONTROL Editar]**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Localize os campos desnecessários, verifique se a opção **[!UICONTROL Acesso de Leitura]** e **[!UICONTROL Editar Acesso]** está desmarcada. Clique em **[!UICONTROL Salvar]** quando terminar.

   >[!NOTE]
   >
   >Edite somente a acessibilidade para os campos personalizados.

   ![](assets/sfdc-sync-field-edit2.png)

1. Depois de concluir a desabilitação de todos os campos desnecessários, você deve verificar o **[!UICONTROL Acesso de Leitura e Acesso de Edição]** para os seguintes campos de objeto. Clique em **[!UICONTROL Salvar]** quando terminar.

<table>
 <tbody>
  <tr>
   <th>Objeto</th>
   <th>Campos</th>
  </tr>
  <tr>
   <td>Conta</td>
   <td>Campo de tipo</td>
  </tr>
  <tr>
   <td>Evento</td>
   <td>Todos os campos</td>
  </tr>
  <tr>
   <td>Tarefa</td>
   <td>Todos os campos</td>
  </tr>
 </tbody>
</table>

![](assets/sfdc-check-the-boxes.png)

## Criar conta de sincronização Marketo-Salesforce {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Crie uma conta [!DNL Salesforce] dedicada (por exemplo, marketo@yourcompany.com) para distinguir as alterações feitas pelo Marketo de outros usuários [!DNL Salesforce].

1. Digite &quot;Gerenciar usuários&quot; na barra de pesquisa de navegação e clique em **[!UICONTROL Usuários]**. Clique em **[!UICONTROL Novo Usuário]**.

   ![](assets/sfdc-new-users.png)

1. Preencha os campos obrigatórios. Em seguida, selecione a **[!UICONTROL Licença de usuário: Salesforce]** e o Perfil criado anteriormente. Clique em **[!UICONTROL Salvar]** quando terminar.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

A etapa 2 de 3 foi concluída.

>[!NOTE]
>
>[Etapa 3 de 3: Conectar o Marketo e [!DNL Salesforce] (Empresa/Ilimitado)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
