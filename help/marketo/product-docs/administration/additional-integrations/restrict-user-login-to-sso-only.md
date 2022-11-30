---
unique-page-id: 2360358
description: Restringir logon de usuário somente ao SSO - Documentos do Marketo - Documentação do produto
title: Login de usuário restrito apenas a SSO
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 5%

---

# Login de usuário restrito apenas a SSO {#restrict-user-login-to-sso-only}

Se você estiver [usando SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) e deseja garantir que os usuários não possam ignorar a segurança do SSO, siga estas instruções.

>[!IMPORTANT]
>
>Este artigo não se aplica a [Habilitado para Adobe IMS](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md) Assinaturas da Marketo.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para o **Administrador** área.

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. Clique em **Configurações de logon**.

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. Clique em **Editar configurações de segurança**.

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. Expanda as configurações avançadas, marque **Exigir SSO** e clique em **Salvar**.

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>A prática recomendada é que os usuários sejam convidados e aceitem o convite. _Depois_ se o convite for aceito, os administradores devem defini-los como &quot;Exigir SSO&quot;.

>[!TIP]
>
>Se você selecionar **Exigir SSO**, você pode excluir um [função de usuário](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) desta restrição, verificando a **Ignorar logon único** durante a configuração da função. Isso permitirá que os usuários façam logon normalmente. Por exemplo, os usuários administradores ainda podem precisar fazer logon no Marketo pela tela de logon.

>[!CAUTION]
>
>Quando novos usuários são convidados, eles recebem emails de convite. No entanto, se **Exigir SSO** for selecionado, eles não receberão esses emails, a menos que sejam atribuídos a uma função definida como **Ignorar logon único**.

Pronto! Agora, todos os usuários (exceto usuários com permissão para ignorar o logon único) serão restritos ao uso somente do logon SSO.

>[!MORELIKETHIS]
>
>* [Adicionar logon único a um portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Uso de uma ID universal para logon de assinatura](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Convidar usuários do Marketo para duas instâncias com ID universal](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

