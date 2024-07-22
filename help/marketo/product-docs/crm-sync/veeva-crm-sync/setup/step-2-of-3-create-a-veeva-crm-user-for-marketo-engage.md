---
description: Etapa 2 de 3 - Criar um usuário do Veeva CRM para Marketo Engage - Documentação do Marketo - Documentação do produto
title: Etapa 2 de 3 - Criar um usuário do Veeva CRM para Marketo Engage
exl-id: 78945192-36b0-4e0b-830a-f37eb0b83484
feature: Veeva CRM
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 6%

---

# Etapa 2 de 3: Criar um usuário do Veeva CRM para Marketo Engage {#step-2-of-3-create-a-veeva-crm-user-for-marketo-engage}

>[!NOTE]
>
>As etapas deste artigo devem ser concluídas por um administrador do Veeva CRM.

>[!PREREQUISITES]
>
>[Etapa 1 de 3: Adicionar campos do Marketo ao Salesforce (Professional)](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}

Neste artigo, você personalizará permissões de campo com um Layout de página do Veeva CRM e criará um usuário de sincronização do Marketo-Veeva CRM.

## Definir Layouts de Página {#set-page-layouts}

Seguir essas etapas permitirá que o usuário de sincronização do Marketo atualize os campos personalizados.

1. Clique nos layouts de página Conta (conta de pessoa) na barra de pesquisa de navegação sem pressionar Enter e clique em **[!UICONTROL Layout da página]** em Contatos.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-1.png)

1. Clique em **[!UICONTROL Layouts de página]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-2.png)

1. Clique em **[!UICONTROL HCP - Profissional]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-3.png)

1. Clique e arraste uma nova **[!UICONTROL Seção]** para o layout da página.

1. Digite &quot;Marketo&quot; para o Nome da Seção e clique em **[!UICONTROL OK]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-4.png)

1. Clique e arraste o campo Score para a seção Marketo.

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

1. Quando terminar com o Layout HCP-Profissional, clique em **[!UICONTROL Salvar]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-6.png)

   >[!NOTE]
   >
   >Repita isso para outros Layouts de página da conta.

## Criar um perfil {#create-a-profile}

1. Clique em **[!UICONTROL Instalação]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-7.png)

1. Digite &quot;perfis&quot; na barra de pesquisa de navegação e clique no link **[!UICONTROL Perfis]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-8.png)

1. Clique em **[!UICONTROL Novo]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-9.png)

1. Selecione Usuário padrão, nomeie o perfil como &quot;Sincronização do Marketo-Salesforce&quot; e clique em **[!UICONTROL Salvar]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-10.png)

## Definir permissões de perfil {#set-profile-permissions}

1. Clique em **[!UICONTROL Editar]** para definir as permissões de segurança.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-11.png)

1. Na seção Permissões administrativas, verifique se **[!UICONTROL API Habilitada]** está selecionado.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-12.png)

   >[!TIP]
   >
   >Certifique-se de marcar a caixa A senha nunca expira.

1. Na seção Permissões gerais de usuário, verifique se **[!UICONTROL Editar eventos]** e **[!UICONTROL Editar tarefas]** estão selecionados.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-13.png)

1. Na seção Permissões de Objeto Padrão, verifique se as permissões de **[!UICONTROL Leitura]**, **[!UICONTROL Criação]**, **[!UICONTROL Edição]** e **[!UICONTROL Exclusão]** estão verificadas em busca de Contas e Contatos.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-14.png)

1. Na seção Permissões de objeto personalizado, verifique se as permissões de leitura estão verificadas para **[!UICONTROL Chamada]**, **[!UICONTROL Mensagem da chave de chamada]** e quaisquer outros Objetos personalizados desejados.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-15.png)

1. Quando terminar, clique em **[!UICONTROL Salvar]** na parte inferior da página.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-16.png)

## Definir permissões de campo {#set-field-permissions}

1. Converse com seus profissionais de marketing para descobrir quais campos personalizados são necessários para a sincronização.

   >[!NOTE]
   >
   >Essa etapa impedirá que campos desnecessários sejam exibidos no Marketo, o que reduzirá a desordem e acelerará a sincronização.

1. Na página de detalhes do perfil, vá para a seção [!UICONTROL Segurança em Nível de Campo]. Clique em **[!UICONTROL Exibir]** para editar a acessibilidade dos objetos Contato e Conta.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-17.png)

   >[!TIP]
   >
   >Você pode configurar outros objetos de acordo com as necessidades de sua organização.

1. Para cada objeto, clique em **[!UICONTROL Editar]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-18.png)

1. Localize os campos desnecessários, verifique se Acesso de Leitura e Acesso de Edição estão _desmarcados_. Clique em **[!UICONTROL Salvar]** quando terminar.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-19.png)

   >[!NOTE]
   >
   >Edite somente a acessibilidade para os campos personalizados.

1. Depois de terminar de desativar todos os campos desnecessários, marque Acesso de leitura e Acesso de edição para os seguintes campos de objeto. Clique em **[!UICONTROL Salvar]** quando terminar.

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

O Marketo requer credenciais para acessar o Veeva CRM. Isso é melhor feito com um usuário dedicado criado com as etapas abaixo.

>[!NOTE]
>
>Se sua organização não tiver licenças adicionais do Veeva CRM, você poderá usar um usuário de Marketing existente com o perfil de Administrador do sistema.

1. Digite &quot;usuários&quot; na barra de pesquisa de Navegação e clique em **[!UICONTROL Usuários]** em Gerenciar usuários.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-20.png)

1. Clique em **[!UICONTROL Novo Usuário]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-21.png)

1. Preencha os campos obrigatórios, selecione a Licença de usuário: Salesforce, defina o Perfil: Usuário de sincronização do Marketo e clique em **[!UICONTROL Salvar]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-22.png)

>[!TIP]
>
>Verifique se o endereço de email inserido é válido. Você precisará fazer logon como o usuário de sincronização para redefinir a senha.

Excelente! Agora você tem uma conta que o Marketo Engage pode usar para se conectar ao Veeva CRM. Vamos fazer isso.

>[!MORELIKETHIS]
>
>[Etapa 3 de 3: Conectar Marketo e Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-3-of-3-connect-marketo-engage-and-veeva-crm.md){target="_blank"}
