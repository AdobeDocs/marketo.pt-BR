---
unique-page-id: 10095554
description: Incorporar um formulário a uma campanha da Web - Documentos do Marketo - Documentação do produto
title: Incorporar um formulário a uma campanha da Web
exl-id: 41e60ae6-9a40-444f-8a55-47fc6ef6c5fb
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Incorporar um formulário a uma campanha da Web {#embed-a-form-into-a-web-campaign}

Veja como incorporar um formulário Marketo em uma campanha da Web (Caixa de diálogo, Em zona ou widget).

1. Clique com o botão direito do mouse em um formulário aprovado. Selecionar **Código incorporado**.

   ![](assets/image2015-12-16-10-3a58-3a39.png)

1. Copie o código.

   ![](assets/image2015-12-16-11-3a16-3a24.png)

1. Na Personalização da Web, acesse **Campanhas da Web**.

   ![](assets/web-campaigns-hand-7.jpg)

1. Clique em **Criar Nova Campanha**.

   ![](assets/create-new-web-campaign-hand-1.jpg)

1. No Editor de Rich Text, clique no ícone de HTML.

   ![](assets/five-1.png)

1. Cole o código incorporado do formulário no Editor de fonte do HTML. Clique em **Atualizar**.

   ![](assets/six-1.png)

1. O formulário não será exibido na visualização do editor, mas você pode visualizá-lo para ver como ele será renderizado em uma campanha.

1. Clique em **Launch** para iniciar a campanha.

   >[!NOTE]
   >
   >Quaisquer alterações nos campos do formulário devem ser feitas dentro das Atividades de marketing do Marketo em Editar rascunho do formulário.

## Três maneiras de adicionar uma imagem de plano de fundo a um formulário {#three-ways-to-add-a-background-image-to-a-form}

Para adicionar uma imagem de plano de fundo ao formulário, é possível:

* Editar o CSS de um Tema de Formulário
* Alterar as cores da caixa de diálogo ou do widget em Definir campanha
* Adicionar código CSS ao script

Para editar o CSS de um Tema de Formulário, consulte [este artigo](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md).

Para alterar a caixa de diálogo ou as cores do widget em Definir campanha:

1. No Editor de Rich Text, selecione um tipo de campanha Caixa de diálogo e um estilo de diálogo, a cor do cabeçalho e a cor do plano de fundo para personalizar as cores de fundo do formulário. Clique em **Salvar**.

   ![](assets/image2015-12-29-18-3a28-3a31.png)

1. Este é um exemplo de como um Estilo de Diálogo de Aparar Moderno é exibido com um cabeçalho roxo claro e uma cor de fundo.

   ![](assets/image2015-12-29-18-3a27-3a31.png)

Para adicionar o código CSS ao script:

1. No Editor de Rich Text, clique no ícone de HTML.

   ![](assets/image2015-12-29-17-3a56-3a13.png)

1. Cole o código incorporado do formulário com o código de estilo de plano de fundo no Editor de fonte do HTML. Clique em **Atualizar**.

   ![](assets/image2015-12-29-18-3a1-3a15.png)

1. Clique em **Visualizar** para ver como ele será renderizado em uma campanha (o formulário não será exibido na visualização do editor). Este é um exemplo de como o código de formulário acima é renderizado em uma campanha com uma imagem de plano de fundo.

   ![](assets/image2015-12-29-18-3a20-3a35.png)

>[!MORELIKETHIS]
>
>* [Editar o CSS de um Tema de Formulário](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md)
>* [Mostrar mensagem de agradecimento sem uma página de aterrissagem de acompanhamento](https://developers.marketo.com/blog/show-thank-you-message-without-a-follow-up-landing-page/)
>* [Forms 2.0](https://developers.marketo.com/documentation/websites/forms-2-0/)

