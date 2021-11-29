---
unique-page-id: 2359449
description: Definir regras de segmento - Documentos do Marketo - Documentação do produto
title: Definir regras de segmento
exl-id: e6631848-aa8c-4709-b182-4c88abbd365b
source-git-commit: 55afdc537d0a5d0b6114f478c4dd2ded09c84e34
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Definir regras de segmento {#define-segment-rules}

Definir regras de segmento permite categorizar suas pessoas em grupos mutuamente exclusivos diferentes.

>[!PREREQUISITES]
>
>[Criar uma segmentação](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

1. Vá para o **Banco de dados.**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. Selecionar **Segmentação** na árvore, em seguida, clique em um **Segmento**.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. Clique em **Lista inteligente** e adicionar filtros.

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >Os segmentos atualmente não são compatíveis _No passado_ e _Em Cronograma_  em filtros. Isso ocorre porque as segmentações só verificam atualizações quando um valor de dados de alteração é registrado. Esses valores são _not_ registrado para itens que mudam automaticamente, como campos de fórmula e datas. Além disso, os operadores de data com intervalos de data relativos não são compatíveis, pois são calculados no momento da aprovação da segmentação, não no momento de uma atividade Alterar valor de dados .

   >[!NOTE]
   >
   >No momento, os filtros &quot;Tipo SFDC&quot; e &quot;Tipo de Microsoft&quot; não são compatíveis com as listas inteligentes de segmentação.

1. Preencha os valores apropriados para os filtros.

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!CAUTION]
   >
   >O comportamento de registro de atividades para campos de Conta pode afetar a qualificação. Portanto, recomendamos não usar os campos Conta ao definir regras de segmento.

1. Clique no botão **Pessoas (Rascunho)** para exibir as pessoas que podem se qualificar para serem membros deste segmento.

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. Ir para **Ações de segmentação**. Clique em **Aprovar**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >O número total de segmentos que você pode criar em uma segmentação depende do número e do tipo de filtros usados e também da complexidade da lógica de seus segmentos. Embora seja possível criar até 100 segmentos usando campos padrão, o uso de outros tipos de filtros pode aumentar a complexidade e sua segmentação pode não ser aprovada. Alguns exemplos: campos personalizados, membro da lista, campos de proprietários de leads e estágios de receita.
   >
   >Se você receber uma mensagem de erro durante a aprovação e precisar de assistência para reduzir a complexidade da segmentação, entre em contato com o [Suporte Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Confira o painel para obter uma visão geral rápida dos segmentos em um gráfico de pizza, bem como as regras aplicadas.

   ![](assets/image2014-9-15-11-3a36-3a19.png)

Bom trabalho! Esses segmentos serão úteis em muitos lugares do Marketo.

>[!NOTE]
>
>Uma pessoa pode se qualificar para segmentos diferentes, mas eventualmente pertence a apenas um que depende da variável [ordem de prioridade dos segmentos](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md).

>[!NOTE]
>
>A tela Pessoas (Rascunho) mostra todas as pessoas que se qualificaram para ser membro e nem sempre é a lista final de pessoas. Aprove seu segmento para ver a lista final.

>[!MORELIKETHIS]
>
>[Aprovar uma segmentação](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)
