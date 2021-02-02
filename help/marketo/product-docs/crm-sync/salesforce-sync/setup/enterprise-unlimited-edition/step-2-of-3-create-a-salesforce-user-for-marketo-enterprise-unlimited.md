---
unique-page-id: 2360364
description: Etapa 2 de 3 - Criar um usuário do Salesforce para o Marketing (Enterprise/Unlimited) - Documentação do produto - Documentação do produto
title: Etapa 2 de 3 - Criar um usuário do Salesforce para o Marketing (Enterprise/Unlimited)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---


# Etapa 2 de 3: Criar um usuário do Salesforce para o Marketing (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Essas etapas devem ser concluídas por um administrador do Salesforce

>[!PREREQUISITES]
>
>[Etapa 1 de 3: Adicionar campos de marketing ao Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

Neste artigo, você configurará permissões de usuário no perfil Salesforce e criará uma conta de integração do Marketing-Salesforce.

## Criar um Perfil {#create-a-profile}

1. Clique em **Configuração**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Digite &quot;perfis&quot; na barra de pesquisa Navegador e clique no link **Perfis**.

   ![](assets/sfdc-profiles-hands.png)

1. Clique em **Novo**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Selecione **Usuário Padrão**, nomeie o perfil como &quot;Sincronização de Marketo-Salesforce&quot; e clique em **Salvar**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Definir permissões de Perfil {#set-profile-permissions}

1. Clique em **Editar** para definir as permissões de segurança.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. Na seção **Permissões administrativas**, verifique se as seguintes caixas estão marcadas:

   * API ativada
   * Editar modelos HTML
   * Gerenciar Documentos públicos
   * Gerenciar modelos públicos

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Certifique-se de marcar a caixa **Senha Nunca expira**.

1. Na seção Permissões gerais de usuário, verifique se as seguintes caixas estão marcadas:

   * Converter clientes em potencial
   * Editar Eventos
   * Editar Tarefas

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. Na seção Permissões de objeto padrão, verifique se as permissões de Leitura, Criação, Edição e Exclusão estão marcadas para:

   * Contas
   * Campanhas
   * Contatos
   * Clientes potenciais
   * Oportunidades

   >[!NOTE]
   >
   >Conceda permissões para as Campanhas, se planeja usar a Sincronização de Campanhas.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Quando terminar, clique em **Salvar** na parte inferior da página.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Definir permissões de campo {#set-field-permissions}

1. Converse com seus comerciantes para descobrir quais campos personalizados são necessários para sincronizar.

   >[!NOTE]
   >
   >Esta etapa evitará que os campos que você não precisa sejam exibidos no Marketo, o que reduzirá a desorganização e agilizará a sincronização.

1. Na página de detalhes do perfil, vá para a seção **Segurança no nível do campo**. Clique em **Visualização** para editar a acessibilidade dos objetos:

   * Chumbo
   * Contato
   * Conta
   * Oportunidade

   >[!TIP]
   >
   >Você pode configurar outros objetos de acordo com as necessidades de sua organização.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Para cada objeto, clique em **Editar**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Localize os campos desnecessários, verifique se **Acesso de leitura** e **Editar acesso** estão desmarcados. Clique em **Salvar** quando terminar.

   >[!NOTE]
   >
   >Edite somente a acessibilidade para os campos personalizados.

   ![](assets/sfdc-sync-field-edit2.png)

1. Depois de desabilitar todos os campos desnecessários, você deve verificar **Acesso de leitura e Editar acesso** para os seguintes campos de objeto. Clique em **Salvar** quando terminar.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1"><p>Objeto</p></th> 
   <th colspan="1" rowspan="1"><p>Campos</p></th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Conta</p></td> 
   <td colspan="1" rowspan="1"><p>Campo Tipo</p></td> 
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

## Criar conta de sincronização do Marketing para Salesforce {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Crie uma conta do Salesforce dedicada (por exemplo, marketo@yourcompany.com) para distinguir as alterações feitas pelo Marketing versus outros usuários do Salesforce.

1. Digite &quot;Gerenciar usuários&quot; na barra de pesquisa Navegador e clique em **Usuários**. Clique em **Novo usuário**.

   ![](assets/sfdc-new-users.png)

1. Preencha os campos obrigatórios. Em seguida, selecione a **Licença de usuário: Salesforce** e o Perfil criado anteriormente. Clique em **Salvar** quando terminar.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

A etapa 2 de 2 é concluída.

>[!NOTE]
>
>[Etapa 3 de 3: Connect Marketing e Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
