---
unique-page-id: 2359947
description: Transição de pessoas entre fluxos de envolvimento - Documentos do Marketo - Documentação do produto
title: Transição de pessoas entre fluxos de envolvimento
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 1%

---

# Transição de pessoas entre fluxos de envolvimento {#transition-people-between-engagement-streams}

Os programas de envolvimento podem ter mais de um fluxo. Se você [adicionar um fluxo](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), você desejará definir uma maneira de as pessoas se moverem de um fluxo para outro. Eles são chamados de **regras de transição.**

1. Ir para **Atividades de marketing**.

   ![](assets/ma.png)

1. Selecione seu programa de engajamento em várias etapas e acesse **Fluxos**.

   ![](assets/multistream.jpg)

1. Clique em **Regras de transição** para o fluxo que você deseja obter de outros fluxos, clique em **Editar regras de transição**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >As regras de transição entram em um fluxo; sempre defina as regras no fluxo que deseja obter.

   Quando a janela da regra de transição for aberta, localize e arraste o acionador de sua escolha. Nesse caso, queremos mover as pessoas para o Mid Stage quando ele for adicionado a uma oportunidade.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Vamos definir o operador como **é qualquer** para que as pessoas se movimentem para qualquer oportunidade adicional.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >Você pode adicionar vários acionadores e filtros a uma regra de transição, mas a regra de transição usa todos os filtros (usar TODOS os filtros é a única opção). Se você precisar usar OU em uma regra de transição, recomendamos configurar uma campanha inteligente externa.

1. Clique em **Fechar**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Ótimo! Agora, qualquer pessoa em seu programa de envolvimento que seja adicionada a uma oportunidade será movida para o fluxo de Preparo intermediário .

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >As etapas descritas acima *do* aplicar a pessoas que [ao pausar](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md) também.
