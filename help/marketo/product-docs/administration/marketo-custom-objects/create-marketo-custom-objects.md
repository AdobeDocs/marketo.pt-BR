---
unique-page-id: 10093192
description: Etapas para criar objetos personalizados do Marketo para estruturas de um para muitos ou de muitos para muitos, incluindo nome de exibição, nome da API e Exibir em detalhes de cliente potencial.
title: Criar objetos personalizados do Marketo
exl-id: d68b41e1-a12b-436f-aad7-42c7264cd901
feature: Custom Objects
TQID: https://experienceleague.adobe.com/ORgicNbsK5gDy67zbW7EzMgcpjZr4U2UNENeoWboeO8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 771
ht-degree: 4%

---

# Criar objetos personalizados do Marketo {#create-marketo-custom-objects}

Use objetos personalizados no Marketo para rastrear métricas específicas para sua empresa. Pode ser qualquer coisa, de carros a cursos, o que você quiser como modelo no Marketo para executar suas campanhas.

>[!NOTE]
>
>Você pode configurar objetos personalizados para funcionarem de um para muitos ou de muitos para muitos. Você cria o objeto inicial da mesma maneira, mas as etapas são diferentes quando começa a adicionar campos ao objeto. Consulte [Entendendo os objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) para obter mais informações.

>[!NOTE]
>
>Não é possível criar, editar ou excluir um Link ou Campo de desduplicação depois que o objeto personalizado é aprovado.

## Criar um objeto personalizado para uma estrutura de um para muitos {#create-a-custom-object-for-a-one-to-many-structure}

Este exemplo mostra um objeto personalizado Car para uso em uma estrutura de um para muitos. Posteriormente, você criará um objeto personalizado do curso e um objeto intermediário para usar em uma estrutura muitos para muitos.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/create-marketo-custom-objects-1.png)

1. Clique em **[!UICONTROL Objetos personalizados do Marketo]**.

   ![](assets/create-marketo-custom-objects-2.png)

1. Clique em **[!UICONTROL Novo objeto personalizado]**.

   ![](assets/create-marketo-custom-objects-3.png)

   >[!NOTE]
   >
   >A guia [!UICONTROL Objetos Personalizados do Marketo] exibe todos os objetos personalizados à direita e detalhes de todos os aprovados, incluindo o número de registros e campos na atualização mais recente.

1. Insira um [!UICONTROL Nome para Exibição]. O [!UICONTROL Nome da API] e o [!UICONTROL Nome do Plural] são preenchidos automaticamente. Insira uma [!UICONTROL Descrição] (opcional).

   ![](assets/create-marketo-custom-objects-4.png)

   >[!NOTE]
   >
   >Você pode editar esses campos ao criá-los, mas depois de salvá-los, você só poderá editar o campo [!UICONTROL Nome no Plural] e o controle deslizante **[!UICONTROL Mostrar em Detalhes do Cliente Potencial]**.

1. Puxe o controle deslizante **[!UICONTROL Mostrar em Detalhes do Cliente Potencial]** para exibir **[!UICONTROL Mostrar]** se desejar exibir dados do objeto personalizado na página Banco de Dados. Clique em **[!UICONTROL Salvar]**.

   ![](assets/create-marketo-custom-objects-5.png)

1. As informações do objeto personalizado exibem o conteúdo inserido. Observe que ele está no estado **[!UICONTROL Rascunho]**.

   ![](assets/create-marketo-custom-objects-6.png)

   A próxima etapa é adicionar campos para [criar seu objeto personalizado](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md).

   >[!NOTE]
   >
   >Você só pode preencher Objetos Personalizados do Marketo por meio de uma importação de lista ou pela [API](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api).

## Criar um objeto personalizado para uma estrutura muitos para muitos {#create-a-custom-object-for-a-many-to-many-structure}

Este exemplo mostra um objeto personalizado do curso, que você usará para criar uma relação muitos para muitos entre pessoas ou empresas e cursos. Quando terminar, você criará um objeto intermediário para conectá-lo às pessoas ou empresas no banco de dados.

