---
unique-page-id: 2360350
description: Criar um serviço personalizado para uso com a API ReST - Documentos do Marketing Cloud - Documentação do produto
title: Criar um serviço personalizado para uso com a API ReST
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---


# Criar um serviço personalizado para uso com a API ReST {#create-a-custom-service-for-use-with-rest-api}

Se você quiser se integrar ao Marketo por meio da API ReST, será necessário criar um serviço personalizado. Veja como.

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
>Consulte a documentação de nossos desenvolvedores para obter detalhes sobre a [API ReST](http://developers.marketo.com/documentation/rest/). Também temos a [API SOAP](http://developers.marketo.com/documentation/soap/) se for isso que você precisa.

>[!NOTE]
>
>Não é possível criar um serviço personalizado se você tiver o nível de Faísca de Marketo.

## Criar Serviço Personalizado {#create-custom-service}

1. Vá para **Admin** e clique em **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. Em **Novo**, clique em **Novo serviço**.

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. Digite um **Nome de exibição** para o serviço. Selecione **Usuário Somente API** [criado anteriormente](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   >[!NOTE]
   >
   >Observe que já temos integração nativa para serviços de webinar populares.

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. Clique em **Criar**.

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   Oh, sim! O serviço agora é criado, vamos continuar e obter todas as credenciais para fornecer acesso.

## Credenciais para Acesso à API {#credentials-for-api-access}

1. Vá para **Admin** e clique em **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. Clique em **Detalhes da Visualização** para obter o serviço personalizado do LaunchPoint criado acima.

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. Clique em **Obter token**.

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. Forneça o **ID do cliente**, **Segredo do cliente**, **Utilizador autorizado** e **Token** à pessoa responsável pela criação da ligação.

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>Não compartilhe essas informações. é a porta de entrada para seus dados. Mantenha-o seguro!
