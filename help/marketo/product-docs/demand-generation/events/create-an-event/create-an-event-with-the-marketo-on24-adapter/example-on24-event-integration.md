---
unique-page-id: 10096679
description: Exemplo de integração de evento ON24 - Documentos do Marketo - Documentação do produto
title: Exemplo de integração de evento ON24
exl-id: 9d34d1bf-1ff8-4b26-906e-4a6bb9d5f3f6
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Exemplo de integração de evento ON24 {#example-on-event-integration}

>[!IMPORTANT]
>
>A partir de agosto de 2022, o ON24 não será mais compatível com novas integrações do Marketo. As informações neste artigo se aplicam apenas aos usuários existentes.

Este é um exemplo de evento, incluindo campanhas, para um webinário ON24. Ao criar seu evento, certifique-se de testar suas campanhas antes de executá-las.

## Criar um novo evento nas atividades de marketing {#create-a-new-event-in-marketing-activities}

1. Selecionar **Novo** > **Novo programa**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Selecione um **Pasta da campanha** onde o evento viverá.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Insira um **Nome** para o evento .

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Selecionar **Evento** como **Tipo de programa**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Selecionar **Webinar** como **Canal** para o evento .

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Clique em **Criar**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Convidar (Campanha em Lote)  {#invite-batch-campaign}

* **Lista inteligente** - Defina quem você convidará para o evento.
* **Fluxo**

   * Enviar email - Se esse for um email de ativo local, ele terá a seguinte convenção de nomenclatura: EventName.EmailName. Também é possível usar emails globais.
   * Alterar status em progressão - Defina como webinar > Convidado.

* **Agendar** - Defina a data para o envio do convite.

## Registro/Confirmação (Campanha do Acionador) {#registration-confirmation-trigger-campaign}

* **Lista inteligente**

   * Acione a campanha com base em **Preenche Formulário**. Certifique-se de incluir a landing page na qual o formulário reside usando **Adicionar restrição**, especialmente se o formulário for usado em várias landing pages.

>[!CAUTION]
>
>Você deve usar um formulário Marketo para registrar pessoas para o evento ou um formulário que não seja da Marketo com a integração de API adequada para enviar dados de registro para o Marketo. Isso é essencial para o sucesso da integração do Parceiro de eventos. **OBSERVAÇÃO**: Se você estiver usando um formulário Marketo em uma página de aterrissagem que não seja a Marketo, o acionador será **Preenche Formulário** com o Nome do formulário.

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Fluxo**

   * **Alterar Status em Progressão** - Defina como Webinar > Registrado. **CUIDADO**: Essa etapa do fluxo é necessária ao configurar a campanha filho. Quando o status da progressão de uma pessoa muda para **Registrado**, o Marketo envia as informações de registro para ON24.

   * **Enviar Email** - Email de confirmação (definido como **Operacional** para que as pessoas que se inscreveram ainda recebam o registro).

![](assets/image2015-12-22-15-3a52-3a9.png)

**OBSERVAÇÃO**: Se a pessoa for retornada com um erro de registro, ela não receberá a confirmação do email.

## Lembrete (Campanha em lote) {#reminder-batch-campaign}

* **Lista inteligente** - Filtrar usando **Membro do Programa** e defina o status como **Registrado**.

* **Fluxo** - Enviar Email (Email do Lembrete).

**OBSERVAÇÃO**: Você pode usar uma campanha semelhante para enviar uma *different* e-mail de acompanhamento para pessoas que foram convidadas mas que ainda não se registraram.

## Campanha de acompanhamento (Campanha em lote ou acionadora) {#follow-up-campaign-batch-or-trigger-campaign}

* **Lista inteligente** - Acionador com base em alterações no status do programa.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Fluxo** - Enviar Email. Use opções para enviar diferentes emails com base no status do programa.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[Noções básicas sobre os eventos do adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
