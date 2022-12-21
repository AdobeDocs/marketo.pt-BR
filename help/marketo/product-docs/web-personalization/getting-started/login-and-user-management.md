---
unique-page-id: 7513771
description: Gerenciamento de logon e do usuário - Documentação da Marketo - Documentação do produto
title: Gerenciamento de logon e de usuários
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Gerenciamento de logon e de usuários {#login-and-user-management}

## Criar uma função de usuário de personalização da Web {#create-a-web-personalization-user-role}

1. Vá para o **Administrador** e, em seguida, clique em **Usuários e funções**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Clique em **Funções**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Se a função de usuário de Personalização da Web (WP) já existir, verifique se ela está configurada como mostrado na Etapa 4.

1. Clique em **Nova função**.

   ![](assets/three-1.png)

1. Insira um Nome de função e selecione Permissões. Clique em **Criar** (esta função deve [aplicar a todos os espaços de trabalho](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)).

   ![](assets/four.png)

   >[!TIP]
   >
   >Para conceder aos usuários permissão de acesso a tudo em Direcionamento e personalização, selecione _all_ as caixas de seleção.

## Personalização da Web e permissões de usuário de conteúdo preditivo {#web-personalization-and-predictive-content-user-permissions}

**Direcionamento e personalização**: O usuário só tem permissões de exibição, se essa permissão estiver selecionada.

**Personalização da Web do administrador + Predictive**: O usuário tem acesso somente às Configurações da conta e às Configurações de conteúdo para o aplicativo Personalização da Web e Conteúdo preditivo . Os usuários podem exibir páginas no aplicativo, mas não têm permissões para criar, editar, excluir e iniciar.

**Editor de conteúdo preditivo**: O usuário tem acesso de editor ao aplicativo de Conteúdo preditivo. A permissão permite criar, editar, excluir partes de conteúdo. Ela não permite ativar o conteúdo para uso preditivo na Web ou no email.

**Iniciador de conteúdo preditivo**: O usuário tem acesso a todos os recursos de Conteúdo preditivo, exceto Configurações de conta e conteúdo. A permissão permite criar, editar, excluir e ativar partes de conteúdo.

**Editor de Campanha Web**: O usuário tem acesso de editor a todos os recursos de Personalização da Web para criar, editar e excluir, mas não iniciar campanhas da Web.

**Iniciador de campanha da Web**: O usuário tem acesso a todos os recursos do aplicativo de Personalização da Web, exceto Configurações de conta e conteúdo. A permissão permite criar, editar, excluir e iniciar campanhas da Web.

## Atribuir função WP ao usuário {#assign-wp-role-to-user}

1. Ir para **Usuários**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Selecione o usuário ao qual conceder acesso ao WP e clique em **Editar usuário**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Selecione a função de usuário WP para todos os espaços de trabalho.

   ![](assets/seven.png)

1. Os usuários recém-habilitados verão a variável **Personalização da Web** em Meu Marketo na próxima vez que fizerem logon.

   ![](assets/eight.png)
