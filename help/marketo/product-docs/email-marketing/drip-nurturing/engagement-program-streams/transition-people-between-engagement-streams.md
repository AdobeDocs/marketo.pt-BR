---
unique-page-id: 2359947
description: Transição De Pessoas Entre Fluxos De Envolvimento - Documentação Do Marketo - Documentação Do Produto
title: Fazer Transição De Pessoas Entre Fluxos De Envolvimento
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 1%

---

# Fazer Transição De Pessoas Entre Fluxos De Envolvimento {#transition-people-between-engagement-streams}

Os programas de engajamento podem ter mais de um fluxo. Se você [adicionar um fluxo](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), desejará definir uma maneira de as pessoas moverem-se de um fluxo para outro. Elas são chamadas de **regras de transição.**

1. Vá para **Atividades de marketing**.

   ![](assets/ma.png)

1. Selecione seu programa de envolvimento multi-streaming e vá para **Streams**.

   ![](assets/multistream.jpg)

1. Clique em **Regras de transição** para o fluxo que você deseja obter de outros fluxos e clique em **Editar regras de transição**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >As regras de transição são extraídas em um fluxo; sempre defina as regras no fluxo para o qual você deseja extrair.

   Quando a janela da regra de transição for aberta, localize e arraste o acionador de sua escolha. Nesse caso, queremos mover as pessoas para o Mid Stage quando ele for adicionado a uma oportunidade.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Vamos definir o operador como **é qualquer** para que as pessoas se movam para qualquer oportunidade adicional.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >É possível adicionar vários acionadores e filtros a uma regra de transição, mas a regra de transição usa todos os filtros (usar TODOS os filtros é a única opção). Se você precisar usar OU em uma regra de transição, recomendamos que você configure uma campanha inteligente externa.

1. Clique em **Fechar**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Ótimo! Agora, qualquer pessoa em seu programa de engajamento que for adicionada a uma oportunidade será movida para o fluxo do Estágio intermediário.

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >As etapas descritas acima *não* aplicam-se também às pessoas que estão [em pausa](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md).
