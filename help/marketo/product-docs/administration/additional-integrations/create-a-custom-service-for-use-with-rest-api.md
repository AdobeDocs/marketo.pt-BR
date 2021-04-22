---
unique-page-id: 2360350
description: Criar um serviço personalizado para uso com a API ReST - Documentos do Marketo - Documentação do produto
title: Criar um serviço personalizado para uso com a API ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '224'
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
>Consulte a documentação de nossos desenvolvedores para obter detalhes sobre a [ReST API](https://developers.marketo.com/documentation/rest/). Também temos a [API SOAP](https://developers.marketo.com/documentation/soap/) se for necessário.

>[!NOTE]
>
>Não é possível criar um serviço personalizado se você tiver o nível de Spark do Marketo.

## Criar Serviço Personalizado {#create-custom-service}

1. Vá para **Admin** e clique em **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. Em **Novo**, clique em **Novo Serviço**.

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. Insira um **Nome de Exibição** para o serviço. Selecione o **Usuário Somente API** [criado anteriormente](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   >[!NOTE]
   >
   >Observe que já temos integração nativa para serviços populares de webinar.

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. Clique em **Criar**.

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   Sim! O serviço foi criado, vamos continuar e obter todas as credenciais para fornecer acesso.

## Credenciais para o Acesso à API {#credentials-for-api-access}

1. Vá para **Admin** e clique em **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. Clique em **Exibir detalhes** para o serviço personalizado do LaunchPoint criado acima.

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. Clique em **Obter token**.

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. Forneça o **Client Id**, **Client Secret**, **Authorized User** e **Token** à pessoa encarregada de estabelecer a conexão.

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>Não compartilhe essas informações; é o backdoor para seus dados. Mantenha seguro!
