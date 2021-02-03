---
unique-page-id: 10096679
description: Exemplo de integração de Evento ON24 - Documentos do Marketing - Documentação do produto
title: Exemplo de integração de Evento ON24
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# Exemplo de integração de Evento ON24 {#example-on-event-integration}

Aqui está um exemplo de evento, incluindo o campanha, para um webinar ON24. Ao criar seu evento, teste suas campanhas antes de executá-las.

## Criar um novo Evento no Marketing Atividade {#create-a-new-event-in-marketing-activities}

1. Selecione **Novo** > **Novo Programa**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Selecione uma **Pasta de Campanha** na qual o evento permanecerá ativo.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Digite um **Nome** para o evento.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Selecione **Evento** como **Tipo de Programa**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Selecione **Webinar** como o **Canal** para o evento.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Clique em **Criar**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Convidar (Campanha em lote) {#invite-batch-campaign}

* **Lista**  inteligente - Defina quem você convidará para o evento.
* **Fluxo**

   * Enviar email - se for um email de ativo local, ele terá a seguinte convenção de nomenclatura: EventName.EmailName. Você também pode usar emails globais.
   * Alterar status na progressão - Defina como Webinar > Convidado.

* **Agendamento**  - Defina a data para o envio do convite.

## Registro/confirmação (Campanha do acionador) {#registration-confirmation-trigger-campaign}

* **Lista inteligente**

   * Acione a campanha com base em **Preenche o formulário**. Certifique-se de incluir a landing page na qual o formulário permanece usando **Adicionar restrição**, especialmente se o formulário for usado em várias landings page.

>[!CAUTION]
>
>É necessário usar um formulário do Marketo para registrar pessoas para o evento ou um formulário que não seja do tipo Marketo com a integração da API adequada para enviar dados de registro para o Marketo. Isso é fundamental para o sucesso da integração do Parceiro do Evento. **NOTA**: Se você estiver usando um formulário Marketo em uma landing page que não seja Marketo, seu acionador será  **Preencher o** formulário com o Nome do formulário.

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Fluxo**

   * **Alterar status na progressão**  - Defina como Webinar > Registrado. **CUIDADO**: Essa etapa de fluxo é necessária ao configurar a campanha secundária. Quando o status de progressão de uma pessoa muda para **Registered**, Marketo envia as informações de registro para ON24.

   * **Enviar e-mail**  - o e-mail de confirmação (definido como  **** Operaçãotambém indica que as pessoas que se registraram e que ainda o receberam).

![](assets/image2015-12-22-15-3a52-3a9.png)

**NOTA**: Se a pessoa for devolvida com um erro de registro, ela não receberá a confirmação do email.

## Lembrete (Campanha em lote) {#reminder-batch-campaign}

* **Lista**  inteligente - filtre usando o  **Membro do** programa e defina o status como  **Registrado**.

* **Fluxo**  - Enviar email (Email do lembrete).

**NOTA**: Você poderia usar uma campanha semelhante para enviar um e-mail de acompanhamento  ** diferente para pessoas que foram convidadas, mas que ainda não se registraram.

## Campanha de acompanhamento (Campanha em lote ou acionador) {#follow-up-campaign-batch-or-trigger-campaign}

* **Lista**  inteligente - Acionador com base nas alterações no status do programa.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Fluxo**  - Enviar email. Use as opções para enviar e-mails diferentes com base no status do programa.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[Noções Gerais dos Eventos do adaptador do Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
