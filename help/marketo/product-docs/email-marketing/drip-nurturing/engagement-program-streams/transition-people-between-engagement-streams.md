---
unique-page-id: 2359947
description: Transição de pessoas entre fluxos de envolvimento - documentos do Marketo - Documentação do produto
title: Transição de pessoas entre fluxos de envolvimento
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# Transição de pessoas entre fluxos de envolvimento {#transition-people-between-engagement-streams}

Os programas de envolvimento podem ter mais de um fluxo. Se você [adicionar um fluxo](../../../../product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), será necessário definir uma maneira de as pessoas se moverem de um fluxo para outro. São chamadas de regras de **transição.**

1. Vá para **Marketing Atividade**.

   ![](assets/ma.png)

1. Selecione seu programa de envolvimento com várias linhas e vá para **Streams**.

   ![](assets/multistream.jpg)

1. Clique em Regras **de** Transição para o fluxo que deseja obter de outros fluxos e clique em **Editar regras de Transição. **

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >As regras de transição entram num fluxo; sempre defina as regras no fluxo que deseja obter.

   Quando a janela da regra de transição for aberta, localize e arraste o seu acionador de escolha. Neste caso, queremos mover pessoas para o Nível Médio quando for adicionado a uma oportunidade.
` ![](assets/image2014-9-15-18-3a10-3a46.png)

   `

1. Vamos definir o operador como*** é qualquer** para que as pessoas mudem para qualquer oportunidade adicional.

   ` ![](assets/image2014-9-15-18-3a11-3a14.png)

   `

   >[!TIP]
   >
   >Você pode adicionar vários disparadores e filtros a uma regra de transição, mas a regra de transição usa todos os filtros (usar TODOS os filtros é a única opção). Se precisar usar OU em uma regra de transição, recomendamos que você configure uma campanha inteligente externa.

1. Clique em **Fechar**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Ótimo! Agora qualquer pessoa em seu programa de envolvimento que for adicionada a uma oportunidade será movida para o fluxo de médio estágio.

   ` ![](assets/image2014-9-15-18-3a11-3a29.png)

   `

   >[!NOTE]
   >
   >As etapas descritas acima *se aplicam* às pessoas que estão [em pausa](http://docs.marketo.com/display/DOCS/Pause+People+in+an+Engagement+Program) também.

