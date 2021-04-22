---
unique-page-id: 6848782
description: Torne sua mensagem de cancelamento de assinatura dinâmica para idiomas - documentos do Marketo - documentação do produto
title: Tornar sua mensagem de cancelamento de assinatura dinâmica para idiomas
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Tornar sua mensagem de cancelamento de assinatura dinâmica para idiomas {#make-your-unsubscribe-message-dynamic-for-languages}

A mensagem de cancelamento de subscrição e o link padrão estão em inglês. Você pode usar o conteúdo dinâmico para exibi-lo em idiomas diferentes.

>[!NOTE]
>
>Configuramos este belo tutorial abaixo para você. Representa uma prática recomendada, mas isso pode ser feito de outras maneiras.

## Prepare seus dados {#prepare-your-data}

1. [Crie um ](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) campo personalizado chamado &quot;Idioma preferencial&quot;. (Configure-o no seu CRM se quiser que esse campo seja sincronizado).

   >[!TIP]
   >
   >No futuro, use esse campo quando [criar um formulário](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) para capturar a preferência de idioma.

## Criar segmentação {#create-segmentation}

1. Vá para o **Banco de Dados**.

   ![](assets/db.png)

1. Na lista suspensa **New**, clique em **New Segmentation**.

   ![](assets/two.png)

1. Nomeie a segmentação **Idioma preferencial**. Clique em **Adicionar segmento**. Digite um idioma.

   ![](assets/image2015-3-9-8-3a33-3a44.png)

   >[!NOTE]
   >
   >O segmento padrão será inglês.

1. Continue a adicionar segmentos até que todos os seus idiomas sejam representados. Clique em **Criar**.

   ![](assets/image2015-3-9-8-3a38-3a5.png)

1. Selecione um segmento.

   ![](assets/image2015-3-9-8-3a38-3a17.png)

1. Vá para a guia **Smart List**. Insira **Idioma preferencial** no campo de pesquisa. Arraste e solte o filtro na tela.

   ![](assets/six.png)

1. Defina o idioma correspondente apropriado.

   ![](assets/seven.png)

1. Repita o procedimento para todos os idiomas diferentes. Em seguida, selecione o menu suspenso **Segmentation Actions** e clique em **Approve**.

   ![](assets/image2015-3-9-8-3a39-3a36.png)

## Criar um trecho {#create-a-snippet}

1. Vá para o **Design Studio**.

   ![](assets/ds.png)

1. Na lista suspensa **New**, clique em **New Snippet**.

   ![](assets/ten.png)

1. Nomeie o trecho **Unsubscribe Message**. Clique em **Criar**.

   ![](assets/image2015-3-9-8-3a40-3a54.png)

1. Digite sua mensagem de cancelamento de subscrição padrão, destaque-a e clique no ícone de hiperlink.

   ![](assets/image2015-3-9-8-3a41-3a47.png)

1. Copie e cole este token: `{{system.unsubscribeLink}}` no campo **Link URL**. Clique em **Inserir**.

   ![](assets/image2015-3-9-8-3a43-3a17.png)

1. Selecione **Segmentar por** na seção Segmentação .

   ![](assets/image2015-3-9-8-3a44-3a16.png)

1. No menu suspenso Segmentação , digite **Preferencial** e selecione **Idioma preferencial**. Clique em **Salvar**.

   ![](assets/image2015-3-9-8-3a44-3a32.png)

1. Selecione um segmento na árvore. Digite sua mensagem de cancelamento de assinatura nesse idioma.

   ![](assets/image2015-3-9-8-3a45-3a43.png)

1. Copie e cole o mesmo token: `{{system.unsubscribeLink}}` no campo **Link URL**. Clique em **Inserir**.

   ![](assets/image2015-3-9-8-3a47-3a4.png)

1. Repita o procedimento para todos os seus segmentos. Em seguida, volte para o Design Studio, clique no menu suspenso **Snippet Actions** e clique em **Approve**.

   ![](assets/image2015-3-9-8-3a47-3a34.png)

   Ótimo. Quase lá.

## Usar trecho em um email {#use-snippet-in-an-email}

1. No editor de email, clique no elemento editável. Em seguida, clique no ícone de engrenagem e selecione **Substituir por trecho**. Se estiver selecionando um elemento de trecho editável, clique no ícone de engrenagem e selecione **Editar**.

   ![](assets/4.1.png)

1. Localize e selecione o trecho no menu suspenso e clique em **Salvar**.

   ![](assets/image2015-3-9-8-3a50-3a16.png)

1. Para testá-lo, clique em **Back**...

   ![](assets/4.3.png)

1. ...em seguida, na guia **Dynamic**.

   ![](assets/4.4.png)

1. Clique nos diferentes idiomas para ver o trecho alterado.

   ![](assets/4.5.png)

   >[!TIP]
   >
   >É claro que também é possível editar o restante do email no idioma dinâmico. Enquanto estiver trabalhando nisso, faça a mesma técnica na página de cancelamento de inscrição.

## Personalizar sua página de cancelamento de assinatura com conteúdo dinâmico {#customizing-your-unsubscribe-page-with-dynamic-content}

Se você quiser que suas pessoas cheguem a uma página de cancelamento de assinatura no idioma preferencial, você poderá usar o conteúdo dinâmico na página de aterrissagem e na página de confirmação.

1. Navegue até o Design Studio.

   ![](assets/ds.png)

1. Digite _Unsubscribe_ no campo de pesquisa. Você deve encontrar suas páginas de Cancelamento de inscrição.

   ![](assets/image2015-3-9-8-3a51-3a53.png)

1. Clique em **Editar rascunho**.

   ![](assets/image2015-3-9-8-3a52-3a23.png)

1. Selecione **Segmentar por**.

   ![](assets/image2015-3-9-8-3a52-3a57.png)

1. Encontre o segmento Idioma preferencial . Clique em **Salvar**.

   ![](assets/image2015-3-9-8-3a53-3a54.png)

   Edite o conteúdo de cada landing page, aprove e pronto!

   >[!NOTE]
   >
   >Saiba mais sobre [conteúdo dinâmico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) e tudo o que você pode fazer de interessante.
