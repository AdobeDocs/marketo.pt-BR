---
unique-page-id: 10097613
description: Adicionar campos de link de objeto personalizado do Marketo - Documentos do Marketo - Documentação do produto
title: Adicionar campos de link de objeto personalizado de marketing
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---


# Adicionar campos de link de objeto personalizado de marketing {#add-marketo-custom-object-link-fields}

Ao criar objetos personalizados, você deve fornecer campos de link para conectar o registro de objetos personalizados ao registro pai correto.

* Para uma estrutura personalizada um para muitos, use o campo de link no objeto personalizado para conectá-lo a uma pessoa ou empresa.
* Para uma estrutura muitas para muitas, você usa dois campos de link, conectados a partir de um objeto intermediário criado separadamente (que é também um tipo de objeto personalizado). Um link se conecta a pessoas ou empresas no banco de dados e o outro se conecta ao objeto personalizado. Nesse caso, o campo de link não está localizado no próprio objeto personalizado.

## Criar um campo de link para uma estrutura de um para muitos {#create-a-link-field-for-a-one-to-many-structure}

Veja como criar um campo de link em um objeto personalizado para uma estrutura um para muitos.

1. Clique em **Admin** e, em **Gerenciamento de banco de dados**, selecione **Objetos personalizados de marketing**.

   ![](assets/image2016-1-18-13-3a25-3a11.png)

1. Selecione o objeto personalizado na lista.

   ![](assets/image2016-1-14-15-3a6-3a2.png)

1. Na guia **Campos**, clique em **Novo campo**.

   ![](assets/image2015-9-17-14-3a9-3a19.png)

1. Nomeie o campo de link e adicione uma descrição opcional. Certifique-se de selecionar o tipo de dados Link.

   ![](assets/image2015-10-5-13-3a24-3a57.png)

   >[!CAUTION]
   >
   >Não será possível voltar e criar, editar ou excluir um Link ou um Campo de exclusão depois que o objeto personalizado for aprovado.

1. Selecione se o objeto de link é para um cliente potencial (pessoa) ou uma empresa.

   ![](assets/image2015-10-5-13-3a28-3a1.png)

   >[!NOTE]
   >
   >Se você escolher o cliente potencial, verá ID, endereço de email e quaisquer campos personalizados na lista.
   >
   >
   >Se você escolher empresa, verá ID e quaisquer campos personalizados na lista.

1. Selecione o campo de link ao qual você deseja se conectar como o pai do novo campo.

   ![](assets/image2015-10-5-13-3a30-3a6.png)

   >[!NOTE]
   >
   >Somente os tipos de campos de string são suportados no campo de link.

1. Clique em **Salvar.**

   ![](assets/image2015-10-5-13-3a34-3a0.png)

## Criar um campo de link para uma estrutura de muitos para muitos {#create-a-link-field-for-a-many-to-many-structure}

Veja como criar um campo de link em um objeto intermediário para uso em uma estrutura muitas para muitas.

>[!PREREQUISITES]
>
>Você já deve ter criado o objeto intermediário e todos os objetos personalizados aos quais deseja vinculá-lo.

1. Clique em **Admin** e, em **Gerenciamento de banco de dados**, selecione **Objetos personalizados de marketing**.

   ![](assets/image2016-1-18-9-3a8-3a14.png)

1. Selecione o objeto intermediário ao qual deseja adicionar o campo.

   ![](assets/image2016-1-18-9-3a10-3a29.png)

1. Na guia **Campos **, clique em **Novo campo**.

   ![](assets/image2016-1-18-9-3a31-3a43.png)

1. É necessário criar dois campos de link. Crie um de cada vez. Primeiro, nomeie o campo para os membros da lista do banco de dados (leadID, por exemplo). Adicione uma descrição opcional. Certifique-se de selecionar o tipo de dados do link.

   ![](assets/image2016-1-18-9-3a38-3a59.png)

   >[!CAUTION]
   >
   >Não será possível voltar e criar, editar ou excluir um Link ou um Campo de exclusão depois que o objeto personalizado for aprovado.

1. Selecione o objeto de link do banco de dados, neste caso Lead.

   ![](assets/image2016-1-18-9-3a50-3a48.png)

1. Selecione o campo de link ao qual você deseja se conectar, neste caso, a Id.

   ![](assets/image2016-1-18-9-3a53-3a54.png)

   >[!NOTE]
   >
   >Somente os tipos de campos de string são suportados no campo de link.

1. Clique em **Salvar.**

   ![](assets/image2016-1-18-9-3a55-3a18.png)

1. Repita esse processo para o segundo link para o objeto personalizado, neste exemplo, cursoID. O Nome do objeto do link será o curso e o Campo do link será o cursoID. Como você já criou e aprovou o objeto personalizado do curso, essas seleções estão disponíveis nos menus suspensos.

   ![](assets/image2016-1-18-9-3a57-3a46.png)

1. Crie quaisquer outros campos que você deseja usar em seu objeto intermediário, como a enrollmentID ou o nível.

## Uso de objetos personalizados {#using-custom-objects}

A próxima etapa é usar esses objetos personalizados em filtros em suas campanhas inteligentes. Com uma relação muitos para muitos, você pode selecionar várias pessoas/empresas e vários objetos personalizados. No exemplo abaixo, qualquer pessoa em seu banco de dados que corresponder a esses critérios será listada. O campo coursename provém do objeto personalizado do curso e o nível de inscrição provém do objeto intermediário.

![](assets/image2016-1-14-15-3a57-3a59.png)

>[!NOTE]
>
>**Artigos relacionados**
>
>* [Adicionar campos de objeto personalizados de marketing](add-marketo-custom-object-fields.md)
>* [Editar e excluir um objeto personalizado de marketing](edit-and-delete-a-marketo-custom-object.md)
>* [Como entender objetos personalizados de marketing](understanding-marketo-custom-objects.md)
>* [Editar e excluir campos de objetos personalizados de marketing](edit-and-delete-marketo-custom-object-fields.md)

>



