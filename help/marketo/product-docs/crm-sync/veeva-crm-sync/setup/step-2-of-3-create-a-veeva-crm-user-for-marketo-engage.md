---
description: Etapa 2 de 3 - Criar um  [!DNL Veeva] Usuário do CRM para Marketo Engage - Documentação do Marketo - Documentação do produto
title: Etapa 2 de 3 - Criar um usuário do Veeva CRM para Marketo Engage
exl-id: 78945192-36b0-4e0b-830a-f37eb0b83484
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 6%

---

# Etapa 2 de 3: Criar um Usuário do CRM do [!DNL Veeva] para Marketo Engage {#step-2-of-3-create-a-veeva-crm-user-for-marketo-engage}

>[!NOTE]
>
>As etapas deste artigo devem ser concluídas por um administrador do CRM [!DNL Veeva].

>[!PREREQUISITES]
>
>[Etapa 1 de 3: Adicionar Campos do Marketo a [!DNL Salesforce] (Profissional)](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}

Neste artigo, você personalizará permissões de campo com um Layout de Página do CRM [!DNL Veeva] e criará um usuário de sincronização do CRM [!DNL Marketo-Veeva].

## Definir Layouts de Página {#set-page-layouts}

Seguir essas etapas permitirá que o usuário de sincronização do Marketo atualize os campos personalizados.

1. Clique nos layouts de página **[!UICONTROL Conta]** (conta de pessoa) na barra de pesquisa de navegação sem pressionar Enter e clique em **[!UICONTROL Layout da página]** em [!UICONTROL Contatos].

   ![](assets/step-2-of-3-create-a-veeva-crm-user-1.png)

1. Clique em **[!UICONTROL Layouts de página]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-2.png)

1. Clique em **[!UICONTROL HCP - Profissional]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-3.png)

1. Clique e arraste uma nova **[!UICONTROL Seção]** para o layout da página.

1. Insira &quot;Marketo&quot; para **[!UICONTROL Nome da Seção]** e clique em **[!UICONTROL OK]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-4.png)

1. Clique e arraste o campo **[!UICONTROL Pontuação]** para a seção Marketo.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-5.png)

1. Repita a etapa acima para os seguintes campos:

   * Cidade indicada
   * Empresa indicada
   * País indicado
   * Área metropolitana indicada
   * Código de área telef. indic.
   * Código postal indicado
   * Estado/região indicado

   >[!NOTE]
   >
   >Esses campos precisam estar no layout da página para que o Marketo possa ler/gravar neles.

   >[!TIP]
   >
   >Crie duas colunas para os campos arrastando para o lado direito da página. Você pode mover campos de um lado para o outro para equilibrar os comprimentos de coluna.

1. Quando terminar com o Layout do [!UICONTROL HCP-Profissional], clique em **[!UICONTROL Salvar]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-6.png)

>[!NOTE]
>
>Repita isso para outros Layouts de página da [!UICONTROL Conta].

## Criar um perfil {#create-a-profile}

1. Clique em **[!UICONTROL Instalação]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-7.png)

1. Digite &quot;perfis&quot; na barra de pesquisa de navegação e clique no link **[!UICONTROL Perfis]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-8.png)

1. Clique em **[!UICONTROL Novo]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-9.png)

1. Selecione **[!UICONTROL Usuário padrão]**, nomeie o perfil como &quot;[!UICONTROL Sincronização Marketo-Salesforce]&quot; e clique em **[!UICONTROL Salvar]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-10.png)

## Definir permissões de perfil {#set-profile-permissions}

1. Clique em **[!UICONTROL Editar]** para definir as permissões de segurança.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-11.png)

1. Na seção [!UICONTROL Permissões administrativas], verifique se [!UICONTROL API Habilitada] está selecionado.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-12.png)

   >[!TIP]
   >
   >Certifique-se de marcar a caixa [!UICONTROL Senha nunca expira].

1. Na seção [!UICONTROL Permissões gerais de usuário], verifique se [!UICONTROL Editar eventos] e [!UICONTROL Editar tarefas] estão selecionados.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-13.png)

