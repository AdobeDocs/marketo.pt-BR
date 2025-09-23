---
unique-page-id: 11382122
description: Ativar trilha de auditoria — Documentação do Marketo — Documentação do produto
title: Habilitar trilha de auditoria
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
feature: Audit Trail
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 4%

---

# Habilitar trilha de auditoria {#enable-audit-trail}

A Trilha de auditoria está disponível para todos os clientes e é controlada por duas permissões de administrador.

>[!NOTE]
>
>Por padrão, todas as funções de administrador do sistema têm ambas as permissões ativadas.

## Ativar trilha de auditoria para uma função {#enable-audit-trail-for-a-role}

1. Clique em **[!UICONTROL Administrador]**.

   ![](assets/enable-audit-trail-1.png)

1. Selecione **[!UICONTROL Usuários e funções]** e clique em **[!UICONTROL Funções]**.

   ![](assets/enable-audit-trail-2.png)

1. Selecione a função para a qual você deseja habilitar a Trilha de Auditoria e clique em **[!UICONTROL Editar Função]**.

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >Você também tem a opção aqui de criar uma nova função e conceder a ela acesso à Trilha de auditoria.

1. Expanda a permissão **[!UICONTROL Acessar Administrador]**. Selecione **[!UICONTROL Acessar trilha de auditoria]** e/ou **[!UICONTROL Acessar histórico de logon]**, dependendo das suas necessidades. Clique em **[!UICONTROL Salvar]**.

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**Definição**
   >
   >**[!UICONTROL Trilha de Auditoria de Acesso]**: Dá aos usuários acesso à [!UICONTROL Trilha de Auditoria de Ativos] e à [!UICONTROL Trilha de Auditoria de Admin].
   >
   >**[!UICONTROL Acessar Histórico de Logon]**: Dá aos usuários acesso ao [Histórico de Logon do Usuário](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## Atribuir função de trilha de auditoria a um usuário {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[Crie](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) ou [habilite](#enable-audit-trail) uma função existente, concedendo a ela permissões de Trilha de Auditoria.

1. Em **[!UICONTROL Usuários e funções]**, clique em **[!UICONTROL Usuários]**.

   ![](assets/enable-audit-trail-5.png)

1. Selecione o usuário ao qual você deseja conceder acesso ao registro de auditoria e clique em **[!UICONTROL Editar usuário]**.

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >Esse processo também se aplica quando você está criando um novo usuário.

1. Selecione as funções de trilha de auditoria que você criou. Neste exemplo, criamos &quot;Trilha de auditoria - Ativo e administrador&quot; e &quot;Trilha de auditoria - Com histórico de logon&quot;.

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >Se você tiver espaços de trabalho ativados, certifique-se de marcar a caixa de seleção da atribuição, que seleciona todos os espaços de trabalho. Desmarcar um espaço de trabalho individual ocultará a Trilha de auditoria. Isso significa que você verá os dados da Trilha de auditoria para cada espaço de trabalho. Você tem a opção de ocultar espaços de trabalho ao [filtrar](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/enable-audit-trail-8.png)
