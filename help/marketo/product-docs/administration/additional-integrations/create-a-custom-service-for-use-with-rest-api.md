---
unique-page-id: 2360350
description: Criar um serviço personalizado para usar com a API ReST - Documentação do Marketo - Documentação do produto
title: Criar um serviço personalizado para usar com a API ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 1%

---

# Criar um serviço personalizado para usar com a API ReST {#create-a-custom-service-for-use-with-rest-api}

Se quiser integrar ao Marketo por meio da API ReST, crie um serviço personalizado. Veja como.

>[!PREREQUISITES]
>
>* [Criar uma função de usuário somente API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Criar um Usuário Somente de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!TIP]
>
>Consulte nossa documentação de desenvolvedores para obter detalhes sobre a [REST API](https://developer.adobe.com/marketo-apis/). Também temos a [API do SOAP](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/soap/soap-api), se for o que você precisa.

## Criar serviço personalizado {#create-custom-service}

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Clique em **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Selecione **[!UICONTROL Novo]** e depois **[!UICONTROL Novo serviço]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Digite um **[!UICONTROL Nome para Exibição]** para o serviço. Selecione o **[!UICONTROL Usuário Somente API]** [criado anteriormente](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >Observe que já temos integração nativa para serviços populares de webinários.

1. Clique em **[!UICONTROL Criar]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Ah, sim! O serviço foi criado, vamos buscar todas as credenciais para fornecer acesso.

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
>Não compartilhe essa informação; é o segredo dos seus dados. Mantenha-o seguro!
