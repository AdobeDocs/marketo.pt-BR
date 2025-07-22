---
unique-page-id: 2949874
description: Criar um evento com [!DNL GotoWebinar] - Documentação do Marketo - Documentação do produto
title: Criar um Evento com [!DNL GotoWebinar]
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 0%

---

# Criar um Evento com [!DNL GotoWebinar] {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [Adicionar [!DNL GoToWebinar] como um [!DNL LaunchPoint] serviço](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [Criar um Novo Programa de Evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Definir as [ações de fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) apropriadas para rastrear o envolvimento

Primeiro, crie seu webinário em [!DNL GoToWebinar]. Certas configurações na criação do seu [!DNL GoToWebinar] são usadas pelo Marketo e algumas somente são usadas pelo [!DNL GoToWebinar].

Depois de criar um evento do Marketo e associar o [!DNL GoToWebinar] a ele, os sistemas poderão compartilhar informações de registro e participação.

Veja abaixo uma lista das configurações usadas pelo Marketo.

## Título e descrição {#title-and-description}

**[!UICONTROL Título]** - insira o nome do webinário. Esse nome poderá ser visto no Marketo.

**[!UICONTROL Descrição]** (opcional) - insira a descrição do webinário. A descrição será exibida no Marketo.

![](assets/image2015-5-28-15-3a1-3a36.png)

## Data e hora {#date-time}

Insira as seguintes informações para seu webinário, que será extraído para o Marketo por meio do adaptador. Se você fizer alterações nessas informações, clique no link &quot;**[!UICONTROL Atualizar do Provedor de Webinar]**&quot; em **[!UICONTROL Ações de Evento]** para que o Marketo veja as alterações.

**[!UICONTROL Data de início]** - digite sua data de início. Ele poderá ser visto no Marketo.

**[!UICONTROL Hora de início]** - digite sua hora de início. Ele poderá ser visto no Marketo.

**[!UICONTROL Hora de Término]** - digite sua hora de término. Ele poderá ser visto no Marketo.

**[!UICONTROL Fuso horário do webinário]** - selecione o fuso horário aplicável. Ele poderá ser visto no Marketo.

**[!UICONTROL Tipo]** - definido como **[!UICONTROL Uma Sessão]**.

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>No momento, o Marketo não oferece suporte a webinários recorrentes. Você deve configurar uma única sessão entre cada Evento Marketo e o webinário [!DNL GoToWebinar].

>[!TIP]
>
>Se precisar de ajuda adicional do [!DNL GoToWebinar], visite o [Site de Ajuda](https://support.logmeininc.com/gotowebinar).

Agora, vamos mergulhar no Marketo!

1. Selecione um evento. Clique em **[!UICONTROL Ações de Eventos]** e escolha **[!UICONTROL Configurações de Eventos]**.

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >O tipo de canal do evento selecionado deve ser **webinário**.

1. Escolha **[!UICONTROL GoToWebinar]** na Lista **[!UICONTROL Parceiro de Evento]**.

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. Escolha a conta.

   ![](assets/rtaimage-2.png)

1. Selecione o webinário.

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. Excelente! Agora o evento é sincronizado e agendado por **[!DNL GoToWebinar]**.

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   >
   >Os campos que o Marketo envia são: Nome, Sobrenome, Endereço de email. Esses campos são obrigatórios e não devem estar vazios.

   >[!TIP]
   >
   >Para popular seu email de confirmação com esta URL exclusiva, use o seguinte token no email: `{{member.webinar url}}`. Quando o URL de confirmação é enviado, esse token é resolvido automaticamente para o URL de confirmação exclusivo da pessoa.
   >
   >Defina seu email de confirmação como **Operacional** para garantir que as pessoas que se registram e podem ter a assinatura cancelada ainda recebam suas informações de confirmação.

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >Evite usar programas de email aninhados para enviar emails de confirmação. Em vez disso, use a campanha inteligente do programa do evento, como mostrado acima.

   >[!TIP]
   >
   >Pode levar até 48 horas para que os dados sejam exibidos no Marketo. Se depois de aguardar tanto tempo você ainda não vir nada, selecione **[!UICONTROL Atualizar do Provedor de Webinar]** no menu [!UICONTROL Ações de Eventos] na guia **[!UICONTROL Resumo]** do seu evento.

As pessoas que se inscreverem no seu webinário serão encaminhadas ao seu provedor do webinário através da etapa de fluxo [!UICONTROL Alterar status do programa] quando o [!UICONTROL Novo status] estiver definido como &quot;Registrado&quot;. Nenhum outro status enviará a pessoa. Além disso, certifique-se de fazer a etapa de fluxo #1 do [!UICONTROL Alterar status do programa] e a etapa de fluxo #2 do [!UICONTROL Enviar email].

## Exibição do Agendamento  {#viewing-the-schedule}

Na exibição de cronograma do programa, clique na entrada de calendário do evento. Você pode ver o cronograma no lado direito da tela.

>[!NOTE]
>
>Para alterar a programação do evento, será necessário editar o webinário em [!DNL GoToWebinar].

![](assets/image2015-5-14-15-3a3-3a13.png)