1. Na seção [!UICONTROL Permissões de Objeto Padrão], verifique se as permissões [!UICONTROL Leitura], [!UICONTROL Criação], [!UICONTROL Edição] e [!UICONTROL Exclusão] estão verificadas em busca de [!UICONTROL Contas] e [!UICONTROL Contatos].

   ![](assets/step-2-of-3-create-a-veeva-crm-user-14.png)

1. Na seção [!UICONTROL Permissões de Objeto Personalizado], verifique se as permissões [!UICONTROL Leitura] estão verificadas para [!UICONTROL Chamada], [!UICONTROL Mensagem de Chave de Chamada] e quaisquer outros Objetos Personalizados desejados.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-15.png)

1. Quando terminar, clique em **[!UICONTROL Salvar]** na parte inferior da página.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-16.png)

## Definir permissões de campo {#set-field-permissions}

1. Converse com seus profissionais de marketing para descobrir quais campos personalizados são necessários para a sincronização.

   >[!NOTE]
   >
   >Essa etapa impedirá que campos desnecessários sejam exibidos no Marketo, o que reduzirá a desordem e acelerará a sincronização.

1. Na página [!UICONTROL detalhes do perfil], vá para a seção **[!UICONTROL Segurança de Nível de Campo]**. Clique em **[!UICONTROL Exibir]** para editar a acessibilidade dos objetos [!UICONTROL Contato] e [!UICONTROL Conta].

   ![](assets/step-2-of-3-create-a-veeva-crm-user-17.png)

   >[!TIP]
   >
   >Você pode configurar outros objetos de acordo com as necessidades de sua organização.

1. Para cada objeto, clique em **[!UICONTROL Editar]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-18.png)

Localize os campos desnecessários, verifique se o [!UICONTROL Acesso de Leitura] e o [!UICONTROL Acesso de Edição] estão **un** marcados. Clique em **[!UICONTROL Salvar]** quando terminar.

![](assets/step-2-of-3-create-a-veeva-crm-user-19.png)

>[!NOTE]
>
>Edite somente a acessibilidade para os campos personalizados.

1. Depois que você terminar de desabilitar todos os campos desnecessários, marque o [!UICONTROL Acesso de Leitura] e o [!UICONTROL Acesso de Edição] para os seguintes campos de objeto. Clique em **[!UICONTROL Salvar]** quando terminar.

<table>
 <tbody>
  <tr>
   <th>Objeto
   <th>Campos
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

## Criar usuário de sincronização {#create-sync-user}

O Marketo requer credenciais para acessar o CRM [!DNL Veeva]. Isso é melhor feito com um usuário dedicado criado com as etapas abaixo.

>[!NOTE]
>
>Se sua organização não tiver [!DNL Veeva] licenças adicionais do CRM, você poderá usar um usuário de Marketing existente com o perfil de Administrador do Sistema.

1. Insira &quot;usuários&quot; na barra de pesquisa de Navegação e clique em **[!UICONTROL Usuários]** em [!UICONTROL Gerenciar usuários].

   ![](assets/step-2-of-3-create-a-veeva-crm-user-20.png)

1. Clique em **[!UICONTROL Novo Usuário]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-21.png)

1. Preencha os campos obrigatórios, selecione a **[!UICONTROL Licença de Usuário]**: **[!UICONTROL Salesforce]**, defina o **[!UICONTROL Perfil]**: **[!UICONTROL Marketo Sync]** Usuário e clique em **[!UICONTROL Salvar]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-22.png)

>[!TIP]
>
>Verifique se o endereço de email inserido é válido. Você precisará fazer logon como o usuário de sincronização para redefinir a senha.

Excelente! Agora você tem uma conta que a Marketo Engage pode usar para se conectar ao CRM [!DNL Veeva]. Vamos fazer isso.

>[!MORELIKETHIS]
>
>[Etapa 3 de 3: Conectar o Marketo e [!DNL Veeva] CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-3-of-3-connect-marketo-engage-and-veeva-crm.md){target="_blank"}
