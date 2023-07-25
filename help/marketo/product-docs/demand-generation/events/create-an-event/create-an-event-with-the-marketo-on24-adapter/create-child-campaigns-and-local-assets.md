---
unique-page-id: 10096675
description: Criar campanhas secundárias e ativos locais - Documentação do Marketo - Documentação do produto
title: Criar campanhas secundárias e ativos locais
exl-id: 272105e1-43d6-455c-a533-aae65e859384
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 1%

---

# Criar campanhas secundárias e ativos locais {#create-child-campaigns-and-local-assets}

Crie campanhas filho e ativos locais usando o Design Studio.

## Página de aterrissagem e formulário {#landing-page-and-form}

Para garantir que as pessoas sejam registradas corretamente no ON24, os seguintes campos devem ser incluídos no formulário do Marketo:

* Nome
* Sobrenome
* Endereço de email

Você também pode enviar os seguintes campos para ON24:

* Nome da empresa
* Nome do cargo

Com a etapa de fluxo adequada adicionada à campanha de registro, as pessoas serão encaminhadas para o ON24 e marcadas como registradas. Você pode adicionar outros campos ao formulário e as informações serão capturadas no Marketo como parte do registro de detalhes da pessoa.

>[!CAUTION]
>
>Para uma integração bem-sucedida, você deve usar um formulário do Marketo para registrar seus funcionários para o Evento ou um formulário que não seja do Marketo com a integração de API adequada para enviar dados de registro para o Marketo.

## Emails e tokens de URL {#emails-and-url-tokens}

Crie o convite, a confirmação, o acompanhamento e agradeça os emails usando o Marketo.

## E-mail de confirmação do Marketo e token de URL {#marketo-confirmation-email-and-url-token}

Use o Marketo para enviar o email de confirmação do evento. Quando uma pessoa se registra, ela recebe um URL exclusivo para usar para inserir o evento.

>[!NOTE]
>
>Para preencher o email de confirmação com esse URL exclusivo, use o seguinte token no email: `{{member.webinar url}}`. Ao enviar o URL de confirmação, esse token é resolvido automaticamente para o URL de confirmação exclusivo da pessoa.
>
>Defina o tipo do email de confirmação como **Operacional** para garantir que as pessoas que se registram recebam suas informações de confirmação, mesmo que tenham cancelado a inscrição.

>[!TIP]
>
>Você pode configurar o ON24 para enviar emails de confirmação, lembrete ou acompanhamento. Consulte a [Site de Ajuda ON24](https://www.on24.com/live-webcast-elite/){target="_blank"} para obter mais informações.

## Requisitos de Campanha Secundária de Registro {#registration-child-campaign-requirements}

Os eventos contêm uma ou mais campanhas filho que trabalham juntas para mover as pessoas pelos status do programa e permitem acompanhar o desempenho do evento.

Exemplos de campanhas filho são uma campanha por convite, uma campanha de registro e campanhas de acompanhamento.

>[!CAUTION]
>
>Para que o adaptador faça seu trabalho, VOCÊ DEVE criar uma campanha de registro. Essa campanha deve ser acionada pela pessoa que preenche um formulário e a primeira etapa deve alterar o status do programa da pessoa para **Registrado**. A campanha envia um email de confirmação. Consulte o restante deste artigo para obter detalhes.

**Registro/Confirmação (Acionar Campanha)**

* Lista inteligente
* Acionar com base em **Preenche o formulário**. Certifique-se de incluir a página de aterrissagem em que o formulário está usando **Adicionar Restrição**, especialmente se o mesmo formulário for usado em várias landings pages.

>[!CAUTION]
>
>Você deve usar um formulário do Marketo para registrar seus funcionários para o evento ou um formulário que não seja do Marketo com a integração de API adequada para enviar dados de registro para o Marketo. Isso é essencial para o sucesso da integração do parceiro de eventos.

>[!NOTE]
>
>Se você estiver usando um formulário do Marketo em uma página de aterrissagem que não seja da Marketo, seu acionador será **Preenche o formulário** com o Nome do formulário.

![](assets/image2015-12-22-15-3a20-3a51.png)

**Fluxo**

* **Alterar status do programa** - Defina como Webinar -> Registrado.

Essa etapa do fluxo é necessária como a PRIMEIRA ETAPA DO FLUXO ao configurar sua campanha filho. Quando o status do programa de uma pessoa muda para Registrado, o Marketo envia as informações de registro para ON24. Nenhum outro status enviará a pessoa.

* **Enviar e-mail** - Email de confirmação. Definir este email como **Operacional** para que as pessoas que cancelaram a inscrição e que se registraram ainda recebam.

A variável **Enviar e-mail** a etapa do fluxo DEVE ser a segunda etapa. O email de confirmação contém a `{{member.webinar url}}`, que é preenchida com informações enviadas de volta para o Marketo a partir do ON24.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>A ordem dessas etapas de fluxo é importante devido à ordem em que as ações são executadas no Marketo. A variável **Alterar status do programa** A etapa envia a pessoa para ON24 para se registrar e um URL exclusivo é gerado. Depois que isso ocorrer, você poderá enviar o email de confirmação que inclui esse URL exclusivo usando o `{{member.webinar URL}}` token.
>
>Se a pessoa retornar com um erro de registro, ela não receberá o email de confirmação.

O próximo passo é [testar a integração do evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Noções básicas sobre os eventos do adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
>* [Exemplo de integração de evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Noções básicas sobre os status do programa de webinário](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
