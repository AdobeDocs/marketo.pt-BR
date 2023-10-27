---
description: Criar um evento com o Webex - Documentação do Marketo - Documentação do produto
title: Criar um evento com o Webex
hide: true
hidefromtoc: true
feature: Events
source-git-commit: e21450610146eea3a14761a7365a35d9cacee523
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 0%

---

# Criar um evento com o Webex {#create-an-event-with-webex}

>[!PREREQUISITES]
>
>* [Adicionar o Webex como um serviço do LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Criar um novo programa de evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Defina as [ações de fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) para rastrear o envolvimento
>* Verifique se você está usando os eventos do Webex (clássicos)

Primeiro, crie um webinário no [Webex](https://www.webex.com/){target="_blank"}. Event in the Webex Event Center. Marketo only uses specific settings and fields for your integration, which we'll go through shortly. Other fields that you might want to configure for Webex are explained in the [Webex Event Center User Guide](https://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf){target="_blank"}.

>[!IMPORTANT]
>
>O Marketo Engage só é compatível com eventos criados em eventos do Webex (clássicos). No momento, o Marketo não é compatível com eventos criados no Webex Events (novo).

## Informações básicas {#basic-information}

* **Nome do evento -** Esse nome poderá ser visto no Marketo.
* **Caixa de seleção não listada**

   * Recomenda-se que você **não** listar seu evento. Isso garantirá que todas as pessoas se registrem por meio da página de aterrissagem do Marketo. As pessoas que se registrarem por meio de um mecanismo diferente do Marketo serão exibidas no Marketo após a conclusão do evento E somente se participarem do evento.
   * Se você optar por listar o evento, ele aparecerá na página Lista de eventos para qualquer pessoa que visitar o site do Centro de eventos.

* **Registro -** Marque esta caixa para definir como &quot;obrigatório&quot;. Você usará um formulário/página de aterrissagem do Marketo para capturar as informações de registro que serão enviadas para o Webex.
* **Senha do evento**- (opcional) Se você usar esse campo, certifique-se de incluí-lo no email de confirmação.

![](assets/image2015-5-28-13-3a30-3a55.png)

## Data e hora {#date-time}

* **Data inicial** - Insira a data de início. Ele poderá ser visto no Marketo.

* **Hora de início** - Insira a hora de início. Ele poderá ser visto no Marketo.

* **Duração estimada** - Especifique a duração do evento. Ele poderá ser visto no Marketo.

* **Fusos horários** - Insira os fusos horários aplicáveis. Eles poderão ser visualizados no Marketo.

![](assets/image2015-5-28-13-3a37-3a39.png)

## Configurações de Audioconferência {#audio-conference-settings}

Essas configurações residem somente no Webex. Eles não são usados ou visualizáveis no Marketo, mas podem ser importantes para o seu webinário, portanto, verifique-os novamente!

## Descrição e opções do evento  {#event-description-options}

As opções a seguir são usadas pelo ou podem ser visualizadas no Marketo. Outros campos residem somente no Webex.

* **Descrição** - Insira uma descrição. Ele será visível, mas não modificável no Marketo.
* **Pesquisa pós-evento** - No momento, o Marketo não pode capturar as informações em uma pesquisa pós-evento da Webex.
* **URL de destino** - (opcional) Você pode inserir o URL de uma página de aterrissagem do Marketo para servir como o URL de destino a ser exibido após o término da sessão.

![](assets/image2015-5-28-13-3a48-3a49.png)

## Participantes e inscrição {#attendees-registration}

Você estará controlando a lista de convites, o formulário de registro e outros emails usando um Evento do Marketo. Outras funcionalidades não serão suportadas pela Marketo, incluindo:

* **Número máximo de inscritos** - Atualmente **não** compatível com a integração Marketo-Webex.  A aprovação manual de inscritos está disponível usando o status de progressão Aprovação pendente no Marketo.

* **A ID de registro é obrigatória** - Atualmente compatível com a integração Marketo-Webex. Você pode usar o Marketo para enviar o email de confirmação do evento. Quando a pessoa se registra, ela recebe um URL exclusivo que usa para inserir o evento.

  >[!TIP]
  >
  >Para preencher o email de confirmação com esse URL exclusivo, use o seguinte token no email: `{{member.webinar url}}`. Quando o URL de confirmação é enviado, esse token é resolvido automaticamente para o URL de confirmação exclusivo da pessoa.
  >
  >Defina seu email de confirmação como **Operacional** para garantir que as pessoas que se registram e podem ter a inscrição cancelada ainda recebam suas informações de confirmação.

* **Senha de registro** - (Opcional) No momento, não compatível com a integração Marketo-Webex.
* **Regras de aprovação** - No momento, não é compatível com a integração Marketo-Webex. No entanto, você pode usar campanhas inteligentes no Marketo para controlar aprovações.

![](assets/image2015-5-28-14-3a4-3a41.png)

### Apresentadores e listas de painéis {#presenters-panelists}

As informações configuradas nesta seção não são passadas para o Marketo.

### Mensagens de email {#email-messages}

Você usará o Marketo para enviar emails para seus inscritos, emails de confirmação etc. Não é necessário configurar nada nesta seção. Desative (desmarque) as opções de mensagem de email no Webex.

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>A integração Marketo-Webex não oferece suporte ao envio de emails de confirmação do Webex. A confirmação deve ser enviada via Marketo. Depois de programar o evento, copie as informações do evento no email de confirmação do Marketo e defina o email como **Operacional**.

Agora estamos prontos para entrar no Marketo!

1. Selecione o evento criado. Abra o **Ações de evento** menu suspenso. Escolher **Configurações do evento.**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >O tipo de canal do evento selecionado deve ser **webinário**.

1. Em **Parceiro de evento**, selecione **Webex**.

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. Em **Logon**, escolha seu logon no Webex.

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. Em **Evento**, escolha o evento Webex recém-criado. Em seguida, selecione uma página de backup opcional e clique em **Salvar**.

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. Selecione uma página de backup opcional para seu evento Webex. Escolha a partir do menu suspenso de páginas de aterrissagem aprovadas do Marketo ou insira o URL de uma página de aterrissagem que não seja da Marketo.

   >[!TIP]
   >
   >Defina uma Página de Backup para direcionar um membro para uma página específica se ele clicar no URL do evento personalizado antes da hora de início do evento.

   >[!NOTE]
   >
   >Os campos que o Marketo envia são: Nome, Sobrenome, Endereço de email.

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >Evite usar programas de email aninhados para enviar emails de confirmação. Em vez disso, use a campanha inteligente do programa do evento, como mostrado acima.

   >[!TIP]
   >
   >Pode levar até 48 horas para que os dados sejam exibidos no Marketo. Se, após esse tempo de espera, você ainda não visualizar nada, selecione **Atualizar do provedor do webinário** no menu Ações de evento na caixa de diálogo **Resumo** do evento.

Doce! Seu evento Webex agora está sincronizado com seu evento do Marketo. As pessoas que se inscreverem no webinário serão encaminhadas ao provedor do webinário por meio da etapa de fluxo Alterar status do programa quando o Novo status for definido como &quot;Registrado&quot;. Nenhum outro status enviará a pessoa. Além disso, certifique-se de marcar a etapa de fluxo Alterar status do programa #1 e a etapa de fluxo Enviar email #2.

## Exibição do Agendamento  {#viewing-the-schedule}

Na exibição de cronograma do programa, clique na entrada de calendário do evento. Você pode ver o cronograma no lado direito da tela!

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>Para alterar a programação do evento, será necessário editar o webinário no Webex.
