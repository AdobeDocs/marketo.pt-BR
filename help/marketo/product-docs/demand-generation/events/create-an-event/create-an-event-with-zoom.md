---
unique-page-id: 17728023
description: Criar um Evento com Zoom - Documentos do Marketing - Documentação do produto
title: Criar um Evento com zoom
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---


# Criar um Evento com zoom {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Adicionar Zoom como um Serviço do LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [Criar um novo Programa de Evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Defina as ações de [fluxo apropriadas para](http://docs.marketo.com/display/DOCS/Flow+Actions)rastrear o envolvimento


Primeiro crie seu webinar em Zoom. Determinadas configurações na criação do seu Zoom são usadas pelo Marketo e algumas são usadas apenas pelo Zoom.

Depois que você criar um evento de marketing e associar um webinar de zoom a ele, os sistemas poderão compartilhar informações de inscrição e presença. Para obter ajuda para criar um webinar, consulte [Introdução aos webinars](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar)de zoom.

Digite as seguintes informações para seu webinar e ele será colocado no Marketo por meio do adaptador. Se você fizer alterações nessas informações, clique no link &quot;Atualizar do provedor de webinar&quot; em Ações do Evento para que o Marketo possa ver as alterações.

**Título e descrição**

* **Nome** do webinar - Insira o nome do webinar. Este nome será visível no Marketo.

* **Descrição** (opcional) - Insira a descrição do webinar. A descrição será`visualizável no Marketo.

**Data e hora**

* **Data** do start - Informe a data do start. Isso será visível em Marketo.

* **Hora** do start - insira a hora do start. Isso será visível em Marketo.

* **Duração** - Informe a duração. A hora e a hora de término do start serão visíveis no Marketo.

* **Fuso horário** - Selecione o fuso horário aplicável. Isso será visível em Marketo.

* **Webinar** recorrente - Manter desmarcado.

* **Registro** - Marque esta caixa para tornar obrigatório o registro. Você usará um formulário/landing page de marketing para capturar informações de registro que serão enviadas para Zoom.

>[!NOTE]
>
>No momento, o Marketo não suporta webinars recorrentes. Você deve configurar uma única sessão entre cada Evento de Marketo e webinar de Zoom.

![](assets/overview2.png)

>[!TIP]
>
>Há campos adicionais que você configurará no Zoom que NÃO afetarão a integração. Consulte a Central [de ajuda do Webinar de](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar) zoom para obter informações adicionais sobre esses campos.

Agora, vamos pular para o Marketo!

1. Selecione um evento. Clique em Ações **do** Evento e escolha Configurações **do** Evento.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >O tipo de canal do evento selecionado deve ser **webinar**.

1. Escolha **Zoom** na Lista **Evento** **Partner** .

   ![](assets/eventsettings1.png)

1. Escolha a conta Zoom à qual deseja associar o evento.

   ![](assets/selectaccount.png)

1. Selecione o webinar.

   ![](assets/selectevent.png)

1. Clique em **Salvar**.

   ![](assets/eventsettingssave.png)

   Excelente! Agora o evento é sincronizado e programado pelo Zoom.

   >[!NOTE]
   >
   >Os campos que o Marketo envia são: Nome, Sobrenome, Endereço de email.

   >[!TIP]
   >
   >Para preencher seu email de confirmação com este URL exclusivo, use o seguinte token no email: `{{member.webinar url}}`. Quando o URL de confirmação é enviado, esse token resolve automaticamente o URL de confirmação exclusivo da pessoa.
   >
   >Defina seu e-mail de confirmação como **Operacional** para garantir que as pessoas que se registram e podem ser canceladas ainda recebam suas informações de confirmação.

   As pessoas que se inscreverem no seu webinar serão encaminhadas para o seu provedor de webinar por meio da etapa de fluxo **Alterar status** do Programa quando o Novo status estiver definido como &quot;Registrado&quot;. Nenhum outro status empurrará a pessoa. Além disso, certifique-se de fazer com que a etapa 1 do fluxo **Alterar status** do Programa e a etapa 2 do fluxo de **Enviar e-mail** .

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >Evite usar programas de e-mail aninhados para enviar seus e-mails de confirmação. Em vez disso, use a campanha inteligente do programa do evento, como mostrado acima.

   >[!TIP]
   >
   >Pode levar até 48 horas para que os dados apareçam no Marketo. Se, depois de aguardar tanto tempo, você ainda não vir nada, selecione **Atualizar no provedor** de webinar no menu Ações do Evento na guia **Resumo** do evento.
