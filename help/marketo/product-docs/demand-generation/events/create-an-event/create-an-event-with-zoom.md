---
unique-page-id: 17728023
description: Criar um evento com [!DNL Zoom] - Documentação do Marketo - Documentação do produto
title: Criar um Evento com [!DNL Zoom]
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 0%

---

# Criar um Evento com [!DNL Zoom] {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Adicionar [!DNL Zoom] como um [!DNL LaunchPoint] Serviço](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [Criar um Novo Programa de Evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Definir as [ações de fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) apropriadas para rastrear o envolvimento

Primeiro, crie seu webinário em [!DNL Zoom]. Certas configurações na criação do seu [!DNL Zoom] são usadas pelo Marketo, e algumas somente são usadas pelo [!DNL Zoom].

Depois de criar um evento do Marketo e associar um webinário do [!DNL Zoom] a ele, os sistemas poderão compartilhar informações de registro e participação. Para obter ajuda sobre como criar um webinário, consulte [Introdução aos [!DNL Zoom] webinários](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar).

Insira as seguintes informações para seu webinário, que será extraído para o Marketo por meio do adaptador. Se você fizer alterações nessas informações, deverá clicar no link &quot;Atualizar do provedor de webinários&quot; em Ações de evento para que o Marketo veja as alterações.

**Título e Descrição**

* **Nome do webinário** - Digite o nome do webinário. Esse nome poderá ser visto no Marketo.

* **Descrição** (opcional) - Insira a descrição do webinário. A descrição será exibida no Marketo.

**Data e hora**

* **Data de início** - Digite a data de início. Ele poderá ser visto no Marketo.

* **Hora de início** - Digite sua hora de início. Ele poderá ser visto no Marketo.

* **Duração** - Insira a duração. A hora de início e a hora de término serão exibidas no Marketo.

* **Fuso Horário** - Selecione o fuso horário aplicável. Ele poderá ser visto no Marketo.

* **Webinar recorrente**- Mantenha desmarcado.

* **Registro** - Marque esta caixa para tornar o registro obrigatório. Você usará um formulário/página de aterrissagem do Marketo para capturar as informações de registro que serão enviadas para [!DNL Zoom].

>[!NOTE]
>
>No momento, o Marketo não oferece suporte a webinários recorrentes. Você deve configurar uma única sessão entre cada Evento Marketo e o webinário [!DNL Zoom].

![](assets/overview2.png)

>[!TIP]
>
>Você configurará outros campos no [!DNL Zoom] que NÃO afetarão a integração. Consulte a [[!DNL Zoom] Central de ajuda do webinário](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar) para obter informações adicionais sobre esses campos.

Agora, vamos mergulhar no Marketo!

1. Selecione um evento. Clique em **[!UICONTROL Ações de Eventos]** e escolha **[!UICONTROL Configurações de Eventos]**.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >O tipo de canal do evento selecionado deve ser **webinário**.

1. Escolha **[!UICONTROL Zoom]** na Lista **[!UICONTROL Parceiro de Evento]**.

   ![](assets/eventsettings1.png)

1. Escolha a conta do [!DNL Zoom] à qual você deseja associar o evento.

   ![](assets/selectaccount.png)

1. Selecione o webinário.

   ![](assets/selectevent.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/eventsettingssave.png)

   Excelente! Agora o evento é sincronizado e agendado por [!DNL Zoom].

   >[!NOTE]
   >
   >Os campos que o Marketo envia são: Nome, Sobrenome, Endereço de email.

   >[!TIP]
   >
   >Para popular seu email de confirmação com esta URL exclusiva, use o seguinte token no email: `{{member.webinar url}}`. Quando o URL de confirmação é enviado, esse token é resolvido automaticamente para o URL de confirmação exclusivo da pessoa.
   >
   >Defina seu email de confirmação como **Operacional** para garantir que as pessoas que se registram e podem ter a assinatura cancelada ainda recebam suas informações de confirmação.

   As pessoas que se inscreverem no seu webinário serão encaminhadas ao seu provedor do webinário através da etapa de fluxo **[!UICONTROL Alterar status do programa]** quando o [!UICONTROL Novo status] estiver definido como &quot;Registrado&quot;. Nenhum outro status enviará a pessoa. Além disso, certifique-se de fazer a etapa de fluxo #1 do **[!UICONTROL Alterar status do programa]** e a etapa de fluxo #2 do **[!UICONTROL Enviar email]**.

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >Evite usar programas de email aninhados para enviar emails de confirmação. Em vez disso, use a campanha inteligente do programa do evento, como mostrado acima.

   >[!TIP]
   >
   >Pode levar até 48 horas para que os dados sejam exibidos no Marketo. Se depois de aguardar tanto tempo você ainda não vir nada, selecione **Atualizar do Provedor de Webinar** no menu Ações de Evento na guia **Resumo** do evento e clique no ícone de atualização na parte inferior direita da tela.
