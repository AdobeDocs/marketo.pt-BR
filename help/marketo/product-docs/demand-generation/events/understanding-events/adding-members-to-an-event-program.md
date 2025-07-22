---
unique-page-id: 37355758
description: Adicionar membros a um programa de evento - Documentação do Marketo - Documentação do produto
title: Adicionar membros a um programa de evento
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
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

1. [Crie uma campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

1. Na Smart List da Campanha Inteligente criada na Etapa Dois, localize e adicione o filtro **[!UICONTROL Membro da Lista]**.

   ![](assets/three.png)

1. Localize e selecione a lista criada na Etapa Um.

   ![](assets/four.png)

1. No Fluxo, localize e adicione a etapa de fluxo **[!UICONTROL Alterar status do programa]**.

   ![](assets/five.png)

1. Localize e selecione seu Programa de evento.

   ![](assets/six.png)

1. Escolha o status desejado.

   ![](assets/seven.png)

1. Na guia [!UICONTROL Agendar], clique em **[!UICONTROL Executar Uma Vez]**.

   ![](assets/eight.png)

1. Selecione **[!UICONTROL Executar agora]** e clique em **[!UICONTROL Executar]**.

   ![](assets/nine.png)

1. Depois que a campanha inteligente for executada, os membros serão adicionados ao programa e contarão nos cálculos de Rastreamento de meta e Progressão de limite de evento.
