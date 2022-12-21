---
unique-page-id: 37355758
description: Adicionar membros a um programa de evento - Documentos da Marketo - Documentação do produto
title: Adicionar membros a um programa de evento
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# Adicionar membros a um programa de evento {#adding-members-to-an-event-program}

Este artigo se aplica somente aos usuários que utilizam o Event Cap ou o Event Targets.

>[!CAUTION]
>
>Importar uma lista de pessoas diretamente para um Programa de Eventos impedirá que esses registros sejam contados em registros reais no relatório de Rastreamento de Meta e no relatório de Progressão de Limite de Eventos. Siga as instruções abaixo para garantir que seus registros sejam contados.

1. Criar e [adicionar pessoas a uma lista estática](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [Criar uma campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

1. Na Smart List (Lista inteligente) da campanha inteligente criada na etapa dois, encontre e adicione o **Membro da Lista** filtro.

   ![](assets/three.png)

1. Localize e selecione a lista criada na Etapa um.

   ![](assets/four.png)

1. No Fluxo, localize e adicione o **Alterar status do programa** etapa de fluxo.

   ![](assets/five.png)

1. Localize e selecione seu Programa de eventos.

   ![](assets/six.png)

1. Escolha o status desejado.

   ![](assets/seven.png)

1. Na guia Agendamento , clique em **Executar uma vez**.

   ![](assets/eight.png)

1. Selecionar **Executar agora** e clique em **Executar**.

   ![](assets/nine.png)

1. Após a execução da campanha inteligente, os membros são adicionados ao programa e contarão nos cálculos Rastreamento de meta e Progressão de limite de evento .
