---
unique-page-id: 2360207
description: Criar um usuário somente de API - Documentação do Marketo - Documentação do produto
title: Criar um usuário somente de API
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
feature: Users and Roles
source-git-commit: ab1ea483998d6cb37277b18adf2c1d3371bb40e6
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 1%

---

# Criar um usuário somente de API {#create-an-api-only-user}

Se quiser integrar ao Marketo por meio da [REST API](https://developers.marketo.com/documentation/rest/){target="_blank"}, será necessário criar um usuário somente de API. Veja como.

>[!IMPORTANT]
>
>Se estiver criando API Somente para usuários em uma assinatura integrada ao Adobe Identity, suas etapas serão diferentes e [pode ser encontrado aqui](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md){target="_blank"}.

>[!PREREQUISITES]
>
>[Criar uma função de usuário somente API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/create-an-api-only-user-1.png)

1. Clique em **[!UICONTROL Usuários e funções]**.

   ![](assets/create-an-api-only-user-2.png)

1. Clique em **[!UICONTROL Convidar novo usuário]**.

   ![](assets/create-an-api-only-user-3.png)

1. Insira um email, nome e sobrenome como usuário somente da API. Clique em **[!UICONTROL Próxima]**.

   ![](assets/create-an-api-only-user-4.png)

   >[!TIP]
   >
   >Adicione um motivo opcional ou uma data de expiração de acesso. As datas de expiração de acesso são úteis para funcionários de curto prazo.

1. Selecione o **[!UICONTROL Somente API]** e verifique a **[!UICONTROL Somente API]** caixa de seleção Clique em **[!UICONTROL Próxima]**.

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
