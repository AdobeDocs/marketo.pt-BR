---
unique-page-id: 2360358
description: Restringir o logon do usuário somente ao SSO - Documentação do Marketo - Documentação do produto
title: Login de usuário restrito apenas a SSO
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
source-git-commit: 1f10e1fcdbd5cf91481f749236fd37050ade29f8
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 5%

---

# Login de usuário restrito apenas a SSO {#restrict-user-login-to-sso-only}

Se você estiver [uso do SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) e quiser garantir que os usuários não possam ignorar a segurança de SSO, siga estas instruções.

>[!IMPORTANT]
>
>Este artigo não se aplica a [Habilitado para Adobe IMS](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md) Assinaturas do Marketo.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. Clique em **[!UICONTROL Configuração de logon]s**.

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. Clique em **[!UICONTROL Editar Configurações de Segurança]**.

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. Expanda a **[!UICONTROL Avançado]** configurações, marque **[!UICONTROL Exigir SSO]** e clique em **[!UICONTROL Salvar]**.

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>A prática recomendada é que os usuários sejam convidados e aceitem o convite. _Depois_ Se o convite for aceito, os administradores deverão defini-los como &quot;[!UICONTROL Exigir SSO].&quot;

>[!TIP]
>
>Se você selecionar **[!UICONTROL Exigir SSO]**, você pode excluir um [função do usuário](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) dessa restrição verificando o **[!UICONTROL Ignorar Logon Único]** durante a configuração da função. Isso permitirá que os usuários façam logon normalmente. Por exemplo, os usuários administradores ainda podem precisar fazer logon no Marketo por meio da tela de logon.

>[!CAUTION]
>
>Quando novos usuários são convidados, eles recebem emails de convite. No entanto, se **[!UICONTROL Exigir SSO]** for selecionada, eles não receberão esses emails, a menos que sejam atribuídos a uma função definida como **[!UICONTROL Ignorar Logon Único]**.

Pronto! Agora todos os usuários (exceto os usuários com permissão para ignorar o logon único) serão restritos a usar somente o logon com SSO.

>[!MORELIKETHIS]
>
>* [Adicionar Logon Único a um Portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Uso de uma Universal ID para logon de assinatura](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Convidar usuários do Marketo para duas instâncias com Universal ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

