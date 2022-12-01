---
unique-page-id: 6848782
description: Torne sua mensagem de cancelamento de assinatura dinâmica para idiomas - documentos do Marketo - documentação do produto
title: Tornar sua mensagem de cancelamento de assinatura dinâmica para idiomas
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
source-git-commit: aeaf1f55b81da70ac8415cab265165a3848b5a0e
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Tornar sua mensagem de cancelamento de assinatura dinâmica para idiomas {#make-your-unsubscribe-message-dynamic-for-languages}

A mensagem de cancelamento de subscrição e o link padrão estão em inglês. Você pode usar o conteúdo dinâmico para exibi-lo em idiomas diferentes.

>[!NOTE]
>
>Este artigo representa uma prática recomendada, mas pode ser realizada de outras maneiras.

## Prepare seus dados {#prepare-your-data}

1. [Criar um campo personalizado](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) chamado de &quot;Idioma preferencial&quot;. (Configure-o no seu CRM se quiser que esse campo seja sincronizado).

   >[!TIP]
   >
   >No futuro, use esse campo quando [criar um formulário](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) para capturar a preferência de idioma.

## Criar segmentação {#create-segmentation}

1. Vá para o **Banco de dados**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-1.png)

1. No **Novo** , clique em **Nova segmentação**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-2.png)

1. Nomeie a segmentação **Idioma preferencial**. Clique em **Adicionar segmento**. Digite um idioma.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-3.png)

   >[!NOTE]
   >
   >O segmento padrão será inglês.

1. Continue a adicionar segmentos até que todos os seus idiomas sejam representados. Clique em **Criar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-4.png)

1. Selecione um segmento.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-5.png)

1. Vá para o **Lista inteligente** guia . Enter **Idioma preferencial** no campo de pesquisa. Arraste e solte o filtro na tela.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-6.png)

1. Defina o idioma correspondente apropriado.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-7.png)

1. Repita o procedimento para todos os idiomas diferentes. Em seguida, selecione a **Ações de segmentação** e clique em **Aprovar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-8.png)

## Criar um trecho {#create-a-snippet}

1. Vá para o **Design Studio**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-9.png)

1. No **Novo** lista suspensa, clique em **Novo trecho**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-10.png)

1. Dê um nome ao trecho **Cancelar assinatura da mensagem**. Clique em **Criar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-11.png)

1. Digite sua mensagem de cancelamento de subscrição padrão, destaque-a e clique no ícone de hiperlink.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-12.png)

1. Copie e cole este token: `{{system.unsubscribeLink}}` na **URL** campo. Clique em **Inserir**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-13.png)

1. Selecionar **Segmentar por** na seção Segmentação .

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-14.png)

1. No menu suspenso Segmentação , digite **Preferencial** e selecione **Idioma preferencial**. Clique em **Salvar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-15.png)

1. Selecione um segmento na árvore. Clique no ícone de cancelamento de subscrição e depois no ícone de link.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-16.png)

1. Certifique-se de `{{system.unsubscribeLink}}` ainda está no campo URL . Edite a opção Exibir texto para corresponder ao idioma selecionado. Clique em **Aplicar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-17.png)

1. Repita o procedimento para todos os seus segmentos. Em seguida, volte para o Design Studio, clique no botão **Ações de trecho** e clique em **Aprovar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-18.png)

Ótimo. Quase lá!

## Usar trecho em um email {#use-snippet-in-an-email}

1. No editor de email, clique no elemento editável. Em seguida, clique no ícone de engrenagem e selecione **Substituir por trecho**. Se estiver selecionando um elemento de trecho editável, clique no ícone de engrenagem e selecione **Editar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-19.png)

1. Encontre e selecione o trecho no menu suspenso e clique em **Salvar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-20.png)

1. Para testar, clique em **Voltar**...

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-21.png)

1. ...em seguida, **Dinâmico** guia .

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-22.png)

1. Clique nos diferentes idiomas para ver o trecho alterado.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-23.png)

   >[!TIP]
   >
   >É claro que também é possível editar o restante do email no idioma dinâmico. Enquanto estiver trabalhando nisso, faça a mesma técnica na página de cancelamento de inscrição.

## Personalização da sua página de cancelamento de assinatura com conteúdo dinâmico {#customizing-your-unsubscribe-page-with-dynamic-content}

Se você quiser que suas pessoas cheguem a uma página de cancelamento de assinatura no idioma preferencial, você poderá usar o conteúdo dinâmico na página de aterrissagem e na página de confirmação.

1. Navegue até o **Design Studio**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-24.png)

1. Digite _Cancelar inscrição_ no campo de pesquisa e selecione a página Cancelar inscrição desejada.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-25.png)

1. Clique em **Editar rascunho**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-26.png)

1. Selecionar **Segmentar por**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-27.png)

1. Encontre o segmento Idioma preferencial . Clique em **Salvar**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-28.png)

   Edite o conteúdo de cada landing page, aprove e pronto!

   >[!NOTE]
   >
   >Saiba mais sobre [conteúdo dinâmico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) e todas as coisas legais que você pode fazer.
