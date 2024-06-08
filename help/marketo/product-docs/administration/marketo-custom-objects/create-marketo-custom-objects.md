---
unique-page-id: 10093192
description: Criar objetos personalizados do Marketo - Documentação do Marketo - Documentação do produto
title: Criar objetos personalizados do Marketo
exl-id: d68b41e1-a12b-436f-aad7-42c7264cd901
feature: Custom Objects
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

# Criar objetos personalizados do Marketo {#create-marketo-custom-objects}

Use objetos personalizados no Marketo para rastrear métricas específicas para sua empresa. Pode ser de carros a cursos, seja qual for o modelo que você queira usar no Marketo para executar suas campanhas.

>[!NOTE]
>
>Você pode configurar objetos personalizados para funcionarem de um para muitos ou de muitos para muitos. Você cria o objeto inicial da mesma maneira, mas as etapas são diferentes quando começa a adicionar campos ao objeto. Consulte  [Noções básicas sobre objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) para obter mais informações.

>[!NOTE]
>
>Não é possível criar, editar ou excluir um Link ou Campo de desduplicação depois que o objeto personalizado é aprovado.

## Criar um objeto personalizado para uma estrutura de um para muitos {#create-a-custom-object-for-a-one-to-many-structure}

Este exemplo mostra um objeto personalizado Car para uso em uma estrutura de um para muitos. Posteriormente, você criará um objeto personalizado do curso e um objeto intermediário para usar em uma estrutura muitos para muitos.

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/create-marketo-custom-objects-1.png)

1. Clique em **[!UICONTROL Objetos personalizados do Marketo]**.

   ![](assets/create-marketo-custom-objects-2.png)

1. Clique em **[!UICONTROL Novo objeto personalizado]**.

   ![](assets/create-marketo-custom-objects-3.png)

   >[!NOTE]
   >
   >A variável [!UICONTROL Objetos personalizados do Marketo] A guia exibe todos os objetos personalizados à direita e detalhes de todos os aprovados, incluindo o número de registros e campos na atualização mais recente.

1. Insira um [!UICONTROL Nome de exibição]. A variável [!UICONTROL Nome da API] e [!UICONTROL Nome no Plural] preencha automaticamente. Insira um [!UICONTROL Descrição] (opcional).

   ![](assets/create-marketo-custom-objects-4.png)

   >[!NOTE]
   >
   >Você pode editar esses campos ao criá-los, mas depois que eles forem salvos, você só poderá editar o campo [!UICONTROL Nome no Plural] e o campo **[!UICONTROL Mostrar em Detalhes de Cliente Potencial]** controle deslizante.

1. Puxe a **[!UICONTROL Mostrar em Detalhes de Cliente Potencial]** controle deslizante sobre para exibir **[!UICONTROL Mostrar]** se quiser exibir dados do objeto personalizado na página Banco de Dados. Clique em **[!UICONTROL Salvar]**.

   ![](assets/create-marketo-custom-objects-5.png)

1. As informações do objeto personalizado exibem o conteúdo inserido. Observe que está em um estado Rascunho.

   ![](assets/create-marketo-custom-objects-6.png)

   A próxima etapa é adicionar campos a [crie seu objeto personalizado](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md).

   >[!NOTE]
   >
   >Você só pode preencher Objetos personalizados do Marketo por meio de uma importação de lista ou pelo [API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api).

## Criar um objeto personalizado para uma estrutura muitos para muitos {#create-a-custom-object-for-a-many-to-many-structure}

Este exemplo mostra um objeto personalizado do curso, que você usará para criar uma relação muitos para muitos entre pessoas/empresas e cursos. Quando terminar, você criará um objeto intermediário para conectá-lo às pessoas ou empresas no banco de dados.

>[!NOTE]
>
>Para uma relação muitos para muitos, não é necessário criar um link no objeto personalizado. Em vez disso, você adicionará dois links ao objeto intermediário (veja abaixo).

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/create-marketo-custom-objects-7.png)

1. Clique em **[!UICONTROL Objetos personalizados do Marketo]**.

   ![](assets/create-marketo-custom-objects-8.png)

1. Clique em **[!UICONTROL Novo objeto personalizado]**.

   ![](assets/create-marketo-custom-objects-9.png)

1. Insira um [!UICONTROL Nome de exibição]. A variável [!UICONTROL Nome da API] e [!UICONTROL Nome no Plural] preencha automaticamente. Insira um [!UICONTROL Descrição] (opcional).

   ![](assets/create-marketo-custom-objects-10.png)

   >[!NOTE]
   >
   >Você pode editar esses campos ao criá-los, mas depois que eles forem salvos, você só poderá editar o campo [!UICONTROL Nome no Plural] e o campo **[!UICONTROL Mostrar em Detalhes de Cliente Potencial]** controle deslizante.

1. Puxe a **[!UICONTROL Mostrar em Detalhes de Cliente Potencial]** controle deslizante sobre para exibir **[!UICONTROL Mostrar]** se quiser exibir dados do objeto personalizado na página Banco de Dados. Clique em **[!UICONTROL Salvar]**.

   ![](assets/create-marketo-custom-objects-11.png)

1. As informações do objeto personalizado exibem o conteúdo inserido. Observe que está em um estado Rascunho.

   ![](assets/create-marketo-custom-objects-12.png)

   >[!NOTE]
   >
   >Você só pode preencher Objetos personalizados do Marketo por meio de uma importação de lista ou pelo [API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api).

A próxima etapa é criar o objeto intermediário (veja abaixo). Mas antes disso, é necessário criar um campo para vincular com ele.

## Criar um Objeto Intermediário {#create-an-intermediary-object}

Use um objeto intermediário para conectar um objeto personalizado a pessoas ou empresas. Neste exemplo, ele é usado para conectar cursos no objeto personalizado do curso a pessoas ou empresas no banco de dados.

>[!NOTE]
>
>Não é necessário criar um objeto intermediário para uma estrutura de objeto personalizado de um para muitos.

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/create-marketo-custom-objects-13.png)

1. Clique em **[!UICONTROL Objetos personalizados do Marketo]**.

   ![](assets/create-marketo-custom-objects-14.png)

1. Clique em **[!UICONTROL Novo objeto personalizado]**.

   ![](assets/create-marketo-custom-objects-15.png)

1. Insira um [!UICONTROL Nome de exibição]. A variável [!UICONTROL Nome da API] e [!UICONTROL Nome no Plural] preencha automaticamente. Insira um [!UICONTROL Descrição] (opcional).

   ![](assets/create-marketo-custom-objects-16.png)

   >[!NOTE]
   >
   >Você pode editar esses campos ao criá-los, mas depois que eles forem salvos, você só poderá editar o campo [!UICONTROL Nome no Plural] e o campo [!UICONTROL Mostrar em Detalhes de Cliente Potencial] controle deslizante.

1. Puxe a **[!UICONTROL Mostrar em Detalhes de Cliente Potencial]** controle deslizante sobre para exibir **Mostrar** se quiser exibir dados do objeto personalizado na página Banco de Dados. Clique em **Salvar**.

   ![](assets/create-marketo-custom-objects-17.png)

1. As informações do objeto personalizado exibem o conteúdo inserido. Observe que está em um estado Rascunho.

   A próxima etapa é que você [adicionar campos de link](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md) para conectar seu objeto intermediário a uma pessoa/empresa e um objeto personalizado.

>[!MORELIKETHIS]
>
>* [Adicionar campos de objeto personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Adicionar campos de link de objeto personalizado do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Noções básicas sobre objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
