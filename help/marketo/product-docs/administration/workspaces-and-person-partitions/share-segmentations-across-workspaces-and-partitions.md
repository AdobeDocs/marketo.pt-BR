---
unique-page-id: 7515767
description: Compartilhar segmentações em espaços de trabalho e partições - Documentos do Marketo - Documentação do produto
title: Compartilhar segmentações em espaços de trabalho e partições
exl-id: b50f4328-fdba-4e39-bc0d-75bade1f9cbc
source-git-commit: 686530e63cffef89bc7b9cbf6affa862689c0a46
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Compartilhar segmentações em espaços de trabalho e partições {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>Este artigo é somente para clientes que possuem espaços de trabalho e partições.

## O que é uma segmentação? {#whats-a-segmentation}

O Marketo é excelente em escolher as pessoas certas para um programa ou campanha inteligente. No entanto, para personas mais permanentes, você deve usar segmentações. Eles são necessários para usar conteúdo dinâmico avançado no Marketo.

>[!NOTE]
>
>Saiba mais [como criar segmentações](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).

Depois de configurar essas personas (_e_ ao usar espaços de trabalho), você deseja compartilhá-los em seus espaços de trabalho. Estas são algumas coisas boas para se saber:

## Regras e dicas {#rules-tips}

* Cada assinatura do Marketo pode conter até 20 Segmentações &quot;total&quot; em vários espaços de trabalho (**não 20 por espaço de trabalho**).
* Você só pode compartilhar uma Segmentação com espaços de trabalho aos quais tem acesso.
* Certifique-se de criar e utilizar um **Espaço de trabalho padrão que tem visibilidade em todas as partições**.

* O processamento de segmentação é executado somente nas pessoas no espaço de trabalho em que a Segmentação é criada.

   * Crie a Segmentação que deseja compartilhar dentro do Espaço de trabalho padrão.
      * Aprovar a segmentação
      * O espaço de trabalho compartilhado vê uma pasta bloqueada e a Segmentação é somente leitura.
      * Não é possível editar a versão compartilhada. Você só pode editar a Segmentação original onde ela foi criada.
   * Ao clicar em um Segmento (por exemplo, Saúde) em uma Segmentação compartilhada, as pessoas que você vê serão apenas pessoas na partição associada ao espaço de trabalho que você está visualizando.
      * Se você criar uma Segmentação no Workspace 1 (WS1) e compartilhá-la com WS2 e WS1 não tiver acesso à partição para WS2, ela NÃO recalculará a Segmentação.
      * Se você criar uma Segmentação em um espaço de trabalho que tem partições limitadas e, em seguida, compartilhá-la com outro espaço de trabalho, esse espaço de trabalho que recebeu a Segmentação compartilhada verá pessoas somente se elas tiverem sobreposição.


>[!NOTE]
>
>Algumas dessas regras são um pouco complexas. A maneira mais fácil de começar é testar com pessoas específicas. Você sempre pode fazer novas segmentações e se livrar das antigas.

## Cenários de exemplo {#example-scenarios}

![](assets/share-segmentations-across-workspaces-and-partitions-1.png)

![](assets/share-segmentations-across-workspaces-and-partitions-2.png)

## Compartilhar uma segmentação {#share-a-segmentation}

1. Vá para o **Banco de dados**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-3.png)

1. Clique com o botão direito do mouse **Segmentações** e selecione **Nova pasta**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-4.png)

1. Nomeie a pasta que você compartilhará nos espaços de trabalho (por exemplo: Compartilhar segmentações) e clique em **Criar**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-5.png)

1. Mova a(s) Segmentação(ões) que deseja compartilhar na pasta.

   ![](assets/share-segmentations-across-workspaces-and-partitions-6.png)

1. Clique com o botão direito do mouse na pasta e selecione **Compartilhar pasta**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-7.png)

1. Selecione os espaços de trabalho com os quais deseja compartilhar a pasta. Clique em **Salvar**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-8.png)

   >[!NOTE]
   >
   >A caixa de diálogo exibe os espaços de trabalho que você tem permissão para visualizar, por isso a Marketo recomenda criar e compartilhar Segmentações do espaço de trabalho Padrão que tem visibilidade em todos os espaços de trabalho e partições.

A pasta de origem é exibida na árvore Banco de dados com uma seta indicando que ela é compartilhada com outros espaços de trabalho. No espaço de trabalho compartilhado, a pasta é exibida com um bloqueio para indicar que o conteúdo da pasta foi compartilhado de outro espaço de trabalho e é somente leitura.
