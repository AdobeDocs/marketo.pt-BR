---
unique-page-id: 2359663
description: Definir um valor de campo de formulário oculto - Documentos do Marketo - Documentação do produto
title: Definir um valor de campo de formulário oculto
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 2%

---

# Definir um valor de campo de formulário oculto {#set-a-hidden-form-field-value}

Campos ocultos geralmente são preenchidos dinamicamente. Eles não são mostrados ao preenchedor do formulário. Veja como definir o valor.

>[!PREREQUISITES]
>
>[Definir um campo de formulário como Oculto](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## Selecionar o campo {#select-the-field}

1. No formulário, selecione o campo oculto e clique em **Editar** para **Preenchimento Automático**.

   ![](assets/autofill.png)

## Usar valor padrão {#use-default-value}

Ao selecionar Usar valor padrão, é possível codificar um valor específico para ser sempre usado quando esse formulário for enviado. Insira o valor padrão e clique em Salvar.

![](assets/image2014-9-15-13-3a5-3a27.png)

## Parâmetro do URL {#url-parameter}

Se você quiser capturar Parâmetros de URL (Sequências de consulta) da página em que a pessoa está ao preencher o formulário, é possível usar **Parâmetros de URL** para preencher o campo oculto.

>[!NOTE]
>
>Parâmetros são meio técnicos, não são? Uma vez que você os tenha, eles são poderosos. Essa [Página da Wikipédia sobre sequências de consulta](https://en.wikipedia.org/wiki/Query_string) é um pouco útil.

1. Selecionar **Parâmetro de URL** para **Obter tipo de valor**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Insira o **Nome do parâmetro** e clique em **Salvar**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Você pode inserir um valor padrão caso o parâmetro do URL não seja encontrado.

## Valor do cookie {#cookie-value}

Se você estiver armazenando dados em cookies, poderá usar **Valor do cookie** para coletar dados quando o formulário for enviado.

1. Selecionar **Valor do cookie** para **Obter valor de**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Insira o Nome do parâmetro do cookie desejado e clique em **Salvar**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Você pode inserir um valor padrão caso o parâmetro/cookie não seja encontrado.

## URL direcional {#referrer-parameter}

Se você quiser capturar dados da página de onde o visitante veio antes de preencher o formulário, é possível usar **Parâmetro referenciador**.

1. Definir **Obter valor de** para **Parâmetro referenciador**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Insira o **Nome do parâmetro** que você deseja ajustar do URL do referenciador e clique em **Salvar**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Você pode inserir um **Valor padrão** caso o parâmetro referrer não seja encontrado.

1. Clique em **Concluir**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Clique em **Aprovar e fechar**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
