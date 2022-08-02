---
unique-page-id: 11385020
description: Ativar conteúdo preditivo em emails - Documentos do Marketo - Documentação do produto
title: Ativar conteúdo preditivo em emails
exl-id: 7eaefee1-23e8-47ee-afff-adcf49096aa7
source-git-commit: 4b1b91a933a7a6d103fe0d44ece9ea95759edc5f
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Ativar conteúdo preditivo em emails {#enable-predictive-content-in-emails}

Faça uma ou mais imagens preditivas no seu email, adaptando a experiência para cada recipient.

>[!NOTE]
>
>Recomenda-se ativar mais de cinco partes de conteúdo por categoria e por fonte (email, mídia avançada, barra) antes de testar e usar Conteúdo preditivo. Mais conteúdo oferece um resultado preditivo melhor.

>[!PREREQUISITES]
>
>Antes de ativar o Conteúdo preditivo, você deve:
>
>* **Preparar seu conteúdo preditivo**
   >
   >   * [Editar conteúdo preditivo para emails](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target=&quot;_blank&quot;} ou
   >   * [Editar conteúdo preditivo para mídias avançadas](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target=&quot;_blank&quot;} ou
   >   * [Editar conteúdo preditivo para a barra de recomendação](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target=&quot;_blank&quot;}
>
>* [Aprovar um título para conteúdo preditivo](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target=&quot;_blank&quot;}


## Adicionar conteúdo preditivo usando o editor de email 2.0 {#adding-predictive-content-using-the-email-editor}

1. Clique em **Atividades de marketing**.

   ![](assets/one.png)

1. Selecione seu email e clique em **Editar rascunho**.

   ![](assets/two.png)

1. Clique na imagem que deseja tornar preditiva. Quando o ícone de engrenagem for exibido, clique nele e selecione **Habilitar ContentAI** (ContentAI é o nome anterior para Conteúdo preditivo).

   ![](assets/three.png)

1. Para selecionar uma ou mais categorias, clique no botão **Categorias** , faça suas seleções e clique em **Aplicar**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Escolher categorias específicas ou alterar o layout preditivo é opcional.

1. Sua imagem agora é preditiva. Repita as etapas 3 e 4 para imagens adicionais (se desejar).

   ![](assets/five.png)

1. Para visualizar seu email, clique em **Visualizar** no canto superior direito.

   ![](assets/six.png)

1. Para exibir imagens diferentes possíveis, clique em **Atualizar**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >A imagem não está selecionada **_até que o recipient abra o email_**. Portanto, o que você vê na visualização é apenas um exemplo, e não será necessariamente a imagem que o recipient vê.

1. Quando terminar de visualizar seu email, clique no link **Visualizar ações** e selecione **Aprovar e fechar**. Ou, se você ainda tiver edição para fazer, clique em **Editar rascunho** à direita.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Ao enviar uma amostra, uma imagem aleatória será selecionada.

Após aprovar seu email, ele será equipado com Conteúdo preditivo e pronto para ser enviado!

>[!CAUTION]
>
>Depois que um recipient abre o email, as imagens preditivas são bloqueadas. Se o conteúdo for removido posteriormente, os recipients verão uma imagem quebrada onde o conteúdo estava.

## Adicionar conteúdo preditivo ao não usar o editor de email 2.0 {#adding-predictive-content-when-not-using-the-email-editor}

Se você não estiver usando um [Email 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)Modelo {target=&quot;_blank&quot;}, a adição de conteúdo preditivo ao email pode ser feita simplesmente marcando uma imagem no modelo como um elemento de imagem editável do Marketo.

Saiba mais sobre o [Sintaxe específica do Marketo aqui](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements){target=&quot;_blank&quot;}.

Este é um exemplo de como o código deve ser (este é apenas um exemplo, não copie exatamente o código abaixo).

**Exemplo**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
