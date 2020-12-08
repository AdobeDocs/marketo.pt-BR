---
unique-page-id: 6848782
description: Torne a sua mensagem de cancelamento de assinatura dinâmica para idiomas - documentos de marketing - documentação do produto
title: Tornar sua mensagem de cancelamento de assinatura dinâmica para idiomas
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---


# Tornar sua mensagem de cancelamento de assinatura dinâmica para idiomas {#make-your-unsubscribe-message-dynamic-for-languages}

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

A mensagem e o link padrão de cancelamento de inscrição estão em inglês. Você pode usar o conteúdo dinâmico para exibi-lo em idiomas diferentes.

>[!NOTE]
>
>Configuramos este belo tutorial abaixo para você. Representa uma prática recomendada, mas isso pode ser feito de outras formas.

1. Preparar seus dados
1. [Crie um](../../../../product-docs/administration/field-management/create-a-custom-field-in-marketo.md)campo personalizado chamado &quot;Idioma preferencial&quot;. (Configure-o no CRM se desejar que esse campo seja sincronizado).

   >[!TIP]
   >
   >No futuro, use esse campo ao [criar um formulário](../../../../product-docs/demand-generation/forms/creating-a-form/create-a-form.md) para capturar a preferência de idioma.

1. Criar segmentação
1. Vá para o **Banco de Dados**.
** ![](assets/db.png)

   **

1. Na lista suspensa **Novo** , clique em **Nova segmentação**.

   ![](assets/two.png)

1. Nomeie o Idioma **** preferencial da segmentação. Clique em **Adicionar segmento**. Digite um idioma.

   ![](assets/image2015-3-9-8-3a33-3a44.png)

   >[!NOTE]
   >
   >O segmento padrão será inglês.

1. Continue a adicionar segmentos até que todos os idiomas sejam representados. Clique em **Criar**.

   ![](assets/image2015-3-9-8-3a38-3a5.png)

1. Selecione um segmento.

   ![](assets/image2015-3-9-8-3a38-3a17.png)

1. Vá para a guia **Lista** inteligente. Insira o Idioma **preferencial** no campo de pesquisa. Arraste e solte o filtro na tela.

   ![](assets/six.png)

1. Defina o idioma correspondente apropriado.

   ![](assets/seven.png)

1. Repita o procedimento para todos os idiomas diferentes. Em seguida, selecione o menu suspenso Ações **de** segmentação e clique em **Aprovar**.

   ![](assets/image2015-3-9-8-3a39-3a36.png)

1. Criar um trecho
1. Vá para o **Design Studio**.

   ![](assets/ds.png)

1. Na lista suspensa **Novo** , clique em **Novo trecho**.

   ** ![](assets/ten.png)

   **

1. Nomeie o snippet **Unsubscribe Message (Cancelar inscrição)**. Clique em **Criar**.

   ![](assets/image2015-3-9-8-3a40-3a54.png)

1. Digite sua mensagem padrão de cancelamento de assinatura, realce-a e clique no ícone de hiperlink.

   ![](assets/image2015-3-9-8-3a41-3a47.png)

1. Copie e cole este token: **`{{system.unsubscribeLink}}`** no campo URL **do** link. Clique em **Inserir**.

   ![](assets/image2015-3-9-8-3a43-3a17.png)

1. Selecione **Segmentar por** na seção Segmentação.

   ![](assets/image2015-3-9-8-3a44-3a16.png)

1. No menu suspenso Segmentação, digite **Preferencial** e selecione Idioma **preferencial**. Clique em **Salvar**.

   ![](assets/image2015-3-9-8-3a44-3a32.png)

1. Selecione um segmento na árvore. Digite sua mensagem de cancelamento de assinatura nesse idioma.

   ![](assets/image2015-3-9-8-3a45-3a43.png)

1. Copie e cole o mesmo token: **`{{system.unsubscribeLink}}`** no campo URL **do** link. Clique em **Inserir**.

   ![](assets/image2015-3-9-8-3a47-3a4.png)

1. Repita o procedimento para todos os seus segmentos. Em seguida, volte para o Design Studio, clique no menu suspenso **Snippet Actions (Ações** de trecho) e clique em **Aprovar**.

   ![](assets/image2015-3-9-8-3a47-3a34.png)

   Incrível. Quase lá.

1. Usar fragmento em um email
1. No editor de email, clique no elemento editável. Em seguida, clique no ícone de engrenagem e selecione **Substituir por trecho**. Se você estiver selecionando um elemento de trecho editável, clique no ícone de engrenagem e selecione **Editar**.

   ![](assets/4.1.png)

1. Localize e selecione seu trecho na lista suspensa e clique em **Salvar**.

   ![](assets/image2015-3-9-8-3a50-3a16.png)

1. Para testá-la, clique em **Voltar**...

   ![](assets/4.3.png)

1. ...em seguida, a guia **Dinâmico** .

   ![](assets/4.4.png)

1. Clique nos diferentes idiomas para ver a alteração do snippet.

   ![](assets/4.5.png)

   >[!TIP]
   >
   >É claro, você também pode editar o restante do seu email para um idioma dinâmico. Enquanto estiver nela, faça a mesma técnica na página de cancelamento de inscrição.

1. Personalizar sua página de cancelamento de assinatura com conteúdo dinâmico

   Se você quiser que seu pessoal acesse uma página de cancelamento de inscrição em seu idioma preferido, você poderá usar o conteúdo dinâmico na landing page e na página de confirmação.

   Navegue até o Design Studio.

   ![](assets/ds.png)

   Digite Cancelar inscrição no campo de pesquisa. Você deve encontrar suas páginas Cancelar inscrição.

   ![](assets/image2015-3-9-8-3a51-3a53.png)

   Clique em Editar rascunho.

   ![](assets/image2015-3-9-8-3a52-3a23.png)

   Selecione Segmentar por.

   ![](assets/image2015-3-9-8-3a52-3a57.png)

   Encontre o segmento Idioma preferencial. Clique em Salvar.

   ![](assets/image2015-3-9-8-3a53-3a54.png)

   Edite seu conteúdo para cada landing page, aprove e você pode ir!

   >[!NOTE]
   >
   >**Mergulho profundo**
   >
   >
   >Saiba mais sobre o conteúdo [](../../../../product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) dinâmico e todas as coisas legais que você pode fazer.

