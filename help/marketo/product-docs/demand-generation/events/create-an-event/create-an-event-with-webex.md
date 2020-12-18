---
unique-page-id: 2949863
description: Criar um Evento com WebEx - Documentos do Marketing - Documentação do produto
title: Criar um Evento com WebEx
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '940'
ht-degree: 0%

---


# Criar um Evento com WebEx {#create-an-event-with-webex}

>[!PREREQUISITES]
>
>* [Adicionar WebEx como um Serviço LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Criar um novo Programa de Evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Defina as [ações de fluxo](http://docs.marketo.com/display/DOCS/Flow+Actions)apropriadas para rastrear o envolvimento


Primeiro, crie um Evento Webex no Centro de Eventos WebEx. O Marketo usa apenas configurações e campos específicos para a sua integração, que passaremos em breve. Outros campos que podem ser configurados para WebEx são explicados no [Guia do Usuário do Centro de Eventos WebEx](http://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf).

## Informações básicas {#basic-information}

* **Nome do evento -** Esse nome será exibido no Marketo.
* **Caixa de seleção não listada**

   * Recomenda-se que você **e não** lista seu evento. Isso garantirá que todas as pessoas se registrem por meio da sua landing page de marketing. As pessoas que se registrarem através de um mecanismo diferente de Marketo serão exibidas no Marketo após a conclusão do evento E somente se tiverem participado do evento.
   * Se você optar por lista do evento, ele será exibido na página Lista dos Eventos para qualquer pessoa que visitar seu site da Central de Eventos.

* **Registro -** Marque esta caixa para definir como &quot;obrigatório&quot;. Você usará um formulário/landing page de marketing para capturar informações de registro que serão enviadas para WebEx.
* **Senha** do evento - (opcional) Se você usar esse campo, certifique-se de incluí-lo no seu email de confirmação!

![](assets/image2015-5-28-13-3a30-3a55.png)

## Data e hora {#date-time}

* **Data**  do start - Informe a data do start. Isso será visível em Marketo.

* **Hora**  do start - insira a hora do start. Isso será visível em Marketo.

* **Duração**  estimada - Especifique a duração do evento. Isso será visível em Marketo.

* **Fusos horários**  - Informe os fusos horários aplicáveis. Eles serão visíveis em Marketo.

![](assets/image2015-5-28-13-3a37-3a39.png)

## Configurações de conferência de áudio {#audio-conference-settings}

Essas configurações residem apenas no WebEx. Eles não são usados por nem visualizáveis no Marketo, mas podem ser importantes para o seu webinar, então verifique-os com duplo!

## Descrição e opções do evento {#event-description-options}

As opções a seguir são usadas ou visualizadas no Marketo. Outros campos residem apenas em WebEx.

* **Descrição**  - Informe uma descrição. Isso será visível, mas não modificável no Marketing.
* **Pesquisa**  pós-evento - o Marketo não pode capturar as informações em uma pesquisa pós-evento do WebEx no momento.
* **URL**  de destino - (opcional) você pode inserir o URL de uma landing page de marketing para servir como o URL de destino a ser exibido após o término da sessão.

![](assets/image2015-5-28-13-3a48-3a49.png)

## Participantes e registro {#attendees-registration}

Você estará controlando a lista do convite, o formulário de inscrição e outros emails usando um Evento de marketing. Outra funcionalidade não será suportada pelo Marketo, incluindo:

* **Número máximo de registrantes**  - atualmente  **** sem suporte usando a integração de Marketo-WebEx.  A aprovação manual dos registrantes está disponível usando o status de progressão de Aprovação pendente no Marketo.

* **ID de registro obrigatório**  - atualmente compatível com a integração com o Marketo-WebEx. Você pode usar o Marketo para enviar o e-mail de confirmação para o seu evento. Quando a pessoa se registra, ela recebe um URL exclusivo que usa para inserir o evento.

   >[!TIP]
   >
   >Para preencher seu email de confirmação com este URL exclusivo, use o seguinte token no email: `{{member.webinar url}}`. Quando o URL de confirmação é enviado, esse token resolve automaticamente o URL de confirmação exclusivo da pessoa.
   >
   >Defina seu e-mail de confirmação como **Operacional** para garantir que as pessoas que se registram e podem ser canceladas ainda recebam suas informações de confirmação.

* **Senha**  de registro - (Opcional) Atualmente não é compatível com o uso da integração com Marketo-WebEx.
* **Regras**  de aprovação - Atualmente não é compatível com o uso da integração de Marketing-WebEx. No entanto, você pode usar campanhas inteligentes no Marketo para controlar as aprovações.

![](assets/image2015-5-28-14-3a4-3a41.png)

### Apresentadores e Painéis {#presenters-panelists}

As informações configuradas nesta seção não são passadas para o Marketo.

### Mensagens de email {#email-messages}

Você usará o Marketo para enviar emails aos seus inscritos, emails de confirmação, etc. Não é necessário configurar nada nesta seção. Desative (desmarque) as opções de mensagem de email no WebEx.

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>A integração com o Marketo-WebEx não suporta o envio de e-mails de confirmação para fora do WebEx. A confirmação deve ser enviada via Marketo. Depois de programar o evento, copie as informações do evento para o e-mail de confirmação do Marketo e defina o e-mail como **Operacional**.

Agora estamos prontos para pular para Marketo!

1. Selecione o evento que você criou. Abra o menu suspenso **Ações do Evento**. Escolha **Configurações do Evento.**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >O tipo de canal do evento selecionado deve ser **webinar**.

1. Em **Parceiro de Evento**, selecione **WebEx**.

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. Em **Logon**, escolha seu login WebEx.

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. Em **Evento**, escolha seu evento WebEx recém-criado. Em seguida, selecione uma Página de backup opcional e clique em **Salvar**.

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. Selecione uma Página de Backup opcional para seu evento WebEx. Escolha na lista suspensa de landings page de marketing aprovadas ou insira o URL de uma landing page que não seja de marketing.

   >[!TIP]
   >
   >Configure uma página de backup para direcionar um membro a uma página específica se ele clicar em seu URL de evento personalizado antes da hora do start.

   >[!NOTE]
   >
   >Os campos que o Marketo envia são: Nome, Sobrenome, Endereço de email.

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >Evite usar programas de e-mail aninhados para enviar seus e-mails de confirmação. Em vez disso, use a campanha inteligente do programa do evento, como mostrado acima.

   >[!TIP]
   >
   >Pode levar até 48 horas para que os dados apareçam no Marketo. Se, depois de aguardar tanto tempo, você ainda não vir nada, selecione **Atualizar do Provedor de Webinar** no menu Ações do Evento na guia **Resumo** do evento.

Doce! Seu evento WebEx agora é sincronizado com seu evento Marketo.  As pessoas que se inscreverem no seu webinar serão encaminhadas para o seu provedor de webinar por meio da etapa de fluxo Alterar status do Programa quando o Novo status estiver definido como &quot;Registrado&quot;. Nenhum outro status empurrará a pessoa. Além disso, certifique-se de fazer a etapa 1 do fluxo Alterar status do Programa e a etapa 2 do fluxo de Enviar e-mail.

## Exibindo o Agendamento {#viewing-the-schedule}

Na [visualização do cronograma do programa](http://docs.marketo.com/display/docs/program+schedule+view), clique na entrada do calendário do evento. Você pode ver o cronograma no lado direito da tela!

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>Para alterar o agendamento do evento, é necessário editar o webinar no WebEx.
