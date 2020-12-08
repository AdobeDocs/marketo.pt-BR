---
unique-page-id: 1900554
description: Editar um HTML de email - Documentos do marketing - Documentação do produto
title: Editar o HTML de um email
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Editar o HTML de um email {#edit-an-emails-html}

Às vezes, pode ser necessário modificar o HTML subjacente de um email. Às vezes, você pode usar um sistema externo para projetar e criar o código do seu email. De qualquer forma, você pode importar e/ou editar facilmente o código no editor de email.

## Editar HTML {#edit-html}

1. Selecione seu email e clique em **Editar rascunho**.

   ![](assets/teamspidey.jpg)

1. Clique em **Editar código**.

   ![](assets/two-4.png)

1. Faça quaisquer alterações. Clique em **Salvar** quando concluído.

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >Mude o que quiser. Você pode substituir o HTML inteiro ou fazer pequenos ajustes.

1. Clique no menu suspenso Ações **de** código para baixar o código como um arquivo .html, embutir seu CSS ou validar o HTML.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >A melhor prática para emails é tornar todos os seus estilos em linha. Vários clientes de email não suportam CSS na `<head>` seção.

## Quebrando um email de seu modelo {#breaking-an-email-from-its-template}

Essas alterações de código não **** quebrarão um email do modelo:

* Editar o conteúdo de qualquer módulo (incluindo a adição de novos elementos dentro do módulo)
* Adicionando um novo módulo ao Container
* Excluindo um módulo do Container

* Alteração de atributos específicos de mkto (por exemplo, &quot;mktoName&quot; ou &quot;mktoImgUrl&quot;) de qualquer Elemento fora de um Módulo
* Editar o conteúdo de qualquer Elemento (rich text, imagem, vídeo etc.) fora de um módulo

Esses itens que você pode fazer no editor de código **quebrarão** o email do modelo:

* Alteração de qualquer item no código fora de um elemento ou módulo
* Adicionar ou alterar atributos não mkto (por exemplo, &quot;id&quot; ou &quot;style&quot;) de qualquer Elemento fora de um Módulo
* Excluindo um elemento que esteja fora de um módulo

## Código de pesquisa {#search-code}

Use a funcionalidade Pesquisar código para localizar e substituir conteúdo com eficiência dentro do código HTML do seu email.

1. No código do seu email, clique em Código **de** pesquisa.

   ![](assets/five-2.png)

1. Digite o que deseja localizar e clique em **Localizar próximo** para pesquisar para frente ou em **Localizar anterior** para pesquisar para trás. Você também tem a opção de **Substituir** e **Substituir tudo**.

   ![](assets/six-1.png)

1. Clique em **Fechar** quando terminar.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >O Código de pesquisa também está disponível no editor [de modelo de](http://docs.marketo.com/display/DOCS/Create+a+New+Email+Template)email.

Recomendamos que você continue editando seus emails usando a funcionalidade integrada do Marketo, mas esse editor de código oferece flexibilidade se você precisar.
