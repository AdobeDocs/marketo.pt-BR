---
unique-page-id: 2949874
description: Criar um evento com o GotoWebinar - Documentos do Marketo - Documentação do produto
title: Criar um evento com o GotoWebinar
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
source-git-commit: 8b0625a7192a80986bc4295726cd13473493ddd7
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Criar um evento com o GotoWebinar {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [Adicionar o GoToWebinar como um serviço do LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [Criar um novo programa de evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Defina as [ações de fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)para rastrear o envolvimento


Primeiro crie seu webinário em GoToWebinar. Determinadas configurações na criação do seu GoToWebinar são usadas pelo Marketo e algumas são usadas apenas pelo GoToWebinar.

Depois de criar um evento do Marketo e associar o GoToWebinar a ele, os sistemas poderão compartilhar informações de registro e presença.

Abaixo está uma lista das configurações usadas pelo Marketo.

## Título e descrição {#title-and-description}

**Nome do webinar** - digite o nome do webinário. Esse nome estará visível no Marketo.

**Descrição** (opcional) - insira a descrição do webinário. A descrição estará visível no Marketo.

![](assets/image2015-5-28-15-3a1-3a36.png)

## Data e hora {#date-time}

Digite as seguintes informações para o seu webinário que será extraído para o Marketo através do adaptador. Se você fizer alterações nessas informações, clique no link &quot;**Atualizar do provedor de webinar**&quot; **Ações do evento**, para que o Marketo veja as alterações.

**Data de início** - digite a data de início. Isso estará visível no Marketo.

**Hora de início** - insira a hora de início. Isso estará visível no Marketo.

**Hora de Término** - insira a hora de término. Isso estará visível no Marketo.

**Fuso Horário** - selecione o fuso horário aplicável. Ele estará visível no Marketo.

**Tipo -** defina como **Uma sessão**.

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>No momento, a Marketo não oferece suporte a webinars recorrentes. Você deve configurar uma única sessão entre cada Evento do Marketo e o webinar do GoToWebinar.

>[!TIP]
>
>Se precisar de ajuda adicional do GoToWebinar, visite as [Site de ajuda](https://support.logmeininc.com/gotowebinar).

Agora vamos entrar no Marketo!

1. Selecione um evento. Clique em **Ações do evento** e escolha **Configurações do evento**.

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >O tipo de canal do evento selecionado deve ser **webinário**.

1. Choose **IrParaWebinar** do **Parceiro de evento** Lista.

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. Escolha a conta.

   ![](assets/rtaimage-2.png)

1. Selecione o webinário.

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. Clique em **Salvar**.

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. Excelente! Agora, o evento é sincronizado e agendado por **IrParaWebinar**.

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   >
   >Os campos que o Marketo envia são: Nome, Sobrenome, Endereço De Email. Esses campos são obrigatórios e não devem estar vazios.

   >[!TIP]
   >
   >Para preencher o email de confirmação com esse URL exclusivo, use o seguinte token no email: `{{member.webinar url}}`. Quando o URL de confirmação é enviado, esse token é automaticamente resolvido para o URL de confirmação exclusivo da pessoa.
   >
   >Defina seu email de confirmação para **Operacional** para garantir que as pessoas que se registram e podem ser canceladas ainda recebam as informações de confirmação.

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >Evite usar programas de email aninhados para enviar seus emails de confirmação. Em vez disso, use a campanha inteligente do programa de eventos, conforme mostrado acima.

   >[!TIP]
   >
   >Pode levar até 48 horas para que os dados apareçam no Marketo. Se, depois de esperar tanto tempo que você ainda não vir nada, selecione **Atualizar do provedor de webinar** no menu Ações do evento na **Resumo** do seu evento.

As pessoas que se inscreverem no seu webinário serão encaminhadas para o seu provedor de webinário por meio da etapa de fluxo Alterar status do programa , quando o Novo status for definido como &quot;Registrado&quot;. Nenhum outro status empurrará a pessoa. Além disso, certifique-se de fazer a etapa 1 do fluxo Alterar status do programa e Enviar fluxo de email etapa 2.

## Exibindo a Programação  {#viewing-the-schedule}

Na exibição do agendamento do programa, clique na entrada do calendário do seu evento. Você pode ver o cronograma no lado direito da tela.

>[!NOTE]
>
>Para alterar seu agendamento de evento, você precisará editar o webinar em GoToWebinar.

![](assets/image2015-5-14-15-3a3-3a13.png)
