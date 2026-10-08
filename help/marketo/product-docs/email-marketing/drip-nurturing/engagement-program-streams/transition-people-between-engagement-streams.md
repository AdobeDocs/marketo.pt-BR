---
unique-page-id: 2359947
description: Saiba como configurar regras de transição para mover pessoas entre fluxos de envolvimento. Defina as regras no fluxo para o qual você deseja obter.
title: Fazer a transição de pessoas entre fluxos de engajamento
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
TQID: 'https://experienceleague.adobe.com/viGLYAkvGqF-9K5bhAHWDSOMYaiBuKRe8F2QginuYps'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: fc5011cf-5b46-40b1-a5de-d7f042f85633
    internal-label: Engagement programs
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 6%
---
# Fazer a transição de pessoas entre fluxos de engajamento {#transition-people-between-engagement-streams}

Os programas de engajamento podem ter mais de um fluxo. Se você [adicionar um fluxo](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), defina uma maneira para as pessoas moverem-se de um fluxo para outro. Elas são chamadas de **regras de transição.**

1. Acesse **[!UICONTROL Atividades de marketing]**.

   ![](assets/ma.png)

1. Selecione seu programa de envolvimento multi-streaming e vá para **[!UICONTROL Streams]**.

   ![](assets/multistream.jpg)

1. Clique em **[!UICONTROL Regras de transição]** para o fluxo que você deseja obter de outros fluxos e clique em **[!UICONTROL Editar regras de transição]**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >As regras de transição são extraídas em um fluxo; sempre defina as regras no fluxo para o qual você deseja extrair.

   Quando a janela da regra de transição for aberta, localize e arraste o acionador de sua escolha. Neste exemplo, as pessoas serão movidas para o [!UICONTROL Estágio intermediário] quando adicionadas a uma oportunidade.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Defina o operador como **[!UICONTROL is any]** para que as pessoas se movam para qualquer oportunidade adicionada.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >É possível adicionar vários acionadores e filtros a uma regra de transição, mas a regra de transição usa todos os filtros (usar TODOS os filtros é a única opção). Se você precisar usar OU em uma regra de transição, é recomendável configurar uma campanha inteligente externa.

1. Clique em **[!UICONTROL Fechar]**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Agora, qualquer pessoa em seu programa de engajamento que for adicionada a uma oportunidade será movida para o fluxo de [!UICONTROL Estágio intermediário].

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >As etapas descritas acima *não* aplicam-se também às pessoas que estão [em pausa](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md).