>[!NOTE]
>
>Para uma relação muitos para muitos, não é necessário criar um link no objeto personalizado. Em vez disso, você adicionará dois links ao objeto intermediário (veja abaixo).

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/create-marketo-custom-objects-7.png)

1. Clique em **[!UICONTROL Objetos personalizados do Marketo]**.

   ![](assets/create-marketo-custom-objects-8.png)

1. Clique em **[!UICONTROL Novo objeto personalizado]**.

   ![](assets/create-marketo-custom-objects-9.png)

1. Insira um [!UICONTROL Nome para Exibição]. O [!UICONTROL Nome da API] e o [!UICONTROL Nome do Plural] são preenchidos automaticamente. Insira uma [!UICONTROL Descrição] (opcional).

   ![](assets/create-marketo-custom-objects-10.png)

   >[!NOTE]
   >
   >Você pode editar esses campos ao criá-los, mas depois de salvá-los, você só poderá editar o campo [!UICONTROL Nome no Plural] e o controle deslizante **[!UICONTROL Mostrar em Detalhes do Cliente Potencial]**.

1. Puxe o controle deslizante **[!UICONTROL Mostrar em Detalhes do Cliente Potencial]** para exibir **[!UICONTROL Mostrar]** se desejar exibir dados do objeto personalizado na página Banco de Dados. Clique em **[!UICONTROL Salvar]**.

   ![](assets/create-marketo-custom-objects-11.png)

1. As informações do objeto personalizado exibem o conteúdo inserido. Observe que ele está no estado **[!UICONTROL Rascunho]**.

   ![](assets/create-marketo-custom-objects-12.png)

   >[!NOTE]
   >
   >Você só pode preencher Objetos Personalizados do Marketo por meio de uma importação de lista ou pela [API](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api).

A próxima etapa é criar o objeto intermediário (veja abaixo). Antes disso, é necessário criar um campo para vincular com ele.

## Criar um Objeto Intermediário {#create-an-intermediary-object}

Use um objeto intermediário para conectar um objeto personalizado a pessoas ou empresas. Neste exemplo, ele é usado para conectar cursos no objeto personalizado do curso a pessoas ou empresas no banco de dados.

>[!NOTE]
>
>Não é necessário criar um objeto intermediário para uma estrutura de objeto personalizado de um para muitos.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/create-marketo-custom-objects-13.png)

1. Clique em **[!UICONTROL Objetos personalizados do Marketo]**.

   ![](assets/create-marketo-custom-objects-14.png)

1. Clique em **[!UICONTROL Novo objeto personalizado]**.

   ![](assets/create-marketo-custom-objects-15.png)

1. Insira um [!UICONTROL Nome para Exibição]. O [!UICONTROL Nome da API] e o [!UICONTROL Nome do Plural] são preenchidos automaticamente. Insira uma [!UICONTROL Descrição] (opcional).

   ![](assets/create-marketo-custom-objects-16.png)

   >[!NOTE]
   >
   >Você pode editar esses campos ao criá-los, mas depois de salvá-los, você só poderá editar o campo [!UICONTROL Nome no Plural] e o controle deslizante [!UICONTROL Mostrar em Detalhes do Cliente Potencial].

1. Puxe o controle deslizante **[!UICONTROL Mostrar em Detalhes do Cliente Potencial]** para exibir **[!UICONTROL Mostrar]** se desejar exibir dados do objeto personalizado na página Banco de Dados. Clique em **[!UICONTROL Salvar]**.

   ![](assets/create-marketo-custom-objects-17.png)

1. As informações do objeto personalizado exibem o conteúdo inserido. Observe que ele está no estado **[!UICONTROL Rascunho]**.

   A próxima etapa é [adicionar campos de link](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md) para conectar seu objeto intermediário a uma pessoa ou empresa e a um objeto personalizado.

>[!MORELIKETHIS]
>
>* [Adicionar campos de objeto personalizado do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Adicionar campos de link de objeto personalizado do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Noções básicas sobre objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
