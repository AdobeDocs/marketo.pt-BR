---
unique-page-id: 2360350
description: Criar um serviço personalizado para uso com a API ReST - Documentos do Marketo - Documentação do produto
title: Criar um serviço personalizado para uso com a API ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Criar um serviço personalizado para uso com a API ReST {#create-a-custom-service-for-use-with-rest-api}

Se quiser integrar com o Marketo por meio da API ReST, crie um serviço personalizado. Veja como.

>[!PREREQUISITES]
>
>* [Criar uma função de usuário somente de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Criar um usuário somente de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>


>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!TIP]
>
>Consulte a documentação de nossos desenvolvedores para obter detalhes sobre o [ReST API](https://developers.marketo.com/documentation/rest/). Também temos o [API SOAP](https://developers.marketo.com/documentation/soap/) se é disso que você precisa.

## Criar serviço personalizado {#create-custom-service}

1. Vá para o **Administrador** área.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Clique em **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Selecionar **Novo** e depois **Novo Serviço**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Insira um **Nome de exibição** para o serviço. Selecione o **Usuário somente API** [criado anteriormente](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >Observe que já temos integração nativa para serviços populares de webinar.

1. Clique em **Criar**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Sim! O serviço foi criado, vamos continuar e obter todas as credenciais para fornecer acesso.

## Credenciais para o Acesso à API {#credentials-for-api-access}

1. Vá para o **Administrador** área.

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Clique em **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Clique em **Exibir detalhes** para o serviço personalizado do LaunchPoint criado acima.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Clique em **Obter token**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Forneça a **ID do cliente**, **Segredo do cliente**, **Usuário autorizado** e **Token** à pessoa encarregada do estabelecimento da ligação.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>Não compartilhe essas informações; é o backdoor para seus dados. Mantenha seguro!
