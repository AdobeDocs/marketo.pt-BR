---
unique-page-id: 10093188
description: Noções básicas sobre objetos personalizados do Marketo - Documentos do Marketo - Documentação do produto
title: Como entender objetos personalizados do Marketo
exl-id: f18b1689-c7bc-4da0-8326-7b29733d527d
source-git-commit: 6f17d79344653d1b2c364753d774998e343c9808
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 2%

---

# Como entender objetos personalizados do Marketo {#understanding-marketo-custom-objects}

Use objetos personalizados para rastrear métricas específicas da sua empresa.

>[!AVAILABILITY]
>
>Nem todos os clientes compraram essa funcionalidade. Confira os detalhes com seu representante de vendas.

Use objetos personalizados como filtros e acionadores em suas campanhas inteligentes. Por exemplo:

* **Filtro**: Enviar emails somente para proprietários de uma marca de veículo específica
* **Acionador**: Enviar um email quando um objeto personalizado for adicionado a uma pessoa ou empresa.

Você pode configurar objetos personalizados em uma relação um para muitos ou muitos para muitos. Por exemplo:

* **Um para muitos**: Uma pessoa possui vários carros
* **Muitos para muitos**: Vários alunos estão matriculados em vários cursos de um catálogo de cursos

Uma estrutura de um para muitos usa um único campo de link para conectar o objeto personalizado a uma pessoa ou empresa.

Muitos objetos personalizados usam dois campos de link, parte de um objeto intermediário. Um campo Link é conectado à pessoa ou empresa e outro é conectado ao objeto personalizado, como o catálogo de curso. Esse objeto intermediário pode conter campos personalizados adicionais, como um grau de curso ou uma data de participação, que definem ainda mais a natureza da conexão.

>[!TIP]
>
>Importe objetos personalizados usando valores separados por vírgula (CSV) na interface do usuário para testar e validar uma amostra de dados. Em seguida, carregue todos os seus arquivos com uma API.

>[!CAUTION]
>
>Não é possível restaurar objetos personalizados, portanto, certifique-se de não precisar mais deles antes de excluí-los.

## Acessar objetos personalizados do Marketo {#accessing-marketo-custom-objects}

1. Para criar ou editar objetos personalizados do Marketo, clique em **Administrador** e depois a **Objetos personalizados do Marketo** link .

   ![](assets/understanding-marketo-custom-objects-1.png)

1. A exibição Objetos personalizados do Marketo lista todos os seus objetos personalizados à direita, mas apenas os aprovados na grade principal.

   ![](assets/understanding-marketo-custom-objects-2.png)

1. A grade exibe o nome do objeto, o número de registros, o número de campos e a data da atualização mais recente.

   >[!TIP]
   >
   >O Marketo atualiza esses campos automaticamente, mas é possível atualizar a exibição clicando no ícone na coluna Registros .

1. Clique no nome do objeto à direita para abrir a página de detalhes.

   ![](assets/understanding-marketo-custom-objects-3.png)

## Exibir objetos personalizados associados a uma pessoa {#view-custom-objects-associated-to-a-person}

Após criar a estrutura de objetos personalizados, ao carregar os dados de objetos personalizados específicos, os objetos personalizados são associados automaticamente às pessoas no banco de dados usando o campo de link no objeto personalizado. É possível exibir informações da guia Objetos personalizados na página de detalhes da pessoa.

1. Ir para **Banco de dados**.

   ![](assets/understanding-marketo-custom-objects-4.png)

1. Abra o banco de dados e clique no botão **Pessoas** guia . Clique duas vezes no registro de uma pessoa associada a um objeto personalizado.

   ![](assets/understanding-marketo-custom-objects-5.png)

1. Na página de detalhes da pessoa, clique no botão **Objetos personalizados** guia . Selecione o objeto no menu suspenso .

   ![](assets/understanding-marketo-custom-objects-6.png)

1. Agora você pode exibir uma lista de todos os objetos personalizados desse tipo que estão associados a essa pessoa.

   ![](assets/understanding-marketo-custom-objects-7.png)

## Uso de objetos personalizados com empresas {#using-custom-objects-with-companies}

Um objeto personalizado vinculado à empresa funciona melhor se você sincronizar empresas do CRM ou se criar empresas explicitamente usando a API. Também recomendamos usar a ID da empresa como o campo de link .

Se houver várias pessoas no Marketo que são registros no CRM ou nos registros somente Marketo, um objeto personalizado vinculado a uma empresa não será associado a mais de um registro individual. Isso ocorre porque uma empresa que tem várias pessoas abaixo dela é suportada somente quando empresas são sincronizadas do CRM ou se você usa uma API para criar empresas explicitamente.

Os objetos personalizados só podem se vincular diretamente a um único registro. Isso significa que, quando o tipo de objeto personalizado é vinculado por campo da empresa, é necessário garantir que os registros de pessoa sejam associados a uma empresa usando a conversão de contato em seu CRM ou usando o campo externalCompanyId , caso gerencie empresas usando as APIs REST da Marketo. Para registros de pessoas que não estão vinculados explicitamente a registros de empresas, objetos personalizados vinculados por empresas serão aleatoriamente vinculados a um único registro, mesmo se o valor do campo de empresa for compartilhado por muitas pessoas.

Consulte [Importar dados de objeto personalizado](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md) para obter mais informações.

>[!MORELIKETHIS]
>
>* [Criar objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md)
>* [Aprovar um objeto personalizado](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
>* [Editar e excluir um objeto personalizado do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Adicionar campos de objeto personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Editar e excluir campos de objeto personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Importar dados de objeto personalizado](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md)

