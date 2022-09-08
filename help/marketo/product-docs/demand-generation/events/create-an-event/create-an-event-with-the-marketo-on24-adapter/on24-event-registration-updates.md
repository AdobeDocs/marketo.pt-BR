---
unique-page-id: 10096683
description: Atualizações do registro de eventos ON24 - Documentos do Marketo - Documentação do produto
title: Atualizações do registro de eventos ON24
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Atualizações do registro de eventos ON24 {#on-event-registration-updates}

>[!IMPORTANT]
>
>A partir de agosto de 2022, o ON24 não será mais compatível com novas integrações do Marketo. As informações neste artigo se aplicam apenas aos usuários existentes.

## Aprovar Registrantes Manualmente {#manually-approving-registrants}

Você pode aprovar manualmente seus registrantes antes de enviar um email de confirmação para eles. Para fazer isso, será necessário configurar suas campanhas para lidar com esta etapa adicional:

1. Para a campanha do Acionador de registro:

   * Na Smart List, defina o acionador como **Preenche Formulário**.
   * No Fluxo, defina o Status em Progressão como **Aprovação pendente**.

1. Vá para o Evento e clique no botão **Membros** guia . Essa guia exibe todas as pessoas que preencheram o formulário. Seu status deve ser definido como **Aprovação pendente**.
1. Use o filtro na parte superior da grade para exibir apenas as pessoas com status de **Aprovação pendente**.
1. Selecione as pessoas que deseja registrar (clique com a tecla Shift pressionada, clique com a tecla Control pressionada ou selecione todas).
1. No menu, clique em **Alterar Status**. Selecionar **Registrado**, **Rejeitada** ou qualquer outro status aplicável.

## Lidar com pessoas com um erro de registro {#handling-people-with-a-registration-error}

Se uma pessoa acabar não sendo registrada, mas sim definida como status Erro de registro, não é tarde demais para se recuperar.

1. Na guia Membros , filtre a lista de pessoas com o status **Erro de Registro**.
1. Antes de continuar, verifique se você determinou e corrigiu o problema com a integração (verifique se não há erros em **Parceiros de evento** em Admin).
1. Depois que o problema for resolvido, selecione todas as pessoas com o status de Erro de Registro e altere seu status para **Registrado**. Isso tentará registrá-los novamente com ON24.

## Atualizando o Status do Membro a partir do ON24 {#updating-member-status-from-on}

A Marketo coleta automaticamente as informações de presença aproximadamente às 23 horas do Pacífico por noite. Para atualizar manualmente as informações de presença, clique em **Atualizar do provedor de webinar** under **Ações do evento**.

>[!MORELIKETHIS]
>
>[Noções básicas sobre os eventos do adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
