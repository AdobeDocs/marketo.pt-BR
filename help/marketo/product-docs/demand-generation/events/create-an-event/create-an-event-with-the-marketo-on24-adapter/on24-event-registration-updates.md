---
unique-page-id: 10096683
description: Atualizações do registro de eventos ON24 - Documentação do Marketo - Documentação do produto
title: Atualizações de registro de evento ON24
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# Atualizações de registro de evento ON24 {#on-event-registration-updates}

## Aprovando Inscritos Manualmente {#manually-approving-registrants}

Você pode aprovar manualmente seus inscritos antes de enviar a eles um email de confirmação. Para fazer isso, será necessário configurar suas campanhas para lidar com essa etapa adicional:

1. Para a campanha Registration Trigger:

   * Na [!UICONTROL Smart List], defina o acionador como **[!UICONTROL Preenche o Formulário]**.
   * No Fluxo, defina o [!UICONTROL Status em Progressão] como **[!UICONTROL Aprovação Pendente]**.

1. Vá para o Evento e clique na guia **[!UICONTROL Membros]**. Esta guia exibe todas as pessoas que preencheram o formulário. O status deve estar definido como **[!UICONTROL Aprovação Pendente]**.
1. Use o filtro na parte superior da grade para exibir apenas as pessoas com o status **[!UICONTROL Aprovação Pendente]**.
1. Selecione as pessoas que deseja registrar (clique com a tecla Shift pressionada, clique com a tecla Control pressionada ou selecione tudo).
1. No menu, clique em **[!UICONTROL Alterar status]**. Selecione **[!UICONTROL Registrado]**, **[!UICONTROL Rejeitado]** ou qualquer outro status aplicável.

## Lidar com pessoas com um erro de registro {#handling-people-with-a-registration-error}

Se uma pessoa acabar não sendo registrada, mas estiver definida para o status [!UICONTROL Erro de Registro], não será tarde demais para recuperação.

1. Na guia [!UICONTROL Membros], filtre a lista de pessoas com o status **[!UICONTROL Erro de Registro]**.
1. Antes de continuar, verifique se você determinou e corrigiu o problema na integração (verifique se não há erros em **[!UICONTROL Parceiros de eventos]** no Admin).
1. Depois que o problema for resolvido, selecione todas as pessoas com o status [!UICONTROL Erro de Registro] e altere seu status para **[!UICONTROL Registrado]**. Isso tentará registrá-los novamente com ON24.

## Atualizando Status do Membro de ON24 {#updating-member-status-from-on}

A Marketo registra automaticamente as informações de presença às 23h00 da Pacific, aproximadamente, todas as noites. Para atualizar manualmente as informações de participação, clique em **[!UICONTROL Atualizar do Provedor de Webinar]** em **[!UICONTROL Ações de Evento]**.

>[!MORELIKETHIS]
>
>[Noções Básicas sobre os Eventos do Adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
