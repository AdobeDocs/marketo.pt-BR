---
unique-page-id: 2949962
description: Alternar dinamicamente a visibilidade de um campo de formulário - Documentos de marketing - Documentação do produto
title: Alternar dinamicamente a visibilidade de um campo de formulário
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---


# Alternar dinamicamente a visibilidade de um campo de formulário {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Adicionar uma lista de seleção de país ao formulário](../../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

>



Um recurso muito interessante dos formulários do Marketing é que é possível ocultar/mostrar dinamicamente campos ou [conjuntos de campos](add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Exemplo**
>
>Neste exemplo, vamos ocultar o campo **Estado** , a menos que **País** esteja selecionado como &quot;Estados Unidos&quot;.

1. Vá para **Marketing** **Atividade**.

   ![](assets/login-marketing-activities-8.png)

1. Selecione o formulário e clique em **Editar** **formulário**.

   ![](assets/editform-1.png)

1. Selecione o campo que deseja ocultar/mostrar dinamicamente e clique no link para **Regras** de visibilidade ****.

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
   >Nós anteriormente convertemos País em um tipo de campo de lista de separação e [adicionamos todos os países como valores](../../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Clique em **Salvar**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

E é isso! Agora, quando as pessoas preencherem este formulário e selecionarem Estados Unidos para o país, o campo Estado aparecerá dinamicamente com as opções especificadas.

>[!NOTE]
>
>**Mergulho profundo**
>
>Quer saber mais sobre [formulários](http://docs.marketo.com/display/docs/forms)?

