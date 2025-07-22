---
unique-page-id: 2949962
description: Alternar dinamicamente a visibilidade de um campo de formulário - Documentação do Marketo - Documentação do produto
title: Alternar dinamicamente a visibilidade de um campo de formulário
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
feature: Forms
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 2%

---

# Alternar dinamicamente a visibilidade de um campo de formulário {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Adicionar uma lista de opções do país ao seu formulário](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

Um recurso muito interessante dos formulários do Marketo é que você pode ocultar/mostrar dinamicamente campos ou [conjuntos de campos](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Exemplo**
>
>Neste exemplo, vamos ocultar o campo **Estado**, a menos que **País** esteja selecionado como &quot;Estados Unidos&quot;.

1. Vá para **[!UICONTROL Atividades de marketing]**.

   ![](assets/login-marketing-activities-8.png)

1. Selecione seu formulário e clique em **[!UICONTROL Editar Formulário]**.

   ![](assets/editform-1.png)

1. Selecione o campo que deseja ocultar/mostrar dinamicamente e clique no link para **[!UICONTROL Regras de visibilidade]**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Localize e selecione o campo no qual deseja criar uma condição.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Selecione o operador.

   >[!TIP]
   >
   >Isso é legal porque você pode escolher correspondências difusas como &quot;[!UICONTROL começa com]&quot;.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Selecione os valores a serem procurados e clique fora do menu suspenso.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Você pode selecionar vários valores clicando neles enquanto o menu suspenso estiver aberto. Por exemplo, você pode selecionar Estados Unidos e Canadá.

   >[!NOTE]
   >
   >Anteriormente convertemos País em um tipo de campo de lista de opções e [adicionamos todos os países como valores](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

E é isso! Agora, quando as pessoas preencherem este formulário e selecionarem Estados Unidos por país, o campo Estado aparecerá dinamicamente com as opções especificadas.

>[!IMPORTANT]
>
>O comportamento do campo de formulário funcionará perfeitamente quando os valores de campo forem definidos/atualizados por meio de script personalizado usando [funções de API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/forms-api-reference){target="_blank"} no Forms 2.0.
>
>Campos condicionais podem não funcionar como esperado se os valores de campo forem modificados por scripts externos diferentes da API do JavaScript do Forms 2.0.
