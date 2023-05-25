---
unique-page-id: 6848782
description: Dinamize sua mensagem de cancelamento de inscrição para idiomas - Documentação do Marketo - Documentação do produto
title: Tornar a mensagem de cancelamento de inscrição dinâmica para idiomas
exl-id: 953a7fd8-b1f2-4f3f-b889-87d1f0471e0d
source-git-commit: 81ee349dbbe48c70b040751cae750c3684b71c78
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 1%

---

# Tornar a mensagem de cancelamento de inscrição dinâmica para idiomas {#make-your-unsubscribe-message-dynamic-for-languages}

A mensagem e o link padrão para cancelar a inscrição estão em inglês. Você pode usar o conteúdo dinâmico para exibi-lo em diferentes idiomas.

>[!NOTE]
>
>Este artigo representa uma prática recomendada, mas pode ser realizado de outras maneiras.

## Preparar seus dados {#prepare-your-data}

1. [Criar um campo personalizado](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) chamado &quot;Idioma preferencial&quot;. (Configure-o no CRM se desejar que esse campo seja sincronizado).

   >[!TIP]
   >
   >No futuro, use este campo quando você [criar um formulário](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) para capturar a preferência de idioma.

## Criar segmentação {#create-segmentation}

1. Vá para a **[!UICONTROL Banco de dados]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-1.png)

1. No **[!UICONTROL Novo]** , clique em **[!UICONTROL Nova segmentação]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-2.png)

1. Nomear a segmentação **[!UICONTROL Idioma Preferencial]**. Clique em **[!UICONTROL Adicionar segmento]**. Digite um idioma.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-3.png)

   >[!NOTE]
   >
   >O segmento padrão será inglês.

1. Continue a adicionar segmentos até que todos os idiomas sejam representados. Clique em **[!UICONTROL Criar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-4.png)

1. Selecione um segmento.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-5.png)

1. Vá para a **[!UICONTROL Lista inteligente]** guia. Enter **[!UICONTROL Idioma Preferencial]** no campo de pesquisa. Arraste e solte o filtro na tela de desenho.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-6.png)

1. Defina o idioma correspondente apropriado.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-7.png)

1. Repita o procedimento para todos os diferentes idiomas. Em seguida, selecione o **[!UICONTROL Ações de segmentação]** e clique em **[!UICONTROL Aprovar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-8.png)

## Criar um trecho {#create-a-snippet}

1. Vá para a **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-9.png)

1. No **[!UICONTROL Novo]** , clique em **[!UICONTROL Novo trecho]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-10.png)

1. Nomeie o trecho **Cancelar inscrição na mensagem**. Clique em **[!UICONTROL Criar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-11.png)

1. Digite a mensagem de cancelamento de inscrição padrão, realce-a e clique no ícone de hiperlink.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-12.png)

1. Copie e cole este token: `{{system.unsubscribeLink}}` no **[!UICONTROL URL]** campo. Clique em **[!UICONTROL Inserir]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-13.png)

1. Selecionar **[!UICONTROL Segmentar por]** no **[!UICONTROL Segmentação]** seção.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-14.png)

1. No **[!UICONTROL Segmentação]** menu suspenso, digite **[!UICONTROL Preferencial]** e selecione **[!UICONTROL Idioma Preferencial]**. Clique em **[!UICONTROL Salvar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-15.png)

1. Selecione um segmento na árvore. Clique no cancelamento de inscrição e no ícone de link.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-16.png)

1. Verifique se `{{system.unsubscribeLink}}` ainda está no **[!UICONTROL URL]** campo. Edite o **[!UICONTROL Texto de exibição]** para corresponder ao idioma selecionado. Clique em **[!UICONTROL Aplicar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-17.png)

1. Repita o procedimento para todos os segmentos. Em seguida, volte para a guia **[!UICONTROL Design Studio]**, clique no link **[!UICONTROL Ações do trecho]** e clique em **[!UICONTROL Aprovar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-18.png)

Ótimo. Quase lá!

## Usar trecho em um email {#use-snippet-in-an-email}

1. No editor de email, clique no elemento editável. Clique no ícone de engrenagem e selecione **[!UICONTROL Substituir pelo trecho]**. Se estiver selecionando um elemento de trecho editável, clique no ícone de engrenagem e selecione **[!UICONTROL Editar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-19.png)

1. Localize e selecione seu trecho na lista suspensa e clique em **[!UICONTROL Salvar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-20.png)

1. Para testar, clique em **[!UICONTROL Voltar]**..

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-21.png)

1. ...depois o **[!UICONTROL Dinâmico]** guia.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-22.png)

1. Clique nos diferentes idiomas para ver a alteração do trecho.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-23.png)

   >[!TIP]
   >
   >É claro que você também pode editar o restante do seu email para linguagem dinâmica. Enquanto estiver nessa página, faça a mesma técnica na página de cancelamento de inscrição.

## Personalização da página de cancelamento de inscrição com conteúdo dinâmico {#customizing-your-unsubscribe-page-with-dynamic-content}

Se você quiser que seus funcionários acessem uma página de cancelamento de inscrição no idioma de sua preferência, é possível usar o conteúdo dinâmico na página de aterrissagem e na página de confirmação.

1. Navegue até a **[!UICONTROL Design Studio]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-24.png)

1. Digitar _Cancelar inscrição_ no campo de pesquisa e selecione a página Cancelar inscrição desejada.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-25.png)

1. Clique em **[!UICONTROL Editar rascunho]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-26.png)

1. Selecionar **[!UICONTROL Segmentar por]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-27.png)

1. Localize o **[!UICONTROL Idioma Preferencial]** segmento. Clique em **[!UICONTROL Salvar]**.

   ![](assets/make-your-unsubscribe-message-dynamic-for-languages-28.png)

   Edite seu conteúdo para cada página de aterrissagem, aprove e você está pronto para prosseguir!

   >[!NOTE]
   >
   >Saiba mais sobre [conteúdo dinâmico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) e todas as coisas legais que você pode fazer.
