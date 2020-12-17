---
unique-page-id: 7515767
description: Compartilhar segmentações entre espaços de trabalho e partições - Documentos de marketing - Documentação do produto
title: Compartilhar segmentações entre espaços de trabalho e partições
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---


# Compartilhar segmentações entre espaços de trabalho e partições {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>Este artigo destina-se apenas aos clientes que possuem espaços de trabalho e partições

## O que é uma segmentação? {#whats-a-segmentation}

Marketo é ótimo em escolher as pessoas certas para um programa ou campanha inteligente. No entanto, para personas mais permanentes, você deve usar segmentações. Eles são necessários para usar conteúdo dinâmico avançado no Marketo.

>[!NOTE]
>
>**Mergulho profundo**
>
>Saiba mais sobre [como criar segmentações](../../../product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).

Depois de configurar essas personas (**e** você usa espaços de trabalho), você desejará compartilhá-las em seus espaços de trabalho. Aqui estão algumas coisas boas para se saber:

## Regras e dicas {#rules-tips}

* Cada subscrição de marketing pode conter até 20 Segmentações &quot;total&quot; em vários espaços de trabalho (**e não 20 por espaço de trabalho**).
* Você só pode compartilhar uma Segmentação com espaços de trabalho aos quais você tem acesso.
* Certifique-se de criar e utilizar um **espaço de trabalho padrão que tenha visibilidade em todas as partições**.

* O processamento de segmentação só é executado nas pessoas no espaço de trabalho onde a Segmentação é criada.

   * Crie a Segmentação que deseja compartilhar dentro da Área de trabalho padrão.

      * Aprovar a segmentação
      * O espaço de trabalho compartilhado vê uma pasta bloqueada e a Segmentação é somente leitura.
      * Não é possível editar a versão compartilhada. Você só pode editar a Segmentação original onde ela foi criada.
   * Ao clicar em um Segmento (por exemplo, Saúde) em uma Segmentação compartilhada, as pessoas que você vê serão apenas pessoas na partição associada ao espaço de trabalho que você está visualizando.

      * Se você criar uma Segmentação no Workspace 1 (WS1) e compartilhá-la com WS2 e WS1 não tiver acesso à partição para WS2, ela NÃO recalculará a Segmentação.
      * Se você criar uma Segmentação em um espaço de trabalho que tenha partições limitadas e, em seguida, compartilhá-la com outro espaço de trabalho, esse espaço de trabalho que recebeu a Segmentação compartilhada só verá pessoas se elas tiverem sobreposição.


>[!NOTE]
>
>Algumas dessas regras são um pouco complexas. A maneira mais fácil de começar é testar com pessoas específicas. Você sempre pode fazer novas segmentações e se livrar das segmentações antigas.

## Cenários de exemplo {#example-scenarios}

![](assets/image2015-5-27-16-3a26-3a25.png)

** ![](assets/image2015-5-27-16-3a26-3a48.png)

**

## Compartilhar uma segmentação {#share-a-segmentation}

1. Vá para o Banco de Dados.

   ![](assets/image2017-3-29-8-3a15-3a40.png)

1. Clique com o botão direito do mouse em Segmentações e selecione Novas pastas.

   ![](assets/image2017-3-29-8-3a40-3a31.png)

1. Nomeie a pasta que você vai compartilhar entre as áreas de trabalho (por exemplo: Compartilhar segmentações.)

   ![](assets/image2017-3-29-8-3a40-3a45.png)

1. Mova as segmentações que deseja compartilhar para a pasta.

   ![](assets/image2017-3-29-8-3a41-3a3.png)

1. Clique com o botão direito do mouse na pasta e selecione Compartilhar pasta.

   ![](assets/image2017-3-29-8-3a41-3a19.png)

1. Selecione os espaços de trabalho com os quais deseja compartilhar a pasta. Clique em Salvar.

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >A caixa de diálogo exibe os espaços de trabalho aos quais você tem permissão para visualização, e é por isso que Marketo recomenda criar e compartilhar Segmentações a partir do espaço de trabalho Padrão que tem visibilidade em todos os espaços de trabalho e partições.

A pasta de origem é exibida na árvore Banco de Dados com uma seta indicando que ela é compartilhada com outros espaços de trabalho. No espaço de trabalho compartilhado, a pasta é exibida com um bloqueio para indicar que o conteúdo da pasta foi compartilhado de outro espaço de trabalho e é somente leitura.

>[!NOTE]
>
>**Artigos relacionados**
>
>[Segmentação e trechos](http://docs.marketo.com/display/docs/segmentation+and+snippets)

