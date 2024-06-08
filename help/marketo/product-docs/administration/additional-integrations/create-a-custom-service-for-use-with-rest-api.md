---
unique-page-id: 2360350
description: Criar um serviço personalizado para usar com a API ReST - Documentação do Marketo - Documentação do produto
title: Criar um serviço personalizado para usar com a API ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Criar um serviço personalizado para usar com a API ReST {#create-a-custom-service-for-use-with-rest-api}

Se quiser integrar ao Marketo por meio da API ReST, crie um serviço personalizado. Veja como.

>[!PREREQUISITES]
>
>* [Criar uma função de usuário somente API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Criar um usuário somente de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!TIP]
>
>Consulte nossa documentação de desenvolvedores para obter detalhes sobre a [REST API](https://developer.adobe.com/marketo-apis/). Também temos o [API SOAP](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/soap/soap-api) se é isso que você precisa.

## Criar serviço personalizado {#create-custom-service}

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Clique em **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Selecionar **[!UICONTROL Novo]** e depois **[!UICONTROL Novo serviço]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Insira um **[!UICONTROL Nome de exibição]** para o serviço. Selecione o **[!UICONTROL Somente usuário da API]** [criado anteriormente](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >Observe que já temos integração nativa para serviços populares de webinários.

1. Clique em **[!UICONTROL Criar]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Ah, sim! O serviço foi criado, vamos buscar todas as credenciais para fornecer acesso.

## Credenciais para acesso à API {#credentials-for-api-access}

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Clique em **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Clique em **[!UICONTROL Exibir detalhes]** para o personalizado [!UICONTROL LaunchPoint] serviço criado acima.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Clique em **[!UICONTROL Obter token]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Forneça o **[!UICONTROL ID do cliente]**, **[!UICONTROL Segredo do cliente]**, **[!UICONTROL Usuário autorizado]**, e **[!UICONTROL Token]** à pessoa encarregada de estabelecer a ligação.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>Não compartilhe essa informação; é o segredo dos seus dados. Mantenha-o seguro!
