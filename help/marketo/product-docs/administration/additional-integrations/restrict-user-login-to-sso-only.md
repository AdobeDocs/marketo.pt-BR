---
unique-page-id: 2360358
description: Restringir o logon do usuário somente para SSO - Documentos de marketing - Documentação do produto
title: Restringir logon de usuário somente para SSO
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# Restringir logon de usuário somente para SSO {#restrict-user-login-to-sso-only}

Se você estiver [usando SSO](add-single-sign-on-to-a-portal.md) e quiser garantir que os usuários não possam ignorar a segurança SSO, siga estas instruções.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para **Admin** e clique em **Definições de Início de Sessão**.

![](assets/image2014-9-24-14-3a44-3a40.png)

1. Clique em **Editar configurações de segurança**.

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. Expanda as configurações avançadas, marque **Exigir SSO** e clique em **Salvar**.

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!TIP]
>
>Se você selecionar **Exigir SSO**, poderá excluir uma [função de usuário](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) desta restrição, marcando a opção **Ignorar logon único** ao configurar a função. Isso permitirá que os usuários façam logon normalmente. Por exemplo, os usuários administradores ainda podem precisar fazer logon no Marketo pela tela de logon.

>[!CAUTION]
>
>Quando novos usuários são convidados, eles recebem e-mails de convite. Entretanto, se **Exigir SSO** for selecionado, eles não receberão esses emails, a menos que sejam atribuídos a uma função definida como **Ignorar logon único**.

É isso! Agora, todos os usuários (exceto os usuários com permissão para ignorar o logon único) estarão restritos ao uso apenas do logon SSO.
