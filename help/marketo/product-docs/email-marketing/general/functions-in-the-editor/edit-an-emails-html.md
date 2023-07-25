---
unique-page-id: 1900554
description: Edite o HTML de um email - Documentação do Marketo - Documentação do produto
title: Editar um HTML de email
exl-id: 9dc8e44d-d9da-4bc2-950f-3ffbb976f5d5
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 1%

---

# Editar um HTML de email {#edit-an-emails-html}

Às vezes, pode ser necessário modificar o HTML subjacente de um email. Às vezes, você pode usar um sistema externo para projetar e criar o código do seu email. De qualquer maneira, você pode importar e/ou editar facilmente o código do no editor de email.

## Editar HTML {#edit-html}

1. Selecione seu email e clique em **Editar rascunho**.

   ![](assets/teamspidey.jpg)

1. Clique em **Editar código**.

   ![](assets/two-4.png)

1. Faça as alterações. Clique em **Salvar** quando terminar.

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >Mude o que quiser. Você pode substituir o HTML inteiro ou fazer pequenos ajustes.

1. Clique em **Ações de código** para baixar o código como um arquivo .html, embutir seu CSS ou validar o HTML.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >A prática recomendada para emails é tornar todos os estilos em linha. Vários clientes de email não são compatíveis com CSS no `<head>` seção.

## Quebra de um email de seu modelo {#breaking-an-email-from-its-template}

Essas alterações de código **não** Interromper um email com base em seu modelo:

* Editar o conteúdo de qualquer módulo (incluindo adicionar novos elementos dentro do módulo)
* Adicionar um novo módulo ao contêiner
* Excluindo um módulo do contêiner

* Alteração de atributos específicos do mkto (por exemplo, &quot;mktoName&quot; ou &quot;mktoImgUrl&quot;) de qualquer Elemento fora de um Módulo
* Editar o conteúdo de qualquer elemento (rich text, imagem, vídeo etc.) fora de um módulo

Estas coisas que você pode fazer no editor de código **irá** separar o email do modelo:

* Alterar qualquer coisa no código fora de um elemento ou módulo
* Adicionar ou alterar atributos não mkto (por exemplo, &quot;id&quot; ou &quot;style&quot;) de qualquer elemento fora de um módulo
* Excluindo um elemento que está fora de um módulo

## Código de pesquisa {#search-code}

Use a funcionalidade Código de pesquisa para localizar e substituir com eficiência o conteúdo no código de HTML do seu email.

1. No código do seu email, clique em **Código de pesquisa**.

   ![](assets/five-2.png)

1. Insira o que deseja localizar e clique em **Localizar próximo** para pesquisar para frente ou **Localizar anterior** para pesquisar para trás. Você também tem a opção de **Substituir** e **Substituir tudo**.

   ![](assets/six-1.png)

1. Clique em **Fechar** quando terminar.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >O Código de pesquisa também está disponível no [Editor de modelo de email](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md).

Recomendamos que você continue a editar seus emails usando a funcionalidade integrada do Marketo, mas esse editor de código oferece flexibilidade se você precisar.
