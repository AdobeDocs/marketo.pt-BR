---
unique-page-id: 17728023
description: Criar um evento com Zoom - Documentos do Marketo - Documentação do produto
title: Criar um evento com zoom
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
source-git-commit: 8b0625a7192a80986bc4295726cd13473493ddd7
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Criar um evento com zoom {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Adicionar Zoom como um Serviço do LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
* [Criar um novo programa de evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
* Defina as [ações de fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)apropriadas para rastrear o envolvimento


Primeiro crie seu webinário em Zoom. Determinadas configurações na criação do Zoom são usadas pelo Marketo e algumas são usadas apenas pelo Zoom.

Depois de criar um evento do Marketo e associar um webinário de Zoom a ele, os sistemas poderão compartilhar informações de registro e presença. Para ajudar a criar um webinário, consulte [Introdução aos webinars de Zoom](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar).

Digite as seguintes informações para o seu webinário que será extraído para o Marketo através do adaptador. Se você fizer alterações nessas informações, clique no link &quot;Atualizar do provedor de webinar&quot; em Ações de evento, para que o Marketo possa ver as alterações.

**Título e descrição**

* **Nome do webinar**  - Insira o nome do webinar. Esse nome estará visível no Marketo.

* **Descrição**  (opcional) - Insira a descrição do webinário. A descrição estará visível no Marketo.

**Data e hora**

* **Data**  de início - Insira a data de início. Isso estará visível no Marketo.

* **Hora de início**  - Insira a hora de início. Isso estará visível no Marketo.

* **Duração**  - Informe a duração. A hora de início e de término estarão disponíveis no Marketo.

* **Fuso horário**  - Selecione o fuso horário aplicável. Isso estará visível no Marketo.

* **Webinário recorrente** - mantenha a opção desmarcada.

* **Registro**  - Marque esta caixa para tornar o registro obrigatório. Você usará um formulário/landing page do Marketo para capturar informações de registro que serão enviadas para Zoom.

>[!NOTE]
No momento, a Marketo não oferece suporte a webinars recorrentes. Você deve configurar uma única sessão entre cada evento do Marketo e o webinário de Zoom.

![](assets/overview2.png)

>[!TIP]
Há campos adicionais que você configurará no Zoom que NÃO afetarão a integração. Consulte o [Zoom Webinar Help Center](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar) para obter mais informações sobre esses campos.

Agora vamos entrar no Marketo!

1. Selecione um evento. Clique em **Ações de Evento** e escolha **Configurações de Evento**.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   O tipo de canal do evento selecionado deve ser **webinar**.

1. Escolha **Zoom** na Lista **Evento** **Parceiro**.

   ![](assets/eventsettings1.png)

1. Escolha a conta Zoom à qual deseja associar o evento.

   ![](assets/selectaccount.png)

1. Selecione o webinário.

   ![](assets/selectevent.png)

1. Clique em **Salvar**.

   ![](assets/eventsettingssave.png)

   Excelente! Agora, o evento é sincronizado e agendado por Zoom.

   >[!NOTE]
   Os campos que o Marketo envia são: Nome, Sobrenome, Endereço De Email.

   >[!TIP]
   Para preencher o email de confirmação com esse URL exclusivo, use o seguinte token no email: `{{member.webinar url}}`. Quando o URL de confirmação é enviado, esse token é automaticamente resolvido para o URL de confirmação exclusivo da pessoa.
   Defina seu email de confirmação para **Operacional** para garantir que as pessoas que se registram e podem ser canceladas ainda recebam suas informações de confirmação.

   As pessoas que se inscreverem no seu webinário serão encaminhadas para o seu provedor de webinário por meio da etapa de fluxo **Alterar status do programa** quando o Novo status for definido como &quot;Registrado&quot;. Nenhum outro status empurrará a pessoa. Além disso, certifique-se de fazer a **Alterar Status do Programa** etapa de fluxo nº 1 e **Enviar Email** etapa de fluxo nº 2.

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   Evite usar programas de email aninhados para enviar seus emails de confirmação. Em vez disso, use a campanha inteligente do programa de eventos, conforme mostrado acima.

   >[!TIP]
   Pode levar até 48 horas para que os dados apareçam no Marketo. Se, depois de esperar tanto tempo que você ainda não vir nada, selecione **Refresh from Webinar Provider** no menu Event Actions na guia **Summary** do seu evento.
