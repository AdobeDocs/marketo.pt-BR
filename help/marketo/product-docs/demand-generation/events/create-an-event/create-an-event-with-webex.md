---
unique-page-id: 2949863
description: Criar um evento com o Webex - Documentação do Marketo - Documentação do produto
title: Criar um evento com o Webex
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
feature: Events
source-git-commit: 7edce24c2199a6a2eaa119d3ef77543bbd97999c
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 1%

---

# Criar um evento com o Webex {#create-an-event-with-webex}

Depois de criar um webinário no Webex, será necessário sincronizar o evento com o Marketo Engage.

>[!PREREQUISITES]
>
>* [Adicionar Webex como um Serviço do LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Criar um Novo Programa de Evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Definir as [ações de fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) apropriadas para rastrear o envolvimento

## Agendar Seu Webinário {#schedule-your-webinar}

Você agenda seu evento e escolhe suas configurações preferidas em [Webex](https://www.webex.com/){target="_blank"}. Somente as seguintes informações podem ser visualizadas no Marketo: nome do webinário, data e hora de início/término, fuso horário e descrição. Informações adicionais sobre os Webinars [da Webex podem ser encontradas aqui](https://help.webex.com/en-us/landing/ld-7srxjs-WebexWebinars/Webex-Webinars){target="_blank"}.

### Informações básicas {#basic-information}

![](assets/create-an-event-with-webex-1.png)

* **Tópico**: este é seu nome de evento e será exibido no Marketo.
* **Data e hora**: data de início/término, hora de início/término, duração e fuso horário estão todos visíveis no Marketo.
* **Número máximo de participantes**: o número máximo de participantes determina quais recursos Webex têm suporte.
* **Exibição de webcast para participantes**: marque esta opção para que seu webinário seja transmitido ao vivo para todos os participantes.
* **Listas de painéis**: Convide pessoas específicas para serem listas de painéis em seu webinário.
* **Agenda do webinário**: preencha esta opção se desejar fornecer contexto no convite por email enviado aos membros do painel.

### Segurança {#security}

![](assets/create-an-event-with-webex-2.png)

* **Senha do webinário**: (opcional) se você usar este campo, certifique-se de incluí-lo no email de confirmação.
* **Senha da lista de painéis**: (opcional) se você usar este campo, certifique-se de incluí-lo na sua agenda de webinários.
* **Exigir conta**: limita os participantes somente àqueles que possuem contas Webex.

### Opções de Conexão de Áudio {#audio-connection-options}

![](assets/create-an-event-with-webex-3.png)

* **Tipo de conexão de áudio**: escolha como os participantes do webinário ingressarão na parte de áudio do seu webinário.
* **Tom de entrada e saída**: selecione o som que você deseja que os usuários façam quando alguém entrar ou sair do webinário (é necessária uma conexão de áudio com o telefone).
* **Silenciar lista de painéis**: escolha as configurações desejadas para silenciar a lista de painéis.

### Opções avançadas {#advanced-options}

![](assets/create-an-event-with-webex-4.png)

* **Gravação automática**: marque essa opção para que seu webinário seja gravado automaticamente.
* **Sessão de prática**: marque essa opção para iniciar uma sessão de prática quando o webinário começar.
* **Sessões de debate**: as sessões de debate permitem que você pré-atribua membros do painel e participantes antes do início do webinário, ou permitem que eles participem durante o webinário.
* **Série de webinários**: adicionar a uma série de webinários permite que as pessoas vejam seu webinário, seja ele público ou não.
* **Registro**: exige que os participantes se registrem e recebam aprovação do host antes de participar.
* **Lembrete de email**: escolha um lembrete de email com duração de 15 minutos, antes do início do webinário, e que pode durar até dois dias.
* **Opções de webinário**: determine quais recursos estão disponíveis para os participantes do webinário.
* **Privilégios de participante**: os privilégios de participante determinam as ações disponíveis para os participantes do webinário.

>[!NOTE]
>
>A integração Marketo-Webex não oferece suporte ao envio de emails de confirmação do Webex. A confirmação deve ser enviada via Marketo. Depois de agendar o evento, copie as informações do evento no email de confirmação do Marketo e defina o email como _Operacional_.

## Sincronizar o evento com o Marketo Engage {#sync-your-event-with-marketo-engage}

1. No Marketo, localize e selecione o Programa de evento desejado. No menu suspenso **Ações de Evento**, selecione **Configurações de Evento**.

   ![](assets/create-an-event-with-webex-5.png)

   >[!NOTE]
   >
   >O tipo de canal do evento selecionado deve ser **webinário**.

1. No menu suspenso **Parceiro de Evento**, selecione **Webex Webinars**.

   ![](assets/create-an-event-with-webex-6.png)

1. No menu suspenso **Logon**, escolha seu logon no Webex.

   ![](assets/create-an-event-with-webex-7.png)

1. No menu suspenso **Evento**, escolha seu evento Webex.

   ![](assets/create-an-event-with-webex-8.png)

1. Os detalhes do webinário serão preenchidos. Clique em **Salvar**.

   ![](assets/create-an-event-with-webex-9.png)

Seu evento Webex agora está sincronizado com seu Programa de evento do Marketo. As pessoas que se inscreverem no webinário serão encaminhadas ao seu provedor de webinário através da etapa de fluxo _Alterar status do programa_ quando o novo status estiver definido como &quot;Registrado&quot;. Nenhum outro status enviará a pessoa. Certifique-se de marcar a etapa de fluxo #1 do _Alterar Status do Programa_ e a etapa de fluxo #2 do _Enviar Email_.

## Itens a Observar {#things-to-note}

* Evite usar Programas de email aninhados para enviar emails de confirmação. Em vez disso, use a Campanha inteligente do programa de evento.

* Pode levar até 48 horas para que os dados sejam exibidos no Marketo. Se, após esse tempo de espera, você ainda não vir nada, clique em **Atualizar do Provedor de Webinar** na lista suspensa **Ações de Evento**, na guia **Resumo** do seu Programa de Eventos.
