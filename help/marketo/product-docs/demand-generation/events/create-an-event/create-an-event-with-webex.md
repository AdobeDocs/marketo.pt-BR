---
unique-page-id: 2949863
description: Criar um evento com o WebEx - Documentos do Marketo - Documentação do produto
title: Criar um evento com WebEx
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
source-git-commit: ed9146f48aecd34025d61abf14d76a714726dcc9
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# Criar um evento com WebEx {#create-an-event-with-webex}

>[!PREREQUISITES]
>
>* [Adicionar WebEx como um Serviço do LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Criar um novo programa de evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Defina as [ações de fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) para rastrear o envolvimento
>* Verifique se você está usando Eventos do Webex (clássico)


Primeiro crie um Evento Webex no WebEx Event Center. O Marketo usa apenas configurações e campos específicos para sua integração, que passaremos em breve. Outros campos que você pode querer configurar para WebEx são explicados na variável [Guia do usuário do WebEx Event Center](https://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf).

>[!IMPORTANT]
>
>O Marketo Engage suporta apenas eventos criados em Eventos Webex (clássico). O Marketo não é compatível com eventos criados nos Eventos do Webex (novos) no momento.

## Informações básicas {#basic-information}

* **Nome do evento -** Esse nome estará visível no Marketo.
* **Caixa de seleção não listada**

   * Recomenda-se que você faça **not** listar seu evento. Isso garantirá que todas as pessoas se registrem por meio da página de aterrissagem do Marketo. As pessoas que se registrarem por meio de um mecanismo diferente do Marketo serão exibidas no Marketo depois que o evento for concluído E somente se participarem do evento.
   * Se você optar por listar o evento, ele aparecerá na página Lista de eventos para qualquer pessoa que visitar o site do Centro de eventos.

* **Registro -** Marque essa caixa para definir como &quot;obrigatório&quot;. Você usará um formulário/landing page do Marketo para capturar informações de registro que serão enviadas para o WebEx.
* **Senha do evento**- (opcional) Se você usar esse campo, certifique-se de incluí-lo no email de confirmação!

![](assets/image2015-5-28-13-3a30-3a55.png)

## Data e hora {#date-time}

* **Data de início** - Insira a data de início. Isso estará visível no Marketo.

* **Hora de início** - Insira a hora de início. Isso estará visível no Marketo.

* **Duração estimada** - Especifique a duração do evento. Isso estará visível no Marketo.

* **Fusos horários** - Insira os fusos horários aplicáveis. Eles estarão visíveis no Marketo.

![](assets/image2015-5-28-13-3a37-3a39.png)

## Configurações de conferência de áudio {#audio-conference-settings}

Essas configurações residem somente no WebEx. Eles não são usados pelo ou visualizáveis no Marketo, mas podem ser importantes para seu webinário, portanto, verifique-os duas vezes!

## Descrição e opções do evento  {#event-description-options}

As opções a seguir são usadas ou visualizadas no Marketo. Outros campos residem somente em WebEx.

* **Descrição** - Insira uma descrição. Isso será visível, mas não modificável no Marketo.
* **Pesquisa pós-evento** - O Marketo não pode capturar as informações em uma pesquisa pós-evento do WebEx no momento.
* **URL de destino** - (opcional) Você pode inserir o URL de uma página de aterrissagem do Marketo para servir como URL de destino a ser exibido depois que a sessão terminar.

![](assets/image2015-5-28-13-3a48-3a49.png)

## Participantes e registro {#attendees-registration}

Você estará controlando a lista de convites, o formulário de registro e outros emails usando um Evento do Marketo. Outras funcionalidades não serão suportadas pela Marketo, incluindo:

* **Número máximo de registantes** - Atualmente **not** compatível com o uso da integração Marketo-WebEx.  A aprovação manual de registrantes está disponível usando o status de progressão de Aprovação pendente no Marketo.

* **ID de registro obrigatório** - Atualmente compatível com o uso da integração Marketo-WebEx. Você pode usar o Marketo para enviar o email de confirmação para o evento. Quando a pessoa se registra, ela recebe um URL exclusivo que usa para inserir o evento.

   >[!TIP]
   >
   >Para preencher o email de confirmação com esse URL exclusivo, use o seguinte token no email: `{{member.webinar url}}`. Quando o URL de confirmação é enviado, esse token é automaticamente resolvido para o URL de confirmação exclusivo da pessoa.
   >
   >Defina seu email de confirmação para **Operacional** para garantir que as pessoas que se registram e podem ser canceladas ainda recebam as informações de confirmação.

* **Senha de registro** - (Opcional) No momento, não há suporte para o uso da integração Marketo-WebEx.
* **Regras de aprovação** - No momento, não há suporte para o uso da integração Marketo-WebEx. No entanto, você pode usar campanhas inteligentes no Marketo para controlar aprovações.

![](assets/image2015-5-28-14-3a4-3a41.png)

### Apresentadores e Painéis {#presenters-panelists}

As informações configuradas nesta seção não são passadas para o Marketo.

### Mensagens de email {#email-messages}

Você usará o Marketo para enviar emails para seus registrantes, emails de confirmação etc. Não é necessário configurar nada nesta seção. Desative (desmarque) as opções de mensagem de email no WebEx.

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>A integração Marketo-WebEx não pode suportar o envio de emails de confirmação de WebEx. A confirmação deve ser enviada via Marketo. Depois de programar o evento, copie as informações do evento para o email de confirmação do Marketo e defina o email como **Operacional**.

Agora estamos prontos para entrar no Marketo!

1. Selecione o evento que você criou. Abra o **Ações do evento** lista suspensa. Choose **Configurações do evento.**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >O tipo de canal do evento selecionado deve ser **webinário**.

1. Em **Parceiro de evento**, selecione **WebEx**.

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. Em **Logon**, escolha seu login do WebEx.

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. Em **Evento**, escolha o evento WebEx recém-criado. Em seguida, selecione uma Página de backup opcional e clique em **Salvar**.

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. Selecione uma Página de Backup opcional para seu evento WebEx. Escolha na lista suspensa de páginas de aterrissagem aprovadas do Marketo ou insira o URL de uma página de aterrissagem que não seja da Marketo.

   >[!TIP]
   >
   >Defina uma Página de backup para direcionar um membro a uma página específica se ele clicar no URL do evento personalizado antes da hora de início do evento.

   >[!NOTE]
   >
   >Os campos que o Marketo envia são: Nome, Sobrenome, Endereço De Email.

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >Evite usar programas de email aninhados para enviar seus emails de confirmação. Em vez disso, use a campanha inteligente do programa de eventos, conforme mostrado acima.

   >[!TIP]
   >
   >Pode levar até 48 horas para que os dados apareçam no Marketo. Se, depois de esperar tanto tempo que você ainda não vir nada, selecione **Atualizar do provedor de webinar** no menu Ações do evento na **Resumo** do seu evento.

Doce! O evento WebEx agora é sincronizado com o evento do Marketo.  As pessoas que se inscreverem no seu webinário serão encaminhadas para o seu provedor de webinário por meio da etapa de fluxo Alterar status do programa , quando o Novo status for definido como &quot;Registrado&quot;. Nenhum outro status empurrará a pessoa. Além disso, certifique-se de fazer a etapa 1 do fluxo Alterar status do programa e Enviar fluxo de email etapa 2.

## Exibindo a Programação  {#viewing-the-schedule}

Na exibição do agendamento do programa, clique na entrada do calendário do seu evento. Você pode ver o cronograma no lado direito da tela!

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>Para alterar seu agendamento de evento, você precisará editar o webinar no WebEx.
