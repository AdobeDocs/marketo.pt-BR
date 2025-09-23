---
unique-page-id: 2359663
description: Definir um valor de campo de formulário oculto - Documentação do Marketo - Documentação do produto
title: Definir um valor de campo de formulário oculto
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 7%

---

# Definir um valor de campo de formulário oculto {#set-a-hidden-form-field-value}

Campos ocultos geralmente são preenchidos dinamicamente. Elas não são mostradas à pessoa que preenche o formulário. Veja como definir o valor.

>[!PREREQUISITES]
>
>[Definir um campo de formulário como oculto](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## Selecionar o campo {#select-the-field}

1. No seu formulário, selecione o campo oculto e clique em **[!UICONTROL Editar]** para **[!UICONTROL Preenchimento Automático]**.

   ![](assets/autofill.png)

## Usar valor padrão {#use-default-value}

Ao selecionar Usar **[!UICONTROL Valor Padrão]**, você pode codificar um valor específico para ser sempre usado quando este formulário for enviado. Insira o **[!UICONTROL Valor padrão]** e clique em **[!UICONTROL Salvar]**.

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL Parameter {#url-parameter}

Se você quiser capturar Parâmetros de URL (Cadeias de Caracteres de Consulta) da página em que a pessoa está ao preencher o formulário, você poderá usar **[!UICONTROL Parâmetros de URL]** para preencher seu campo oculto.

>[!NOTE]
>
>Parâmetros são meio técnicos, não são? Uma vez que você os pega, eles são poderosos. Esta [página da Wikipédia sobre Cadeias de Caracteres de Consulta](https://en.wikipedia.org/wiki/Query_string) é um pouco útil.

1. Selecione o **[!UICONTROL Parâmetro de URL]** para **[!UICONTROL Obter Tipo de Valor]**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Insira o **[!UICONTROL Nome do Parâmetro]** e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Você pode inserir um **[!UICONTROL Valor padrão]** caso o parâmetro de URL não seja encontrado.

## Valor do cookie {#cookie-value}

Se estiver armazenando dados em cookies, você pode usar o **[!UICONTROL Valor do Cookie]** para coletar dados quando o formulário for enviado.

1. Selecione **[!UICONTROL Valor do Cookie]** para **[!UICONTROL Obter Valor de]**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Insira o cookie **[!UICONTROL Nome do parâmetro]** desejado e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Você pode inserir um **[!UICONTROL Valor padrão]** caso o parâmetro/cookie não seja encontrado.

## URL direcional {#referrer-parameter}

Se quiser capturar dados da página de origem do visitante antes de preencher o formulário, você pode usar o **[!UICONTROL Parâmetro do referenciador]**.

1. Definir **[!UICONTROL Obter Valor de]** para **[!UICONTROL Parâmetro do Referenciador]**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Insira o **[!UICONTROL Nome do Parâmetro]** que você deseja assimilar da URL do referenciador e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Você pode inserir um **[!UICONTROL Valor padrão]** caso o parâmetro referenciador não seja encontrado.

1. Clique em **[!UICONTROL Concluir]**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Clique em **[!UICONTROL Aprovar e Fechar]**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
