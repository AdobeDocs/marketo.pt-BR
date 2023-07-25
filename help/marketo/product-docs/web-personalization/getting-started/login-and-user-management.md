---
unique-page-id: 7513771
description: Gerenciamento de logon e usuários - Documentação do Marketo - Documentação do produto
title: Gerenciamento de logon e usuários
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Gerenciamento de logon e usuários {#login-and-user-management}

## Criar uma função de usuário de personalização da Web {#create-a-web-personalization-user-role}

1. Vá para a **Admin** e clique em **Usuários e funções**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Clique em **Funções**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Se a função de usuário Web Personalization (WP) já existir, verifique se ela está configurada como mostrado na Etapa 4.

1. Clique em **Nova Função**.

   ![](assets/three-1.png)

1. Insira um Nome de função e selecione Permissões. Clique em **Criar** (esta função deve [aplicar a todos os espaços de trabalho](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)).

   ![](assets/four.png)

   >[!TIP]
   >
   >Para conceder aos usuários permissão para acessar tudo no Target e na Personalização, selecione _all_ as caixas de seleção.

## Personalização da Web e permissões de usuário de conteúdo preditivo {#web-personalization-and-predictive-content-user-permissions}

**Direcionamento e personalização**: o usuário tem permissões somente para visualização, caso essa permissão esteja selecionada.

**Personalização da Web do administrador + Predictive**: o usuário tem acesso somente às Configurações da conta e às Configurações de conteúdo para o aplicativo Personalização da Web e Conteúdo preditivo. Os usuários podem visualizar páginas no aplicativo, mas não têm permissões para criar, editar, excluir, iniciar.

**Editor de conteúdo preditivo**: o usuário tem acesso de editor ao aplicativo Conteúdo preditivo. A permissão permite criar, editar e excluir partes de conteúdo. Ele não permite ativar o conteúdo para uso preditivo na Web ou por email.

**Iniciador de conteúdo preditivo**: o usuário tem acesso a todos os recursos de Conteúdo preditivo, exceto Configurações de conta e conteúdo. A permissão permite criar, editar e excluir e ativar partes de conteúdo.

**Editor de campanha da Web**: o usuário tem acesso de editor a todos os recursos de Personalização da Web para criar, editar e excluir, mas não iniciar campanhas da Web.

**Iniciador da campanha da Web**: o usuário tem acesso a todos os recursos do aplicativo de Personalização da Web, exceto Configurações de conta e conteúdo. A permissão permite criar, editar, excluir e iniciar campanhas da Web.

## Atribuir Função WP ao Usuário {#assign-wp-role-to-user}

1. Ir para **Usuários**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Selecione o usuário ao qual conceder acesso de WP e clique em **Editar Usuário**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Selecione a função de usuário WP para todos os espaços de trabalho.

   ![](assets/seven.png)

1. Os usuários recém-ativados verão a variável **Personalização da Web** lado a lado em Meu Marketo na próxima vez que fizerem logon.

   ![](assets/eight.png)
