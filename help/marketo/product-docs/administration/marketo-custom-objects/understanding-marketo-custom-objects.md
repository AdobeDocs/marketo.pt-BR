---
unique-page-id: 10093188
description: Como entender objetos personalizados do Marketing - Documentos do Marketing - Documentação do produto
title: Como entender objetos personalizados de marketing
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---


# Como entender objetos personalizados de marketing {#understanding-marketo-custom-objects}

Use objetos personalizados para rastrear métricas específicas à sua empresa.

>[!AVAILABILITY]
>
>Nem todos os clientes adquiriram essa funcionalidade. Entre em contato com seu representante de vendas para obter detalhes.

Use objetos personalizados como filtros e acionadores em suas campanhas inteligentes. Por exemplo:

* **Filtro**: Enviar emails somente para proprietários de uma marca de veículo específica
* **Acionador**: Envie um email quando um objeto personalizado for adicionado a uma pessoa ou empresa.

É possível configurar objetos personalizados em uma relação um para muitos ou muitos para muitos. Por exemplo:

* **Um para muitos**: Uma pessoa possui vários carros
* **Muitos para muitos**: Vários alunos estão inscritos em vários cursos de um catálogo de cursos

Uma estrutura de um para muitos usa um único campo de link para conectar o objeto personalizado a uma pessoa ou empresa.

Muitos objetos personalizados usam dois campos de link, parte de um objeto intermediário. Um campo de link é conectado à pessoa ou empresa e outro é conectado ao objeto personalizado, como o catálogo de cursos. Esse objeto intermediário pode conter campos personalizados adicionais, como um grau de curso ou uma data de participação, que definem ainda mais a natureza da conexão.

>[!TIP]
>
>Importe objetos personalizados usando valores separados por vírgula (CSV) na interface do usuário para testar e validar uma amostra de dados. Em seguida, carregue todos os seus arquivos com uma API.

>[!CAUTION]
>
>Não é possível restaurar objetos personalizados, portanto, certifique-se de que não precisa mais deles antes de excluí-los.

## Acessar objetos personalizados de marketing {#accessing-marketo-custom-objects}

1. Para criar ou editar objetos personalizados do Marketo, clique no link **Admin** e **Objetos personalizados do Marketing**.

   ![](assets/image2016-5-18-16-3a59-3a30.png)

1. A exibição Objetos personalizados de marketing lista todos os objetos personalizados à direita, mas somente os aprovados na grade principal.

   ![](assets/image2016-6-10-15-3a14-3a18.png)

1. A grade exibe o nome do objeto, o número de registros, o número de campos e a data da atualização mais recente.

   >[!TIP]
   >
   >O Marketo atualiza esses campos automaticamente, mas você pode atualizar a exibição clicando no ícone na coluna Registros.

1. Clique no nome do objeto à direita para abrir a página de detalhes.

   ![](assets/image2016-6-10-15-3a15-3a29.png)

## Visualização de objetos personalizados associados a uma pessoa {#view-custom-objects-associated-to-a-person}

Depois de criar a estrutura de objetos personalizados, ao carregar os dados de objetos personalizados específicos, os objetos personalizados são automaticamente associados às pessoas no banco de dados usando o campo de link no objeto personalizado. Você pode visualização informações na guia Objetos personalizados na página de detalhes da pessoa.

1. Vá para **Banco de Dados**.

   ![](assets/db.png)

1. Abra o banco de dados e clique na guia **Pessoas**. Clique no duplo do registro de uma pessoa associada a um objeto personalizado.

   ![](assets/five.png)

1. Na página de detalhes da pessoa, clique na guia **Objetos personalizados**. Selecione o objeto no menu suspenso.

   ![](assets/six.png)

1. Agora você pode visualização uma lista de todos os objetos personalizados desse tipo que estão associados a essa pessoa.

   ![](assets/seven.png)

## Uso de objetos personalizados com Empresa {#using-custom-objects-with-companies}

Um objeto personalizado vinculado à empresa funciona melhor se você sincronizar o empresa do CRM ou se criar explicitamente o empresa usando a API. Também recomendamos que você use a ID da Empresa como campo de link.

Se você tiver várias pessoas no Marketo que são registros no CRM ou somente no Marketo, um objeto personalizado vinculado a uma empresa não será associado a mais de um registro individual. Isso ocorre porque uma empresa com várias pessoas abaixo dela é suportada somente quando o empresa é sincronizado do CRM ou se você usa uma API para criar explicitamente o empresa.

Objetos personalizados podem se vincular diretamente a um único registro. Isso significa que, quando seu tipo de objeto personalizado é vinculado por campo de empresa, você deve garantir que seus registros pessoais sejam associados a uma empresa usando a conversão de contato no CRM ou usando o campo externalCompanyId, se você gerenciar empresa usando as APIs REST do Marketo. Para registros pessoais que não estejam vinculados explicitamente a registros de empresa, objetos personalizados vinculados por empresa serão aleatoriamente vinculados a um único registro, mesmo se o valor do campo de empresa for compartilhado entre muitas pessoas.

Consulte [Importar dados de objeto personalizados](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md) para obter mais informações.

>[!MORELIKETHIS]
>
>* [Criar objetos personalizados de marketing](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md)
>* [Aprovar um objeto personalizado](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
>* [Editar e excluir um objeto personalizado de marketing](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Adicionar campos de objeto personalizados de marketing](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Editar e excluir campos de objetos personalizados de marketing](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Importar dados de objetos personalizados](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md)

