---
unique-page-id: 2949962
description: Alternar dinamicamente a visibilidade de um campo de formulário - Documentos de marketing - Documentação do produto
title: Alternar dinamicamente a visibilidade de um campo de formulário
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---


# Alternar dinamicamente a visibilidade de um campo de formulário {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Adicionar uma lista de seleção de país ao formulário](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)


Um recurso muito interessante dos formulários do Marketing é que você pode ocultar/mostrar dinamicamente campos de formulário ou [conjuntos de campos](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Exemplo**
>
>Neste exemplo, vamos ocultar o campo **State** a menos que **Country** esteja selecionado como &quot;Estados Unidos&quot;.

1. Vá para **Atividades de marketing**.

   ![](assets/login-marketing-activities-8.png)

1. Selecione o formulário e clique em **Editar formulário**.

   ![](assets/editform-1.png)

1. Selecione o campo que deseja ocultar/mostrar dinamicamente e clique no link para **Regras de visibilidade**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Localize e selecione o campo ao redor do qual deseja criar uma condição.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Selecione o operador.

   >[!TIP]
   >
   >Isso é legal porque você pode escolher correspondências indistintas como &quot;start com&quot;.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Selecione os valores que deseja procurar e clique fora da lista suspensa.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Você pode selecionar vários valores clicando neles enquanto a lista suspensa está aberta. Por exemplo, você pode selecionar Estados Unidos e Canadá.

   >[!NOTE]
   >
   >Nós anteriormente convertemos País em um tipo de campo de lista de separação e [adicionamos todos os países como valores](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Clique em **Salvar**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

E é isso! Agora, quando as pessoas preencherem este formulário e selecionarem Estados Unidos para o país, o campo Estado aparecerá dinamicamente com as opções especificadas.
