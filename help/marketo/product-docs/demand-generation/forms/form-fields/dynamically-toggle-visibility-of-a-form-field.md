---
unique-page-id: 2949962
description: Alternar dinamicamente a visibilidade de um campo de formulário - Documentos do Marketo - Documentação do produto
title: Alternar dinamicamente a visibilidade de um campo de formulário
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Alternar dinamicamente a visibilidade de um campo de formulário {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Adicionar uma lista de seleção de país ao seu formulário](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)


Um recurso muito interessante do Marketo forms é que você pode ocultar/mostrar dinamicamente campos de formulário ou [fieldsets](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Exemplo**
>
>Neste exemplo, vamos ocultar a variável **Estado** campo exceto **País** é selecionada como &quot;Estados Unidos&quot;.

1. Ir para **Atividades de marketing**.

   ![](assets/login-marketing-activities-8.png)

1. Selecione o formulário e clique em **Editar formulário**.

   ![](assets/editform-1.png)

1. Selecione o campo que deseja ocultar/mostrar dinamicamente e clique no link para **Regras de visibilidade**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Localize e selecione o campo no qual deseja criar uma condição.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Selecione o operador .

   >[!TIP]
   >
   >Isso é legal porque você pode escolher correspondências difusas como &quot;começa com&quot;.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Selecione os valores a serem procurados e clique em fora da lista suspensa.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Você pode selecionar vários valores clicando neles enquanto a lista suspensa está aberta. Por exemplo, é possível selecionar Estados Unidos e Canadá.

   >[!NOTE]
   >
   >anteriormente, convertemos País em um tipo de campo de lista de separação e [adição de todos os países como valores](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Clique em **Salvar**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

E é isso! Agora, quando as pessoas preencherem este formulário e selecionarem Estados Unidos para país, o campo Estado aparecerá dinamicamente com as opções especificadas.
