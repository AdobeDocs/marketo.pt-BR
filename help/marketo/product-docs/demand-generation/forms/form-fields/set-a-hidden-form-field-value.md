---
unique-page-id: 2359663
description: Definir um valor de campo de formulário oculto - Documentos de marketing - Documentação do produto
title: Definir um valor de campo de formulário oculto
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---


# Definir um valor de campo de formulário oculto {#set-a-hidden-form-field-value}

Campos ocultos normalmente são preenchidos dinamicamente. Elas não são mostradas à pessoa que preenche o formulário. Veja como definir o valor.

>[!NOTE]
>
>**Pré-requisitos**
>
>[Definir um campo de formulário como oculto](set-a-form-field-as-hidden.md)

## Selecionar o campo {#select-the-field}

1. No formulário, selecione o campo oculto e clique em **Editar** para preenchimento **automático**.

   ![](assets/autofill.png)

## Usar valor padrão {#use-default-value}

Ao selecionar Usar valor padrão, é possível codificar um valor específico para ser sempre usado quando esse formulário for enviado. Insira o Valor padrão e clique em Salvar.

![](assets/image2014-9-15-13-3a5-3a27.png)

## Parâmetro de URL {#url-parameter}

Se desejar capturar Parâmetros de URL (Strings de Query) da página em que a pessoa está ao preencher o formulário, você pode usar **Parâmetros** de **URL** para preencher o campo oculto.

>[!NOTE]
>
>Parâmetros são meio técnicos, não são? Uma vez que você os pega, eles são poderosos. Esta página da [Wikipedia sobre Strings](http://en.wikipedia.org/wiki/Query_string) de Query é útil.

1. Selecione Parâmetro **de** URL para Tipo **de** Obtenção de Valor.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Digite o Nome **do** parâmetro e clique em **Salvar**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Você pode inserir um Valor padrão caso o parâmetro de URL não seja encontrado.

## Valor do cookie {#cookie-value}

Se você estiver armazenando dados em cookies, poderá usar **Cookie** **Value** para coletar dados quando o formulário for enviado.

1. Selecione **Cookie** **Value** para **Obter** **valor** **de**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Digite o Nome do parâmetro do cookie desejado e clique em **Salvar**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Você pode inserir um Valor padrão caso o parâmetro/cookie não seja encontrado.

## Parâmetro de quem indicou {#referrer-parameter}

Se você quiser capturar dados da página de onde o visitante veio antes de preencher o formulário, use o **Quem indicou** **Parâmetro**.

1. Defina **Obter** **valor** **de** para **Quem indicou** **Parâmetro**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Digite o Nome **do** parâmetro que você deseja ajustar do URL da quem indicou e clique em **Salvar**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Você pode inserir um **Valor** **Padrão** caso o parâmetro de quem indicou não seja encontrado.

1. Clique em **Concluir**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Clique em **Aprovar e fechar**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)

Doce! Você está indo muito bem. Há mais para aprender sobre [formas](http://docs.marketo.com/display/docs/forms).
