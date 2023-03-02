---
unique-page-id: 7515767
description: Compartilhar segmentações entre espaços de trabalho e partições - Documentação do Marketo - Documentação do produto
title: Compartilhar segmentações entre espaços de trabalho e partições
exl-id: b50f4328-fdba-4e39-bc0d-75bade1f9cbc
source-git-commit: 4d4d87d2a03bc0966a6e77d97cb68a2c38a3c676
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Compartilhar segmentações entre espaços de trabalho e partições {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>Este artigo destina-se apenas a clientes que têm Espaços de trabalho e Partições.

## O que é uma segmentação? {#whats-a-segmentation}

O Marketo é excelente para escolher as pessoas certas para um programa ou campanha inteligente. No entanto, para perfis mais permanentes, você deve usar segmentações. Eles são necessários para usar conteúdo dinâmico avançado no Marketo.

>[!NOTE]
>
>Saiba mais [como criar segmentação](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).

Depois de configurar esses perfis (_e_ use espaços de trabalho), você desejará compartilhá-los em seus espaços de trabalho. Estas são algumas coisas boas a saber:

## Regras e dicas {#rules-tips}

* Cada assinatura do Marketo pode conter até 20 segmentações &quot;no total&quot; em vários espaços de trabalho (**não 20 por espaço de trabalho**).
* Você só pode compartilhar uma Segmentação com espaços de trabalho aos quais tem acesso.
* Crie e utilize um **Espaço de trabalho padrão que tem visibilidade em todas as partições**.

* O processamento de segmentação só é executado nas pessoas no espaço de trabalho em que a segmentação é criada.

   * Crie a Segmentação que deseja compartilhar no Espaço de trabalho padrão.
      * Aprovar a segmentação
      * O espaço de trabalho compartilhado vê uma pasta bloqueada e a Segmentação é somente leitura.
      * Não é possível editar a versão compartilhada. Você só pode editar a Segmentação original onde ela foi criada.
   * Ao clicar em um Segmento (por exemplo, Assistência médica) em uma Segmentação compartilhada, as pessoas que você vê serão somente pessoas na partição associadas ao espaço de trabalho que você está visualizando.
      * Se você criar uma Segmentação no Espaço de trabalho 1 (WS1) e compartilhá-la com WS2 e WS1 não tiver acesso à partição para WS2, ela NÃO recalculará a Segmentação.
      * Se você criar uma Segmentação em um espaço de trabalho que tenha partições limitadas e, em seguida, compartilhá-la com outro espaço de trabalho, esse espaço de trabalho que recebeu a Segmentação compartilhada só verá pessoas se elas tiverem sobreposição.


>[!NOTE]
>
>Algumas dessas regras são um pouco complexas. A maneira mais fácil de começar é testar com pessoas específicas. Você sempre pode fazer novas segmentações e se livrar das antigas.

## Exemplos de cenários {#example-scenarios}

![](assets/image2015-5-27-16-3a26-3a25.png)

![](assets/image2015-5-27-16-3a26-3a48.png)

## Compartilhar uma segmentação {#share-a-segmentation}

1. Vá para a **Banco de dados**.

   ![](assets/image2017-3-29-8-3a15-3a40.png)

1. Clique com o botão direito do mouse **Segmentações** e selecione **Novas pastas**.

   ![](assets/image2017-3-29-8-3a40-3a31.png)

1. Nomeie a pasta que você compartilhará entre espaços de trabalho (exemplo: Compartilhar segmentações).

   ![](assets/image2017-3-29-8-3a40-3a45.png)

1. Mova as Segmentações que deseja compartilhar para a pasta.

   ![](assets/image2017-3-29-8-3a41-3a3.png)

1. Clique com o botão direito do mouse e selecione **Compartilhar pasta**.

   ![](assets/image2017-3-29-8-3a41-3a19.png)

1. Selecione os espaços de trabalho com os quais deseja compartilhar a pasta. Clique em **Salvar**.

   ![](assets/share-segmentations-across-workspaces-and-partitions.png)

   >[!NOTE]
   >
   >A caixa de diálogo exibe os espaços de trabalho que você tem permissão para exibir, razão pela qual a Marketo recomenda criar e compartilhar Segmentações do espaço de trabalho Padrão que tenha visibilidade de todos os espaços de trabalho e partições.

A pasta de origem é exibida na árvore do Banco de dados com uma seta indicando que ela é compartilhada com outros espaços de trabalho. No espaço de trabalho compartilhado, a pasta é exibida com um bloqueio para indicar que o conteúdo da pasta foi compartilhado de outro espaço de trabalho e é somente leitura.
