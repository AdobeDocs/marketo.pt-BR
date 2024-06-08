---
unique-page-id: 2949962
description: Alternar dinamicamente a visibilidade de um campo de formulário - Documentação do Marketo - Documentação do produto
title: Alternar dinamicamente a visibilidade de um campo de formulário
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
feature: Forms
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 1%

---

# Alternar dinamicamente a visibilidade de um campo de formulário {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Adicionar uma lista de opções de país ao formulário](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

Um recurso realmente interessante do Marketo Forms é que você pode ocultar/mostrar campos de formulário dinamicamente ou [fieldsets](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Exemplo**
>
>Neste exemplo, vamos ocultar a variável **Estado** campo, a menos que **País** é selecionado como &quot;Estados Unidos&quot;.

1. Ir para **Atividades de marketing**.

   ![](assets/login-marketing-activities-8.png)

1. Selecione o formulário e clique em **Editar formulário**.

   ![](assets/editform-1.png)

1. Selecione o campo que deseja ocultar/mostrar dinamicamente e clique no link **Regras de visibilidade**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Localize e selecione o campo no qual deseja criar uma condição.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Selecione o operador.

   >[!TIP]
   >
   >Isso é legal porque você pode escolher correspondências difusas como &quot;começa com&quot;.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Selecione os valores a serem procurados e clique fora do menu suspenso.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Você pode selecionar vários valores clicando neles enquanto o menu suspenso estiver aberto. Por exemplo, você pode selecionar Estados Unidos e Canadá.

   >[!NOTE]
   >
   >Anteriormente, convertemos o País em um tipo de campo de lista de opções e [adicionados todos os países como valores](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Clique em **Salvar**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

E é isso! Agora, quando as pessoas preencherem este formulário e selecionarem Estados Unidos por país, o campo Estado aparecerá dinamicamente com as opções especificadas.

>[!IMPORTANT]
>
>O comportamento do campo de formulário funcionará perfeitamente quando os valores de campo forem definidos/atualizados por meio de um script personalizado usando [Funções da API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/forms-api-reference){target="_blank"} no Forms 2.0.
>
>Campos condicionais podem não funcionar como esperado se os valores de campo forem modificados por scripts externos diferentes da API JavaScript do Forms 2.0.
