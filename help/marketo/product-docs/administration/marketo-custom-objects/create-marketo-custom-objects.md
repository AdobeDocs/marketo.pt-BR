---
unique-page-id: 10093192
description: Criar objetos personalizados do Marketo - Documentos do Marketo - Documentação do produto
title: Criar objetos personalizados do Marketo
exl-id: d68b41e1-a12b-436f-aad7-42c7264cd901
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Criar objetos personalizados do Marketo {#create-marketo-custom-objects}

Use objetos personalizados no Marketo para rastrear métricas específicas de sua empresa. Isso pode ser qualquer coisa, desde carros, até cursos, qualquer coisa que você queira modelar no Marketo para executar suas campanhas.

>[!NOTE]
>
>É possível configurar objetos personalizados para funcionarem de um para muitos ou muitos para muitos. O objeto inicial é criado da mesma forma, mas as etapas são diferentes quando você começa a adicionar campos ao objeto. Consulte  [Como entender objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) para obter mais informações.

>[!NOTE]
>
>Não é possível criar, editar ou excluir um Link ou Campo de eliminação de duplicatas depois que o objeto personalizado é aprovado.

## Criar um objeto personalizado para uma estrutura de um para muitos {#create-a-custom-object-for-a-one-to-many-structure}

Este exemplo mostra um objeto personalizado Carro, para uso em uma estrutura um para muitos. Posteriormente, você criará um objeto personalizado de curso e um objeto intermediário para usar em uma estrutura muitos para muitos.

1. Clique em **Administrador** e em **Gerenciamento de banco de dados** select **Objetos personalizados do Marketo**.

   ![](assets/image2016-1-18-13-3a12-3a19.png)

1. Clique em **Novo objeto personalizado**.

   ![](assets/image2016-5-18-16-3a28-3a4.png)

   >[!NOTE]
   >
   >A guia Objetos personalizados do Marketo exibe todos os objetos personalizados à direita e os detalhes de quaisquer objetos aprovados, incluindo o número de registros e campos na atualização mais recente.

1. Insira um nome de exibição. O Nome da API e o Nome do Plural são preenchidos automaticamente. Insira uma descrição (opcional).

   ![](assets/image2015-9-15-16-3a29-3a17.png)

   >[!NOTE]
   >
   >Você pode editar esses campos ao criá-los, mas depois que eles forem salvos, você só poderá editar o campo Nome do Plural e o campo **Mostrar em Detalhes do Cliente Potencial** controle deslizante.

1. Puxe a **Mostrar em Detalhes do Cliente Potencial** controle deslizante sobre a exibição **Mostrar** se quiser exibir dados de objeto personalizado na página Banco de Dados de Lead. Clique em **Salvar**.

   ![](assets/image2015-9-15-16-3a32-3a2.png)

1. As informações do objeto personalizado exibem o conteúdo inserido. Observe que está em um estado de Rascunho.

   ![](assets/image2015-9-15-16-3a38-3a22.png)

   A próxima etapa é adicionar campos ao [criar o objeto personalizado](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md).

   >[!NOTE]
   >
   >Você só pode preencher os Objetos Personalizados do Marketo por meio de uma importação de lista ou do [API](https://developers.marketo.com/documentation/rest/).

## Criar um objeto personalizado para uma estrutura de muitas para muitas {#create-a-custom-object-for-a-many-to-many-structure}

Este exemplo mostra um objeto personalizado de curso, que será usado para criar uma relação muitos para muitos entre pessoas/empresas e cursos. Quando terminar, você criará um objeto intermediário para conectá-lo às pessoas ou empresas em seu banco de dados.

>[!NOTE]
>
>Para uma relação muitos para muitos, não é necessário criar um link no objeto personalizado. Em vez disso, você adicionará dois links ao objeto intermediário (veja abaixo).

1. Clique em **Administrador** e em **Gerenciamento de banco de dados** select **Objetos personalizados do Marketo**.

   ![](assets/image2016-1-18-13-3a16-3a25.png)

1. Clique em **Novo objeto personalizado**.

   ![](assets/image2016-5-18-16-3a32-3a42.png)

1. Insira um nome de exibição. O Nome da API e o Nome do Plural são preenchidos automaticamente. Insira uma descrição (opcional).

   ![](assets/image2016-1-14-13-3a38-3a46.png)

   >[!NOTE]
   >
   >Você pode editar esses campos ao criá-los, mas depois que eles forem salvos, você só poderá editar o campo Nome do Plural e o campo **Mostrar em Detalhes do Cliente Potencial** controle deslizante.

1. Puxe a **Mostrar em Detalhes do Cliente Potencial** controle deslizante sobre a exibição **Mostrar** se quiser exibir dados de objeto personalizado na página Banco de Dados de Lead. Clique em **Salvar**.

   ![](assets/image2016-1-14-13-3a42-3a56.png)

1. As informações do objeto personalizado exibem o conteúdo inserido. Observe que está em um estado de Rascunho.

   ![](assets/image2016-1-18-8-3a38-3a58.png)

   >[!NOTE]
   >
   >Você só pode preencher os Objetos Personalizados do Marketo por meio de uma importação de lista ou do [API](https://developers.marketo.com/documentation/rest/).

A próxima etapa é criar o objeto intermediário (veja abaixo). Mas antes disso, é necessário criar um campo para vincular a com ele.

## Criar um objeto intermediário {#create-an-intermediary-object}

Use um objeto intermediário para conectar um objeto personalizado a pessoas ou empresas. Neste exemplo, ele é usado para conectar cursos em seu objeto personalizado do curso a pessoas ou empresas em seu banco de dados.

>[!NOTE]
>
>Não é necessário criar um objeto intermediário para uma estrutura de objeto personalizada de um para muitos.

1. Clique em **Administrador** e em **Gerenciamento de banco de dados**, selecione **Objetos personalizados do Marketo**.

   ![](assets/image2016-1-18-13-3a17-3a40.png)

1. Clique em **Novo objeto personalizado**.

   ![](assets/image2016-5-18-16-3a33-3a16.png)

1. Insira um nome de exibição. O Nome da API e o Nome do Plural são preenchidos automaticamente. Insira uma descrição (opcional).

   ![](assets/image2016-1-14-14-3a10-3a44.png)

   >[!NOTE]
   >
   >É possível editar esses campos ao criá-los, mas depois que eles forem salvos, você só poderá editar o campo Nome do Plural e o controle deslizante Mostrar em Detalhes do lead .

1. Puxe a **Mostrar em Detalhes do Cliente Potencial** controle deslizante sobre a exibição **Mostrar** se quiser exibir dados de objeto personalizado na página Banco de Dados de Lead. Clique em **Salvar**.

   ![](assets/image2016-1-14-14-3a12-3a49.png)

1. As informações do objeto personalizado exibem o conteúdo inserido. Observe que está em um estado de Rascunho.

   O próximo passo é [adicionar campos de link](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md) para conectar seu objeto intermediário a uma pessoa/empresa e um objeto personalizado.

>[!MORELIKETHIS]
>
>* [Adicionar campos de objeto personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Adicionar campos de link de objeto personalizado do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Como entender objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

