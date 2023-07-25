---
unique-page-id: 37355758
description: Adicionar membros a um programa de evento - Documentação do Marketo - Documentação do produto
title: Adicionar membros a um programa de evento
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# Adicionar membros a um programa de evento {#adding-members-to-an-event-program}

Este artigo se aplica somente aos usuários que utilizam Limite de evento ou Metas de evento.

>[!CAUTION]
>
>Importar uma lista de pessoas diretamente para um Programa de evento impedirá que esses registros sejam contados em registros reais no relatório Rastreamento de meta e no relatório Progressão de limite do evento. Siga as instruções abaixo para garantir que seus registros sejam contados.

1. Criar e [adicionar pessoas a uma lista estática](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [Criar uma campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

1. Na Smart List da Campanha inteligente criada na Etapa dois, localize e adicione o **Membro da lista** filtro.

   ![](assets/three.png)

1. Localize e selecione a lista criada na Etapa Um.

   ![](assets/four.png)

1. No Fluxo, localize e adicione a variável **Alterar status do programa** etapa do fluxo.

   ![](assets/five.png)

1. Localize e selecione seu Programa de evento.

   ![](assets/six.png)

1. Escolha o status desejado.

   ![](assets/seven.png)

1. Na guia Schedule, clique em **Executar uma vez**.

   ![](assets/eight.png)

1. Selecionar **Executar agora** e clique em **Executar**.

   ![](assets/nine.png)

1. Depois que a campanha inteligente for executada, os membros serão adicionados ao programa e contarão nos cálculos de Rastreamento de meta e Progressão de limite de evento.
