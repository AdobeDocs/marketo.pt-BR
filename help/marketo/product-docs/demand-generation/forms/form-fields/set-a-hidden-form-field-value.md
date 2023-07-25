---
unique-page-id: 2359663
description: Definir um valor de campo de formulário oculto - Documentação do Marketo - Documentação do produto
title: Definir um valor de campo de formulário oculto
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 2%

---

# Definir um valor de campo de formulário oculto {#set-a-hidden-form-field-value}

Campos ocultos geralmente são preenchidos dinamicamente. Elas não são mostradas à pessoa que preenche o formulário. Veja como definir o valor.

>[!PREREQUISITES]
>
>[Definir um campo de formulário como oculto](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## Selecionar o campo {#select-the-field}

1. No formulário, selecione o campo oculto e clique em **Editar** para **Preenchimento automático**.

   ![](assets/autofill.png)

## Usar valor padrão {#use-default-value}

Ao selecionar Usar valor padrão, você pode codificar um valor específico para ser sempre usado quando este formulário for enviado. Insira o Valor padrão e clique em Salvar.

![](assets/image2014-9-15-13-3a5-3a27.png)

## Parâmetro do URL {#url-parameter}

Se você quiser capturar os Parâmetros de URL (Cadeias de caracteres de consulta) da página em que a pessoa está ao preencher o formulário, você pode usar **Parâmetros de URL** para preencher o campo oculto.

>[!NOTE]
>
>Parâmetros são meio técnicos, não são? Uma vez que você os pega, eles são poderosos. Este [Página da Wikipédia em sequências de consulta](https://en.wikipedia.org/wiki/Query_string) é um pouco útil.

1. Selecionar **Parâmetro de URL** para **Obter Tipo de Valor**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Insira o **Nome do parâmetro** e clique em **Salvar**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Você pode inserir um Valor padrão caso o parâmetro de URL não seja encontrado.

## Valor do cookie {#cookie-value}

Se estiver armazenando dados em cookies, você pode usar **Valor do cookie** para coletar dados quando o formulário for enviado.

1. Selecionar **Valor do cookie** para **Obter valor de**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Insira o Nome do parâmetro do cookie desejado e clique em **Salvar**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Você pode inserir um Valor padrão caso o parâmetro/cookie não seja encontrado.

## URL direcional {#referrer-parameter}

Se quiser capturar dados da página de onde o visitante veio antes de preencher o formulário, você pode usar **Parâmetro do referenciador**.

1. Definir **Obter valor de** para **Parâmetro do referenciador**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Insira o **Nome do parâmetro** que você deseja extrair do URL do referenciador e clicar em **Salvar**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Você pode inserir um **Valor padrão** caso o parâmetro referrer não seja encontrado.

1. Clique em **Concluir**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Clique em **Aprovar e fechar**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
