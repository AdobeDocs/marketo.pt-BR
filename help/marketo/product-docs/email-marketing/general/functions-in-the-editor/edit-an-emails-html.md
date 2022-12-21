---
unique-page-id: 1900554
description: Editar um HTML de email - Documentos do Marketo - Documentação do produto
title: Editar o HTML de um email
exl-id: 9dc8e44d-d9da-4bc2-950f-3ffbb976f5d5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 1%

---

# Editar o HTML de um email {#edit-an-emails-html}

Às vezes, pode ser necessário modificar o HTML subjacente de um email. Às vezes, você pode usar um sistema externo para projetar e criar o código do seu email. De qualquer maneira, você pode importar e/ou editar facilmente o código de dentro do editor de email.

## Editar HTML {#edit-html}

1. Selecione seu email e clique em **Editar rascunho**.

   ![](assets/teamspidey.jpg)

1. Clique em **Editar código**.

   ![](assets/two-4.png)

1. Faça qualquer alteração. Clique em **Salvar** quando concluído.

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >Mude o que quiser. Você pode substituir o HTML inteiro ou fazer pequenos ajustes.

1. Clique no botão **Ações do código** para baixar o código como um arquivo .html, embutir seu CSS ou validar o HTML.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >A prática recomendada para emails é tornar todos os seus estilos em linha. Vários clientes de email não suportam CSS no `<head>` seção.

## Quebra de email a partir de seu modelo {#breaking-an-email-from-its-template}

Essas alterações de código **não** quebrar um email de seu template:

* Editar o conteúdo de qualquer Módulo (incluindo a adição de novos Elementos dentro do Módulo)
* Adição de um novo módulo ao contêiner
* Exclusão de um módulo do contêiner

* Alteração de atributos específicos de mkto (por exemplo, &quot;mktoName&quot; ou &quot;mktoImgUrl&quot;) de qualquer elemento fora de um Módulo
* Editar o conteúdo de qualquer elemento (rich text, imagem, vídeo etc.) fora de um módulo

Essas coisas que você pode fazer no editor de código **will** dividir o email do template:

* Alteração de qualquer item do código fora de um elemento ou módulo
* Adicionar ou alterar atributos não mkto (por exemplo, &quot;id&quot; ou &quot;style&quot;) de qualquer elemento fora de um Módulo
* Exclusão de um elemento fora de um módulo

## Código de pesquisa {#search-code}

Use a funcionalidade Pesquisar código para encontrar e substituir com eficiência o conteúdo no código de HTML do seu email.

1. No código do seu email, clique em **Código de pesquisa**.

   ![](assets/five-2.png)

1. Insira o que deseja localizar e clique em **Localizar próximo** para pesquisar ou **Localizar anterior** para pesquisar para trás. Você também tem a opção de **Substituir** e **Substituir tudo**.

   ![](assets/six-1.png)

1. Clique em **Fechar** quando concluído.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >O Código de pesquisa também está disponível na variável [Editor de modelo de email](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md).

Recomendamos que você continue editando seus emails usando a funcionalidade integrada do Marketo, mas esse editor de código fornece flexibilidade se precisar.
