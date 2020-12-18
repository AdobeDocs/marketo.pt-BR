---
unique-page-id: 37355758
description: Adicionar membros a um Programa Evento - Documentos do Marketing - Documentação do produto
title: Adicionar membros a um Programa Evento
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Adicionar membros a um Programa de Evento {#adding-members-to-an-event-program}

Este artigo se aplica somente aos usuários que utilizam o Evento Cap ou o Evento de Metas.

>[!CAUTION]
>
>Importar uma lista de pessoas diretamente para um Programa de Evento impedirá que esses registros sejam contados em registros reais no relatório de Rastreamento de metas e no relatório de Progressão de Evento. Siga as instruções abaixo para garantir que seus registros sejam contados.

1. Crie e [adicione pessoas a uma lista estática](http://docs.marketo.com/x/ecKt).
1. [Crie uma campanha](http://docs.marketo.com/x/M4AR) inteligente.
1. Na Lista inteligente da Campanha inteligente criada na Etapa dois, localize e adicione o filtro **Membro da Lista**.

   ![](assets/three.png)

1. Localize e selecione a lista criada na Etapa Um.
1. ![](assets/four.png)

1. No Fluxo, localize e adicione a etapa de fluxo **Alterar status do Programa**.
1. ![](assets/five.png)

1. Localize e selecione seu Programa de Evento.

   ![](assets/six.png)

1. Escolha seu status desejado.

   ![](assets/seven.png)

1. Na guia Agendamento, clique em **Executar uma vez**.
1. ![](assets/eight.png)

1. Selecione **Executar agora** e clique em **Executar**.
1. ![](assets/nine.png)

1. Depois que a campanha inteligente for executada, os membros serão adicionados ao programa e contarão nos cálculos Rastreamento de metas e Progressão de Evento.

