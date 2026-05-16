---
unique-page-id: 2359457
description: Saiba como aprovar uma segmentação para que ela possa ser usada para conteúdo dinâmico e relatórios. Use as ações de banco de dados e segmentação para aprovar após definir as regras de segmento.
title: Aprovar uma segmentação
exl-id: c8b0fbe9-012c-47bf-8769-0167156b43d3
feature: Segmentation
TQID: https://experienceleague.adobe.com/hvFKybwLh1INYx2YWtOmdebJVYXOzhNMMncqeOoV8EU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 255
ht-degree: 5%

---

# Aprovar uma segmentação {#approve-a-segmentation}

Uma segmentação precisa ser aprovada antes de ser usada.

>[!PREREQUISITES]
>
>* [Criar uma segmentação](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>* [Definir Regras de Segmento](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>Um máximo de 20 segmentações podem ser aprovadas de cada vez.

1. Vá para o **[!UICONTROL Banco de Dados]**.

   ![](assets/approve-a-segmentation-1.png)

1. Na segmentação, clique em **[!UICONTROL Ações de segmentação]** e depois em **[!UICONTROL Aprovar]**.

   ![](assets/approve-a-segmentation-2.png)

   >[!NOTE]
   >
   >O status muda para _Aprovando_ enquanto a aprovação está em andamento.

   >[!CAUTION]
   >
   >A aprovação pode levar de alguns minutos a um ou dois dias para ser concluída, dependendo do tamanho do banco de dados.

1. Depois de aprovado, o [!UICONTROL Status] muda de [!UICONTROL Aprovando] para [!UICONTROL Aprovado].

   ![](assets/approve-a-segmentation-3.png)

   >[!TIP]
   >
   >O número de pessoas em cada segmento é mostrado entre parênteses ao lado do nome do segmento.

1. A guia **[!UICONTROL Pessoas]** no **[!UICONTROL Segmento]** agora mostra a lista final de pessoas para o segmento.

   ![](assets/approve-a-segmentation-4.png)

>[!CAUTION]
>
>O número total de segmentos que você pode criar em uma segmentação depende do número e do tipo de filtros usados e também da complexidade da lógica dos seus segmentos. Embora você possa criar até 100 segmentos usando campos padrão, usar outros tipos de filtros pode aumentar a complexidade e sua segmentação pode deixar de ser aprovada. Alguns exemplos são: campos personalizados, membro de lista, campos de proprietário de lead e estágios de receita.
>
>Se você receber uma mensagem de erro durante a aprovação e precisar de assistência para reduzir a complexidade da segmentação, contate o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>[Usar filtros de segmento em uma lista inteligente](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/use-segment-filters-in-a-smart-list.md)
