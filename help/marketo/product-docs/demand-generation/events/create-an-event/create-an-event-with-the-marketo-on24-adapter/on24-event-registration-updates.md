---
unique-page-id: 10096683
description: Atualizações do registro de eventos ON24 - Documentação do Marketo - Documentação do produto
title: Atualizações de registro de evento ON24
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# Atualizações de registro de evento ON24 {#on-event-registration-updates}

## Aprovando Inscritos Manualmente {#manually-approving-registrants}

Você pode aprovar manualmente seus inscritos antes de enviar a eles um email de confirmação. Para fazer isso, será necessário configurar suas campanhas para lidar com essa etapa adicional:

1. Para a campanha Registration Trigger:

   * Na Smart List, defina o acionador como **Preenche o Formulário**.
   * No Fluxo, defina o Status em Progressão como **Aprovação pendente**.

1. Vá para o Evento e clique na guia **Membros**. Esta guia exibe todas as pessoas que preencheram o formulário. O status deve estar definido como **Aprovação Pendente**.
1. Use o filtro na parte superior da grade para exibir apenas as pessoas com o status **Aprovação Pendente**.
1. Selecione as pessoas que deseja registrar (clique com a tecla Shift pressionada, clique com a tecla Control pressionada ou selecione tudo).
1. No menu, clique em **Alterar status**. Selecione **Registrado**, **Rejeitado** ou qualquer outro status aplicável.

## Lidar com pessoas com um erro de registro {#handling-people-with-a-registration-error}

Se uma pessoa acabar não sendo registrada, mas sim definida com o status Erro de registro, não é tarde demais para se recuperar.

1. Na guia Membros, filtre a lista de pessoas com o status **Erro de Registro**.
1. Antes de continuar, verifique se você determinou e corrigiu o problema na integração (verifique se não há erros em **Parceiros de eventos** no Admin).
1. Depois que o problema for resolvido, selecione todas as pessoas com o status de Erro de Registro e altere seu status para **Registrado**. Isso tentará registrá-los novamente com ON24.

## Atualizando Status do Membro de ON24 {#updating-member-status-from-on}

A Marketo registra automaticamente as informações de presença às 23h00 da Pacific, aproximadamente, todas as noites. Para atualizar manualmente as informações de participação, clique em **Atualizar do Provedor de Webinar** em **Ações de Evento**.

>[!MORELIKETHIS]
>
>[Noções Básicas sobre os Eventos do Adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
