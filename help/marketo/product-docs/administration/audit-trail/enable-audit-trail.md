---
unique-page-id: 11382122
description: Ativar trilha de auditoria - Documentos do Marketo - Documentação do produto
title: Ativar Trilha de Auditoria
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Habilitar Trilha de Auditoria {#enable-audit-trail}

A trilha de auditoria está disponível para todos os clientes e é controlada por duas permissões de administrador.

>[!NOTE]
>
>Por padrão, todas as funções de administrador do sistema têm as duas permissões habilitadas.

## Habilitar Trilha de Auditoria para uma Função {#enable-audit-trail-for-a-role}

1. Clique em **Admin**.

   ![](assets/one-2.png)

1. Selecione **Usuários e funções** e clique em **Funções**.

   ![](assets/two-2.png)

1. Selecione a função para a qual deseja habilitar a Trilha de Auditoria e clique em **Editar Função**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Você também tem a opção aqui para criar uma nova função e conceder a ela acesso à Trilha de auditoria.

1. Expanda a permissão **Acessar o administrador**. Selecione **Access Audit Trail** e/ou **Access Login History**, dependendo das suas necessidades. Clique em **Salvar**.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >**Definição**
   >
   >**Trilha de auditoria de acesso:** concede aos usuários acesso à trilha de auditoria de ativos e à trilha de auditoria de administração.
   >
   >**Histórico de logon de acesso:** concede aos usuários acesso ao Histórico de logon  [do usuário](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## Atribuir a função de trilha de auditoria a um usuário {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) Crie ou  [](#enable-audit-trail) ative uma função existente, dando a ela permissões de Trilha de auditoria.

1. Em **Usuários e funções**, clique em **Usuários**.

   ![](assets/five-1.png)

1. Selecione o usuário ao qual deseja conceder acesso à Trilha de Auditoria e clique em **Editar Usuário**.

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >Esse processo também se aplica quando você está criando um novo usuário.

1. Selecione as funções da Trilha de Auditoria que você criou. Neste exemplo, criamos &quot;Trilha de auditoria - Ativo e administrador&quot; e &quot;Trilha de auditoria - com histórico de logon&quot;.

   ![](assets/seven-1.png)

   >[!CAUTION]
   >
   >Se você tiver espaços de trabalho ativados, marque a caixa de seleção da função, que seleciona todos os espaços de trabalho. Desmarcar um espaço de trabalho individual ocultará a Trilha de auditoria. Isso significa que você verá os dados da Trilha de auditoria para cada espaço de trabalho. Você tem a opção de ocultar espaços de trabalho quando [filtering](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. Clique em **Salvar**.

   ![](assets/eight-1.png)
