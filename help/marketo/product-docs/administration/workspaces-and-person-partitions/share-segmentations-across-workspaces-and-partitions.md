---
unique-page-id: 7515767
description: Compartilhar segmentações entre espaços de trabalho e partições - Documentação do Marketo - Documentação do produto
title: Compartilhar segmentações entre espaços de trabalho e partições
exl-id: b50f4328-fdba-4e39-bc0d-75bade1f9cbc
feature: Partitions, Workspaces
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '474'
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
>Saiba [como criar segmentações](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).

Depois de configurar essas personalidades (_e_ você usa espaços de trabalho), convém compartilhá-las em seus espaços de trabalho. Estas são algumas coisas boas a saber:

## Regras e dicas {#rules-tips}

* Cada assinatura do Marketo pode conter até 20 Segmentações &quot;no total&quot; em vários espaços de trabalho (**não 20 por espaço de trabalho**).
* Você só pode compartilhar uma Segmentação com espaços de trabalho aos quais tem acesso.
* Crie e utilize um **Espaço de trabalho padrão que tenha visibilidade sobre todas as partições**.

* O processamento de segmentação só é executado nas pessoas no espaço de trabalho em que a segmentação é criada.

   * Crie a Segmentação que deseja compartilhar no Workspace padrão.
      * Aprovar a segmentação
      * O espaço de trabalho compartilhado vê uma pasta bloqueada e a Segmentação é somente leitura.
      * Não é possível editar a versão compartilhada. Você só pode editar a Segmentação original onde ela foi criada.

   * Ao clicar em um Segmento (por exemplo, Assistência médica) em uma Segmentação compartilhada, as pessoas que você vê serão somente pessoas na partição associadas ao espaço de trabalho que você está visualizando.
      * Se você criar uma Segmentação no Workspace 1 (WS1) e compartilhá-la com WS2 e WS1 não tiver acesso à partição para WS2, ela NÃO recalculará a Segmentação.
      * Se você criar uma Segmentação em um espaço de trabalho que tenha partições limitadas e, em seguida, compartilhá-la com outro espaço de trabalho, esse espaço de trabalho que recebeu a Segmentação compartilhada só verá pessoas se elas tiverem sobreposição.

>[!NOTE]
>
>Algumas dessas regras são um pouco complexas. A maneira mais fácil de começar é testar com pessoas específicas. Você sempre pode fazer novas segmentações e se livrar das antigas.

## Exemplos de cenários {#example-scenarios}

![](assets/share-segmentations-across-workspaces-and-partitions-1.png)

![](assets/share-segmentations-across-workspaces-and-partitions-2.png)

## Compartilhar uma segmentação {#share-a-segmentation}

1. Vá para o **[!UICONTROL Banco de Dados]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-3.png)

1. Clique com o botão direito do mouse em **[!UICONTROL Segmentações]** e selecione **[!UICONTROL Nova Pasta]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-4.png)

1. Nomeie a pasta que você vai compartilhar entre espaços de trabalho (exemplo: Compartilhar segmentações) e clique em **[!UICONTROL Criar]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-5.png)

1. Mova as Segmentações que deseja compartilhar para a pasta.

   ![](assets/share-segmentations-across-workspaces-and-partitions-6.png)

1. Clique com o botão direito do mouse na pasta e selecione **[!UICONTROL Compartilhar Pasta]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-7.png)

1. Selecione os espaços de trabalho com os quais deseja compartilhar a pasta. Clique em **[!UICONTROL Salvar]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-8.png)

   >[!NOTE]
   >
   >A caixa de diálogo exibe os espaços de trabalho que você tem permissão para exibir, razão pela qual a Marketo recomenda criar e compartilhar Segmentações do espaço de trabalho Padrão que tenha visibilidade de todos os espaços de trabalho e partições.

A pasta de origem é exibida na árvore do Banco de dados com uma seta indicando que ela é compartilhada com outros espaços de trabalho. No espaço de trabalho compartilhado, a pasta é exibida com um bloqueio para indicar que o conteúdo da pasta foi compartilhado de outro espaço de trabalho e é somente leitura.
