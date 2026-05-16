---
unique-page-id: 2360358
description: Exigir SSO para todos os usuários para que eles não possam ignorar a segurança SSO por meio das Configurações de logon de administrador (não se aplica ao Adobe IMS).
title: Logon de usuário restrito apenas a SSO
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
TQID: https://experienceleague.adobe.com/2YaweRRhrf8po6RR3V64kCan8qQhDNKDrhr7TfnNNJs
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 273
ht-degree: 5%

---

# Logon de usuário restrito apenas a SSO {#restrict-user-login-to-sso-only}

Se você estiver [usando SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) e quiser garantir que os usuários não possam ignorar a segurança SSO, siga estas instruções.

>[!IMPORTANT]
>
>Este artigo não se aplica a [assinaturas do Marketo habilitadas para Adobe IMS](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md).

>[!NOTE]
>
>**Permissões de administrador são necessárias**

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. Clique em **[!UICONTROL Configurações de logon]**.

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. Clique em **[!UICONTROL Editar configurações de segurança]**.

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. Expanda as configurações **[!UICONTROL Avançadas]**, marque **[!UICONTROL Solicitar SSO]** e clique em **[!UICONTROL Salvar]**.

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>A prática recomendada é que os usuários sejam convidados e aceitem o convite. _Depois_ que o convite for aceito, os administradores devem defini-los como &quot;[!UICONTROL Exigir SSO].&quot;

>[!TIP]
>
>Se você selecionar **[!UICONTROL Exigir SSO]**, poderá excluir uma [função de usuário](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) dessa restrição marcando a opção **[!UICONTROL Ignorar Logon Único]** ao configurar a função. Isso permite que os usuários façam logon normalmente. Por exemplo, os usuários administradores ainda podem precisar fazer logon no Marketo por meio da tela de logon. Se o SSO e a Universal ID estiverem habilitados, você deve ter a permissão &quot;Ignorar logon único&quot; definida para alternar entre as assinaturas.

>[!CAUTION]
>
>Quando novos usuários são convidados, eles recebem emails de convite. No entanto, se **[!UICONTROL Exigir SSO]** for selecionado, eles não receberão esses emails, a menos que sejam atribuídos a uma função definida como **[!UICONTROL Ignorar Logon Único]**.

Agora todos os usuários (exceto os usuários com permissão para ignorar o logon único) estão restritos a usar somente o logon com SSO.

>[!MORELIKETHIS]
>
>* [Adicionar Logon Único a um Portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Convidando Usuários do Marketo para Duas Instâncias com Universal ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
