---
unique-page-id: 10097613
description: Adicionar campos de link de objeto personalizado do Marketo - Documentação do Marketo - Documentação do produto
title: Adicionar campos de link de objeto personalizado do Marketo
exl-id: e7537d79-9fca-4966-881a-9d7d312008e2
feature: Custom Objects
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Adicionar campos de link de objeto personalizado do Marketo {#add-marketo-custom-object-link-fields}

Ao criar objetos personalizados, você deve fornecer campos de link para conectar o registro de objeto personalizado ao registro pai correto.

* Para uma estrutura personalizada de um para muitos, use o campo de link no objeto personalizado para conectá-lo a uma pessoa ou empresa.
* Para uma estrutura muitos para muitos, você usa dois campos de link, conectados de um objeto intermediário criado separadamente (que também é um tipo de objeto personalizado). Um link se conecta a pessoas ou empresas no banco de dados e o outro se conecta ao objeto personalizado. Nesse caso, o campo de link não está localizado no próprio objeto personalizado.

>[!IMPORTANT]
>
>O Marketo Engage só oferece suporte a um único objeto de borda para cada objeto de ponte no relacionamento Muitos para Muitos. Na amostra apresentada abaixo, cada inscrição só pode ser vinculada a um único curso. No entanto, pode haver muitos objetos de ponte para cada objeto de borda, assim como há muitas inscrições de alunos para cada curso (relacionamento muitos para um). Se você tiver seus dados de objeto personalizados estruturados de modo que haja mais de um registro de objeto do Edge para cada registro de objeto do Bridge (Um para muitos ou Muitos para muitos), poderá criar vários registros de objeto do Bridge que se referem a um único registro de objeto do Edge para representar esses dados no Marketo.

## Criar um campo de link para uma estrutura de um para muitos {#create-a-link-field-for-a-one-to-many-structure}

Veja como criar um campo de link em um objeto personalizado para uma estrutura de um para muitos.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/add-marketo-custom-object-link-fields-1.png)

1. Clique em **[!UICONTROL Objetos personalizados do Marketo]**.

   ![](assets/add-marketo-custom-object-link-fields-2.png)

1. Selecione o objeto personalizado na lista.

   ![](assets/add-marketo-custom-object-link-fields-3.png)

1. Na guia **[!UICONTROL Campos]**, clique em **[!UICONTROL Novo Campo]**.

   ![](assets/add-marketo-custom-object-link-fields-4.png)

1. Nomeie o campo de link e adicione uma [!UICONTROL Descrição] opcional. Certifique-se de selecionar o tipo de dados [!UICONTROL Link].

   ![](assets/add-marketo-custom-object-link-fields-5.png)

   >[!CAUTION]
   >
   >Você não poderá voltar e criar, editar ou excluir um [!UICONTROL Link] ou [!UICONTROL Campo de Desduplicação] depois que o objeto personalizado for aprovado.

1. Selecione se o [!UICONTROL Objeto de Link] é para uma [!UICONTROL cliente em potencial] (pessoa) ou uma [!UICONTROL empresa].

   ![](assets/add-marketo-custom-object-link-fields-6.png)

   >[!NOTE]
   >
   >Se você escolher [!UICONTROL cliente em potencial], verá ID, endereço de email e quaisquer campos personalizados na lista.
   >
   >Se você escolher [!UICONTROL empresa], verá a ID e todos os campos personalizados na lista.

1. Selecione o [!UICONTROL Campo de Links] ao qual você deseja se conectar como o pai do novo campo.

   ![](assets/add-marketo-custom-object-link-fields-7.png)

   >[!NOTE]
   >
   >Há suporte somente para tipos de campo de cadeia de caracteres no [!UICONTROL Campo de Link].

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/add-marketo-custom-object-link-fields-8.png)

## Criar um campo de link para uma estrutura muitos para muitos {#create-a-link-field-for-a-many-to-many-structure}

Veja como criar um campo de link em um objeto intermediário para uso em uma estrutura muitos para muitos.

>[!PREREQUISITES]
>
>Você já deve ter criado o objeto intermediário e quaisquer objetos personalizados aos quais pretende vinculá-lo.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/add-marketo-custom-object-link-fields-9.png)

1. Clique em **[!UICONTROL Objetos personalizados do Marketo]**.

   ![](assets/add-marketo-custom-object-link-fields-10.png)

1. Selecione o objeto intermediário ao qual deseja adicionar o campo.

   ![](assets/add-marketo-custom-object-link-fields-11.png)

1. Na guia **[!UICONTROL Campos]**, clique em **[!UICONTROL Novo Campo]**.

   ![](assets/add-marketo-custom-object-link-fields-12.png)

1. Você precisa criar dois campos de link. Crie um de cada vez. Primeiro, nomeie o campo para os membros da lista do banco de dados (leadID, por exemplo). Adicione uma [!UICONTROL Descrição] opcional. Certifique-se de selecionar o [!UICONTROL link] [!UICONTROL Tipo de Dados].

   ![](assets/add-marketo-custom-object-link-fields-13.png)

   >[!CAUTION]
   >
   >Você não poderá voltar e criar, editar ou excluir um [!UICONTROL Link] ou [!UICONTROL Campo de Desduplicação] depois que o objeto personalizado for aprovado.

1. Selecione o [!UICONTROL Objeto de Link] do seu banco de dados; neste caso, [!UICONTROL Lead].

   ![](assets/add-marketo-custom-object-link-fields-14.png)

1. Selecione o [!UICONTROL Campo de Links] ao qual você deseja se conectar; neste caso, [!UICONTROL Id].

   ![](assets/add-marketo-custom-object-link-fields-15.png)

   >[!NOTE]
   >
   >Há suporte somente para tipos de campo de cadeia de caracteres no [!UICONTROL Campo de Link].

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/add-marketo-custom-object-link-fields-16.png)

1. Repita esse processo para o segundo link para seu objeto personalizado, neste exemplo, courseID. O nome do [!UICONTROL Objeto de Link] será course, e o [!UICONTROL Campo de Link] será courseID. Como você já criou e aprovou o objeto personalizado do curso, essas seleções estão disponíveis nos menus suspensos.

   ![](assets/add-marketo-custom-object-link-fields-17.png)

1. Crie quaisquer outros campos que deseja usar no objeto intermediário, como enrollmentID ou grade.

## Uso de objetos personalizados {#using-custom-objects}

A próxima etapa é usar esses objetos personalizados em filtros em suas campanhas inteligentes. Com uma relação muitos para muitos, você pode selecionar várias pessoas/empresas e vários objetos personalizados. No exemplo abaixo, qualquer pessoa no banco de dados que corresponda a esses critérios será listada. O campo nome do curso vem do objeto personalizado do curso e o nível de inscrição vem do objeto intermediário.

![](assets/add-marketo-custom-object-link-fields-18.png)

>[!MORELIKETHIS]
>
>* [Adicionar campos de objeto personalizado do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Editar e excluir um objeto personalizado do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Noções básicas sobre objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
>* [Editar e excluir campos de objeto personalizado do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
