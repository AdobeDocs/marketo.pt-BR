---
unique-page-id: 2949874
description: Criar um Evento com o GotoWebinar - Documentos do Marketing - Documentação do produto
title: Criar um Evento com GotoWebinar
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---


# Criar um Evento com GotoWebinar {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [Adicionar GoToWebinar como um serviço do LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [Criar um novo Programa de Evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Defina as ações de [fluxo apropriadas para](http://docs.marketo.com/display/DOCS/Flow+Actions)rastrear o envolvimento


Primeiro crie seu webinar em GoToWebinar. Determinadas configurações na criação do GoToWebinar são usadas pelo Marketo e algumas são usadas apenas por GoToWebinar.

Depois de criar um evento de marketing e associar o GoToWebinar a ele, os sistemas poderão compartilhar informações de inscrição e presença. Para obter ajuda sobre como criar um GoToWebinar, consulte o Guia [do Usuário do](http://docs.marketo.com/display/docs/assets/gotowebinar-user-guide.pdf)GoToWebinar.

Abaixo está uma lista das configurações usadas por Marketo.

## Título e descrição {#title-and-description}

**Nome** do webinar - insira o nome do webinar. Este nome será visível no Marketo.

**Descrição** (opcional) - insira a descrição do webinar. A descrição será`visualizável no Marketo.

![](assets/image2015-5-28-15-3a1-3a36.png)

## Data e hora {#date-time}

`Enter the following information for your webinar and it will be pulled into Marketo via the`adaptador. Se você fizer alterações nessas informações, clique no link &quot;**Atualizar do provedor** de webinar&quot; em Ações **de** Evento para que o Markeet possa ver as alterações.

**Data** do start - insira a data do start. Isso será visível em Marketo.

**Hora** do start - insira a hora do start. Isso será visível em Marketo.

**Hora** de término - insira a hora de término. Isso será visível em Marketo.

**Fuso horário** - selecione o fuso horário aplicável. Será visível em Marketo.

**Digite -** definido como **Uma sessão**.

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>No momento, o Marketo não suporta webinars recorrentes. Você deve configurar uma única sessão entre cada Evento de marketing e o webinar GoToWebinar.

>[!TIP]
>
>Há campos adicionais que você configurará em GoToWebinar que NÃO afetarão a integração. Consulte o Guia [do usuário do](http://docs.marketo.com/display/docs/assets/gotowebinar-user-guide.pdf) GoToWebinar para obter informações adicionais sobre esses campos, pois eles não serão abordados neste artigo. Se precisar de ajuda adicional do GoToWebinar, visite o Site [de](http://support.logmeininc.com/gotowebinar)Ajuda.

Agora, vamos pular para o Marketo!

1. Selecione um evento. Clique em Ações **do** Evento e escolha Configurações **do** Evento.

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >O tipo de canal do evento selecionado deve ser **webinar**.

1. Escolha **IrParaWebinar** na Lista **Evento** **Parceiro** .

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. Escolha a conta.

   ![](assets/rtaimage-2.png)

1. Selecione o webinar.

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. Clique em **Salvar**.

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. Excelente! Agora o evento é sincronizado e programado por **GoToWebinar**.

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   >
   >Os campos que o Marketo envia são: Nome, Sobrenome, Endereço de email. Esses campos são obrigatórios e não devem estar vazios.

   >[!TIP]
   >
   >Para preencher seu email de confirmação com este URL exclusivo, use o seguinte token no email: `{{member.webinar url}}`. Quando o URL de confirmação é enviado, esse token resolve automaticamente o URL de confirmação exclusivo da pessoa.
   >
   >Defina seu e-mail de confirmação como **Operacional** para garantir que as pessoas que se registram e podem ser canceladas ainda recebam suas informações de confirmação.

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >Evite usar programas de e-mail aninhados para enviar seus e-mails de confirmação. Em vez disso, use a campanha inteligente do programa do evento, como mostrado acima.

   >[!TIP]
   >
   >Pode levar até 48 horas para que os dados apareçam no Marketo. Se, depois de aguardar tanto tempo, você ainda não vir nada, selecione **Atualizar no provedor** de webinar no menu Ações do Evento na guia **Resumo** do evento.

As pessoas que se inscreverem no seu webinar serão encaminhadas para o seu provedor de webinar por meio da etapa de fluxo Alterar status do Programa quando o Novo status estiver definido como &quot;Registrado&quot;. Nenhum outro status empurrará a pessoa. Além disso, certifique-se de fazer a etapa 1 do fluxo Alterar status do Programa e a etapa 2 do fluxo de Enviar e-mail.

## Exibindo a Programação  {#viewing-the-schedule}

Na visualização [do](http://docs.marketo.com/display/docs/program+schedule+view)cronograma do programa, clique na entrada do calendário do evento. Você pode ver o cronograma no lado direito da tela.

>[!NOTE]
>
>Para alterar a programação do evento, é necessário editar o webinar em GoToWebinar.

![](assets/image2015-5-14-15-3a3-3a13.png)
