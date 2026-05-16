---
unique-page-id: 2360350
description: Criar um serviço LaunchPoint personalizado vinculado a um usuário somente API para integração com a API ReST.
title: Criar um serviço personalizado para usar com a API REST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
TQID: https://experienceleague.adobe.com/7RYZTS-1WiaU0A8ThqHvk01S7GLIIP65xyKI3SIuPyo
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 175
ht-degree: 15%

---

# Criar um serviço personalizado para usar com a API REST {#create-a-custom-service-for-use-with-rest-api}

Se quiser integrar ao Marketo por meio da API ReST, crie um serviço personalizado.

>[!PREREQUISITES]
>
>* [Criar uma função de usuário somente API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Criar um Usuário Somente de API](/help/marketo/product-docs/administration/users-and-roles/create-api-only-user.md)
>

>[!NOTE]
>
>**Permissões de administrador são necessárias**

>[!TIP]
>
>Consulte a documentação de desenvolvedores para obter detalhes sobre a [REST API](https://developer.adobe.com/marketo-apis/).

## Criar serviço personalizado {#create-custom-service}

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Clique em **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Selecione **[!UICONTROL Novo]** e depois **[!UICONTROL Novo serviço]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Digite um **[!UICONTROL Nome para Exibição]** para o serviço. Selecione o **[!UICONTROL Usuário Somente API]** [criado anteriormente](/help/marketo/product-docs/administration/users-and-roles/create-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

1. Clique em **[!UICONTROL Criar]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   O serviço foi criado. Recupere as credenciais para fornecer acesso.

## Credenciais para acesso à API {#credentials-for-api-access}

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Clique em **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Clique em **[!UICONTROL Exibir Detalhes]** para o serviço [!UICONTROL LaunchPoint] personalizado criado acima.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Clique em **[!UICONTROL Obter token]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Forneça a **[!UICONTROL ID do Cliente]**, o **[!UICONTROL Segredo do Cliente]**, o **[!UICONTROL Usuário Autorizado]** e o **[!UICONTROL Token]** à pessoa encarregada de estabelecer a conexão.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>Não compartilhe essas informações, pois elas fornecem acesso aos seus dados.
