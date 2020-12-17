---
unique-page-id: 10093192
description: Criar objetos personalizados de marketing - Documentos de marketing - Documentação do produto
title: Criar objetos personalizados de marketing
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---


# Criar objetos personalizados de marketing {#create-marketo-custom-objects}

Use objetos personalizados no Marketo para rastrear métricas específicas para sua empresa. Isto pode ser qualquer coisa, desde carros, até cursos, qualquer coisa que você queira modelar no Marketo para administrar suas campanhas.

>[!NOTE]
>
>É possível configurar objetos personalizados para funcionar com base em um para muitos ou muitos para muitos. Você cria o objeto inicial da mesma maneira, mas as etapas são diferentes ao start de adicionar campos ao objeto. Consulte [Entendendo objetos personalizados de marketing](understanding-marketo-custom-objects.md) para obter mais informações.

>[!NOTE]
>
>Não é possível criar, editar ou excluir um Link ou um Campo de exclusão depois que o objeto personalizado é aprovado.

## Criar um objeto personalizado para uma estrutura One-to-many {#create-a-custom-object-for-a-one-to-many-structure}

Este exemplo mostra um objeto personalizado Carro, para uso em uma estrutura um para muitos. Posteriormente, você criará um objeto personalizado do curso e um objeto intermediário para usar em uma estrutura muitas para muitas.

1. Clique em **Admin** e, em **Gerenciamento de banco de dados** selecione **Objetos personalizados de marketing**.

   ** ![](assets/image2016-1-18-13-3a12-3a19.png)

   **

1. Clique em **Novo objeto personalizado**.

   ![](assets/image2016-5-18-16-3a28-3a4.png)

   >[!NOTE]
   >
   >A guia Marketo Custom Objects (Objetos personalizados de marketing) exibe todos os objetos personalizados à direita e detalhes de quaisquer objetos aprovados, incluindo o número de registros e campos na atualização mais recente.

1. Insira um nome para exibição. O Nome da API e o Nome do plural são preenchidos automaticamente. Insira uma descrição (opcional).

   ![](assets/image2015-9-15-16-3a29-3a17.png)

   >[!NOTE]
   >
   >Você pode editar esses campos ao criá-los, mas depois que eles forem salvos, você só poderá editar o campo Nome do plural e o controle deslizante **Mostrar em Detalhe do cliente potencial**.

1. Puxe o **Show in Lead Detail **controle deslizante para exibir **Mostrar** se você deseja visualização dados de objeto personalizados na página do Banco de Dados Principal. Clique em **Salvar**.

   ![](assets/image2015-9-15-16-3a32-3a2.png)

1. As informações do objeto personalizado exibem o conteúdo inserido. Observe que está em um estado de Rascunho.

   ![](assets/image2015-9-15-16-3a38-3a22.png)

   A próxima etapa é adicionar campos a [criar seu objeto personalizado](add-marketo-custom-object-fields.md).

   >[!NOTE]
   >
   >Você só pode preencher objetos personalizados de marketing por meio de uma importação de lista ou da [API](http://developers.marketo.com/documentation/rest/).

## Criar um objeto personalizado para uma estrutura de muitos para muitos {#create-a-custom-object-for-a-many-to-many-structure}

Este exemplo mostra um objeto personalizado do curso, que você usará para criar uma relação muitos para muitos entre pessoas/empresas e cursos. Quando terminar, você criará um objeto intermediário para conectá-lo a pessoas ou empresas em seu banco de dados.

>[!NOTE]
>
>Para uma relação muitos para muitos, não é necessário criar um link no objeto personalizado. Em vez disso, você adicionará dois links ao objeto intermediário (consulte abaixo).

1. Clique em **Admin** e, em **Gerenciamento de banco de dados** selecione **Objetos personalizados de marketing**.

   ![](assets/image2016-1-18-13-3a16-3a25.png)

1. Clique em **Novo objeto personalizado**.

   ![](assets/image2016-5-18-16-3a32-3a42.png)

1. Insira um nome para exibição. O Nome da API e o Nome do plural são preenchidos automaticamente. Insira uma descrição (opcional).

   ![](assets/image2016-1-14-13-3a38-3a46.png)

   >[!NOTE]
   >
   >Você pode editar esses campos ao criá-los, mas depois que eles forem salvos, você só poderá editar o campo Nome do plural e o controle deslizante **Mostrar em Detalhe do cliente potencial**.

1. Puxe o **Show in Lead Detail **controle deslizante para exibir Mostrar se você deseja visualização dados de objeto personalizados na página Banco de Dados de Cliente Potencial. Clique em **Salvar**.

   ![](assets/image2016-1-14-13-3a42-3a56.png)

1. As informações do objeto personalizado exibem o conteúdo inserido. Observe que está em um estado de Rascunho.

   ![](assets/image2016-1-18-8-3a38-3a58.png)

   >[!NOTE]
   >
   >Você só pode preencher objetos personalizados de marketing por meio de uma importação de lista ou da [API](http://developers.marketo.com/documentation/rest/).

A próxima etapa é criar seu objeto intermediário (veja abaixo). Mas antes disso, você precisa criar um campo para se conectar com ele.

## Criar um objeto intermediário {#create-an-intermediary-object}

Use um objeto intermediário para conectar um objeto personalizado a pessoas ou empresas. Neste exemplo, ele é usado para conectar cursos em seu objeto personalizado do curso a pessoas ou empresas em seu banco de dados.

>[!NOTE]
>
>Não é necessário criar um objeto intermediário para uma estrutura de objeto personalizada um para muitos.

1. Clique em **Admin** e, em **Gerenciamento de banco de dados**, selecione **Objetos personalizados de marketing**.

   ![](assets/image2016-1-18-13-3a17-3a40.png)

1. Clique em **Novo objeto personalizado**.

   ![](assets/image2016-5-18-16-3a33-3a16.png)

1. Insira um nome para exibição. O Nome da API e o Nome do plural são preenchidos automaticamente. Insira uma descrição (opcional).

   ![](assets/image2016-1-14-14-3a10-3a44.png)

   >[!NOTE]
   >
   >Você pode editar esses campos ao criá-los, mas depois que eles forem salvos, você só poderá editar o campo Nome do plural e o controle deslizante Mostrar em detalhes do cliente potencial.

1. Puxe o controle deslizante **Mostrar em Detalhe do Cliente Potencial** para exibir Mostrar se deseja visualização de dados de objeto personalizados na página Banco de Dados Principal. Clique em **Salvar**.

   ![](assets/image2016-1-14-14-3a12-3a49.png)

1. As informações do objeto personalizado exibem o conteúdo inserido. Observe que está em um estado de Rascunho.

   A próxima etapa consiste em [adicionar campos de link](add-marketo-custom-object-link-fields.md) para conectar seu objeto intermediário a uma pessoa/empresa e a um objeto personalizado.

>[!MORELIKETHIS]
>
>* [Adicionar campos de objeto personalizados de marketing](add-marketo-custom-object-fields.md)
>* [Adicionar campos de link de objeto personalizado de marketing](add-marketo-custom-object-link-fields.md)
>* [Como entender objetos personalizados de marketing](understanding-marketo-custom-objects.md)

>



