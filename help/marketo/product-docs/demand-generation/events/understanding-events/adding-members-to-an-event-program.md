---
unique-page-id: 37355758
description: Adicionar membros a um Programa Evento - Documentos do Marketing - Documentação do produto
title: Adicionar membros a um Programa Evento
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# Adicionar membros a um Programa de Evento {#adding-members-to-an-event-program}

Este artigo se aplica somente aos usuários que utilizam o Evento Cap ou o Evento de Metas.

>[!CAUTION]
>
>Importar uma lista de pessoas diretamente para um Programa de Evento impedirá que esses registros sejam contados em registros reais no relatório de Rastreamento de metas e no relatório de Progressão de Evento. Siga as instruções abaixo para garantir que seus registros sejam contados.

1. Crie e [adicione pessoas a uma lista estática](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [Crie uma campanha](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) inteligente.

1. Na Lista inteligente da Campanha inteligente criada na Etapa dois, localize e adicione o filtro **Membro da Lista**.

   ![](assets/three.png)

1. Localize e selecione a lista criada na Etapa Um.

   ![](assets/four.png)

1. No Fluxo, localize e adicione a etapa de fluxo **Alterar status do Programa**.

   ![](assets/five.png)

1. Localize e selecione seu Programa de Evento.

   ![](assets/six.png)

1. Escolha seu status desejado.

   ![](assets/seven.png)

1. Na guia Agendamento, clique em **Executar uma vez**.

   ![](assets/eight.png)

1. Selecione **Executar agora** e clique em **Executar**.

   ![](assets/nine.png)

1. Depois que a campanha inteligente for executada, os membros serão adicionados ao programa e contarão nos cálculos Rastreamento de metas e Progressão de Evento.
