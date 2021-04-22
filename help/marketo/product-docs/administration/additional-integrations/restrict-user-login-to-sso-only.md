---
unique-page-id: 2360358
description: Restringir logon de usuário somente ao SSO - Documentos do Marketo - Documentação do produto
title: Login de usuário restrito apenas a SSO
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 5%

---

# Login de usuário restrito apenas a SSO {#restrict-user-login-to-sso-only}

Se você estiver [usando SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) e quiser garantir que os usuários não possam ignorar a segurança SSO, siga estas instruções.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para **Admin** e clique em **Definições de Início de Sessão**.

   ![](assets/image2014-9-24-14-3a44-3a40.png)

1. Clique em **Editar configurações de segurança**.

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. Expanda as Configurações avançadas, marque **Exigir SSO** e clique em **Salvar**.

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!NOTE]
>
>A prática recomendada é que os usuários sejam convidados e aceitem o convite. __ Depois que o convite for aceito, os administradores devem defini-los como &quot;Exigir SSO&quot;.

>[!TIP]
>
>Se você selecionar **Exigir SSO**, poderá excluir [função de usuário](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) dessa restrição marcando a opção **Ignorar logon único** ao configurar a função. Isso permitirá que os usuários façam logon normalmente. Por exemplo, os usuários administradores ainda podem precisar fazer logon no Marketo pela tela de logon.

>[!CAUTION]
>
>Quando novos usuários são convidados, eles recebem emails de convite. No entanto, se **Exigir SSO** for selecionado, eles não receberão esses emails, a menos que sejam atribuídos a uma função definida como **Ignorar logon único**.

Pronto! Agora, todos os usuários (exceto usuários com permissão para ignorar o logon único) serão restritos ao uso somente do logon SSO.

>[!MORELIKETHIS]
>
>* [Adicionar logon único a um portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Uso de uma ID universal para logon de assinatura](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Convidar usuários do Marketo para duas instâncias com ID universal](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

