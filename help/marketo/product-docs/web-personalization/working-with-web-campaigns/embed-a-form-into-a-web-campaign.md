---
unique-page-id: 10095554
description: Incorpore um formulário em uma campanha da Web - Documentação do Marketo - Documentação do produto
title: Incorporar um formulário em uma campanha da Web
exl-id: 41e60ae6-9a40-444f-8a55-47fc6ef6c5fb
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 2%

---

# Incorporar um formulário em uma campanha da Web {#embed-a-form-into-a-web-campaign}

Veja como incorporar um formulário do Marketo em uma campanha da Web (Caixa de diálogo, Na zona ou Widget).

1. Clique com o botão direito do mouse em um formulário aprovado. Selecione **[!UICONTROL Código Incorporado]**.

   ![](assets/image2015-12-16-10-3a58-3a39.png)

1. Copie o código.

   ![](assets/image2015-12-16-11-3a16-3a24.png)

1. Em [!DNL Web Personalization], vá para **[!UICONTROL Campanhas da Web]**.

   ![](assets/web-campaigns-hand-7.jpg)

1. Clique em **[!UICONTROL Criar nova campanha]**.

   ![](assets/create-new-web-campaign-hand-1.jpg)

1. No Editor de Rich Text, clique no ícone HTML.

   ![](assets/five-1.png)

1. Cole o código de inserção do formulário no [!UICONTROL HTML Source Editor]. Clique **[!UICONTROL Atualizar]**.

   ![](assets/six-1.png)

1. O formulário não será exibido na visualização do editor, mas você pode visualizá-lo para ver como ele será renderizado em uma campanha.

1. Clique em **[!UICONTROL Iniciar]** para iniciar a campanha.

   >[!NOTE]
   >
   >Quaisquer alterações nos campos do formulário devem ser feitas nas Atividades de marketing do Marketo em Editar rascunho do formulário.

## Três maneiras de adicionar uma imagem de fundo a um formulário {#three-ways-to-add-a-background-image-to-a-form}

Para adicionar uma imagem de plano de fundo ao formulário, você pode:

* Editar o CSS de um tema de formulário
* Alterar as cores da caixa de diálogo ou do widget no Definir campanha
* Adicionar código CSS ao script

Para editar o CSS de um tema de formulário, consulte [este artigo](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md).

Para alterar as cores da caixa de diálogo ou do widget em Definir campanha:

1. No Editor de Rich Text, selecione um tipo de campanha de caixa de diálogo e um estilo de caixa de diálogo, cor do cabeçalho e cor do plano de fundo para personalizar as cores do plano de fundo do formulário. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-12-29-18-3a28-3a31.png)

1. Este é um exemplo de como um Estilo de Caixa de Diálogo de Corte Moderno é exibido com um cabeçalho roxo claro e cor de fundo.

   ![](assets/image2015-12-29-18-3a27-3a31.png)

Para adicionar o código CSS ao script:

1. No Editor de Rich Text, clique no ícone HTML.

   ![](assets/image2015-12-29-17-3a56-3a13.png)

1. Cole o código de inserção do formulário com o código de estilo de plano de fundo no [!UICONTROL HTML Source Editor]. Clique **[!UICONTROL Atualizar]**.

   ![](assets/image2015-12-29-18-3a1-3a15.png)

1. Clique em **[!UICONTROL Visualizar]** para ver como ele será renderizado em uma campanha (o formulário não será exibido no modo de exibição do editor). Este é um exemplo de como o código de formulário acima é renderizado em uma campanha com uma imagem de fundo.

   ![](assets/image2015-12-29-18-3a20-3a35.png)

>[!MORELIKETHIS]
>
>* [Editar o CSS de um Tema de Formulário](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md)
>* [Mostrar mensagem de agradecimento sem uma página de aterrissagem de acompanhamento](https://developers.marketo.com/blog/show-thank-you-message-without-a-follow-up-landing-page/)
>* [Forms 2.0](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/javascriptapi/forms-api-reference)
