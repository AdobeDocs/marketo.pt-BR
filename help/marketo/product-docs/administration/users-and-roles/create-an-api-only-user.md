---
unique-page-id: 2360207
description: Criar um usuário somente de API - Documentação do Marketo - Documentação do produto
title: Criar um usuário somente de API
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
feature: Users and Roles
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 6%

---

# Criar um usuário somente de API {#create-an-api-only-user}

Se você quiser integrar com o Marketo por meio da [REST API](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}, será necessário criar um usuário somente de API. Veja como.

>[!IMPORTANT]
>
>Se você estiver criando somente API de usuários em uma assinatura que foi integrada à Adobe Identity, suas etapas serão diferentes e [poderá ser encontrado aqui](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md){target="_blank"}.

>[!PREREQUISITES]
>
>[Criar uma função de usuário somente API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/create-an-api-only-user-1.png)

1. Clique em **[!UICONTROL Usuários e funções]**.

   ![](assets/create-an-api-only-user-2.png)

1. Clique em **[!UICONTROL Convidar novo usuário]**.

   ![](assets/create-an-api-only-user-3.png)

1. Insira um email, nome e sobrenome como usuário somente da API. Clique em **[!UICONTROL Avançar]**.

   ![](assets/create-an-api-only-user-4.png)

   >[!TIP]
   >
   >Adicione uma [!UICONTROL Razão] opcional ou uma data de [!UICONTROL Expiração do Acesso]. As datas de expiração de acesso são úteis para funcionários de curto prazo.

1. Selecione a função **[!UICONTROL Somente API]** e marque a caixa de seleção **[!UICONTROL Somente API]**. Clique em **[!UICONTROL Avançar]**.

   ![](assets/create-an-api-only-user-5.png)

1. Clique em **[!UICONTROL Enviar]**.

   ![](assets/create-an-api-only-user-6.png)

>[!NOTE]
>
>A janela pop-up diz: &quot;Um convite não é necessário somente para API&quot;, mas isso não significa que você fez algo errado. Significa apenas que criaremos a função sem que um email de convite tenha que ser enviado.

Tudo bem, então! Agora vamos criar o serviço personalizado.

>[!MORELIKETHIS]
>
>[Criar um serviço personalizado para usar com a API REST](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md){target="_blank"}
