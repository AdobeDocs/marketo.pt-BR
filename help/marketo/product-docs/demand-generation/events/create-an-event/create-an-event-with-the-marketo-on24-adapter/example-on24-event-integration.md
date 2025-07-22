---
unique-page-id: 10096679
description: Exemplo de integração de evento ON24 - Documentação do Marketo - Documentação do produto
title: Exemplo de integração de evento ON24
exl-id: 9d34d1bf-1ff8-4b26-906e-4a6bb9d5f3f6
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Exemplo de integração de evento ON24 {#example-on-event-integration}

Este é um evento de amostra, incluindo campanhas, para um webinário ON24. Ao criar seu evento, certifique-se de testar suas campanhas antes de executá-las.

## Criar um novo evento em atividades de marketing {#create-a-new-event-in-marketing-activities}

1. Selecione **[!UICONTROL Novo]** > **[!UICONTROL Novo programa]**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Selecione uma **[!UICONTROL Pasta de campanha]** onde o evento irá viver.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Digite um **[!UICONTROL Nome]** para o evento.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Selecione **[!UICONTROL Evento]** como o **[!UICONTROL Tipo de Programa]**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Selecione **[!UICONTROL Webinar]** como o **[!UICONTROL Canal]** para o evento.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Clique em **[!UICONTROL Criar]**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Convidar (Campanha em Lote)  {#invite-batch-campaign}

* **Smart List** - Defina quem você convidará para o evento.
* **Fluxo**

   * Enviar email - Se esse for um email de ativo local, ele terá a seguinte convenção de nomenclatura: EventName.EmailName. Você também pode usar emails globais.
   * Alterar status na progressão - Defina como Webinar > Convidado.

* **Agendar** - Defina a data para o convite a ser enviado.

## Registro/Confirmação (Acionar campanha) {#registration-confirmation-trigger-campaign}

* **Lista Inteligente**

   * Acione a campanha com base no **[!UICONTROL Formulário de Preenchimento]**. Certifique-se de incluir a página de aterrissagem em que o formulário está usando **[!UICONTROL Adicionar restrição]**, especialmente se o formulário for usado em várias páginas de aterrissagem.

>[!CAUTION]
>
>Você deve usar um formulário do Marketo para registrar pessoas para o evento ou um formulário que não seja do Marketo com a integração de API adequada para enviar dados de registro para o Marketo. Isso é essencial para o sucesso da sua integração com o [!UICONTROL Parceiro de Evento]. **OBSERVAÇÃO**: se você estiver usando um formulário do Marketo em uma página de aterrissagem que não seja da Marketo, seu acionador será **[!UICONTROL Preencher formulário]** com o [!UICONTROL Nome do formulário].

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Fluxo**

   * **Alterar Status na Progressão** - Defina como Webinar > Registrado. **ATENÇÃO**: esta etapa de fluxo é necessária ao configurar sua campanha filho. Quando o status de progressão de uma pessoa é alterado para **Registrada**, o Marketo envia as informações de registro para ON24.

   * **Enviar Email** - Email de confirmação (definido como **Operacional** para que as pessoas com assinatura cancelada que se registraram ainda recebam).

![](assets/image2015-12-22-15-3a52-3a9.png)

**OBSERVAÇÃO**: se a pessoa retornar com um erro de registro, ela não receberá o email de confirmação.

## Lembrete (Campanha em Lote) {#reminder-batch-campaign}

* **Smart List** - Filtrar usando **Membro do Programa** e definir o status como **Registrado**.

* **Fluxo** - Enviar Email (Email de Lembrete).

**OBSERVAÇÃO**: você poderia usar uma campanha semelhante para enviar um email de acompanhamento *diferente* para pessoas convidadas, mas que ainda não se registraram.

## Campanha de acompanhamento (campanha em lote ou de acionador) {#follow-up-campaign-batch-or-trigger-campaign}

* **Smart List** - Acionar com base nas alterações no status do programa.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Fluxo** - Enviar Email. Use opções para enviar emails diferentes com base no status do programa.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[Noções Básicas sobre os Eventos do Adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
