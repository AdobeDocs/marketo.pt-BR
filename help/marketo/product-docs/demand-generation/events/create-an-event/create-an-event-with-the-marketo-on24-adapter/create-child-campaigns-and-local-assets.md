---
unique-page-id: 10096675
description: Criar campanhas filhas e ativos locais - Documentos do Marketo - Documentação do produto
title: Criar campanhas filhas e ativos locais
exl-id: 272105e1-43d6-455c-a533-aae65e859384
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 1%

---

# Criar campanhas filhas e ativos locais {#create-child-campaigns-and-local-assets}

Crie campanhas filho e ativos locais usando o Design Studio.

## Página de aterrissagem e formulário {#landing-page-and-form}

Para garantir que as pessoas estejam registradas corretamente com ON24, os seguintes campos devem ser incluídos em seu formulário Marketo:

* Nome
* Sobrenome
* Endereço de e-mail

Também é possível mover os seguintes campos para ON24:

* Nome da empresa
* Nome do cargo

Com a etapa de fluxo adequada adicionada à campanha de registro, as pessoas serão encaminhadas para o ON24 e marcadas como registradas. Você pode adicionar outros campos ao formulário e as informações serão capturadas no Marketo como parte do registro de detalhes da pessoa.

>[!CAUTION]
>
>Para uma integração bem-sucedida, você deve usar um formulário Marketo para registrar as pessoas do Evento ou um formulário que não seja da Marketo com a integração de API adequada para enviar dados de registro para o Marketo.

## Emails e tokens de URL {#emails-and-url-tokens}

Crie o convite, a confirmação, o acompanhamento e agradeça os emails usando o Marketo.

## Email de confirmação do Marketo e token de URL {#marketo-confirmation-email-and-url-token}

Use o Marketo para enviar o email de confirmação para o seu evento. Quando uma pessoa se registra, ela recebe uma URL exclusiva para usar a para inserir o evento.

>[!NOTE]
>
>Para preencher o email de confirmação com esse URL exclusivo, use o seguinte token no email: `{{member.webinar url}}`. Quando você envia o URL de confirmação, esse token resolve automaticamente o URL de confirmação exclusivo da pessoa.
>
>Defina o tipo do email de confirmação para **Operacional** para garantir que as pessoas que se registram recebam as informações de confirmação, mesmo que sejam canceladas.

>[!TIP]
>
>Você pode configurar o ON24 para enviar confirmação, lembrete ou emails de acompanhamento. Consulte a [Site de Ajuda do ON24](https://www.on24.com/live-webcast-elite/) para obter mais informações.

## Requisitos de Campanha Filho de Registro {#registration-child-campaign-requirements}

Os eventos contêm uma ou mais campanhas-filho que trabalham juntas para movimentar pessoas pelos status do programa e permitem rastrear o desempenho do evento.

Exemplos de campanhas-filho são uma campanha de convite, uma campanha de registro e campanhas de acompanhamento.

>[!CAUTION]
>
>Para que o adaptador faça seu trabalho, você DEVE criar uma Campanha de registro. Essa campanha deve ser acionada pela pessoa que preenche um formulário e a primeira etapa deve alterar o status do programa da pessoa para **Registrado**. A campanha envia um email de confirmação. Consulte o resto deste artigo para obter detalhes.

**Registro/Confirmação (Campanha do Acionador)**

* Lista inteligente
* Acionar com base em **Preenche Formulário**. Certifique-se de incluir a landing page na qual o formulário reside usando **Adicionar restrição**, especialmente se o mesmo formulário for usado em várias landing pages.

>[!CAUTION]
>
>Você deve usar um formulário Marketo para registrar suas pessoas no evento ou um formulário que não seja da Marketo com a integração de API adequada para enviar dados de registro para o Marketo. Isso é essencial para o sucesso da integração do parceiro de eventos.

>[!NOTE]
>
>Se você estiver usando um formulário Marketo em uma página de aterrissagem que não seja a Marketo, o acionador será **Preenche o Formulário** com o Nome do formulário.

![](assets/image2015-12-22-15-3a20-3a51.png)

**Fluxo**

* **Alterar status do programa** - Defina como Webinar -> Registrado.

Esta etapa do fluxo é necessária como a PRIMEIRA ETAPA DO FLUXO ao configurar sua campanha filho. Quando o status do programa de uma pessoa muda para Registrado, o Marketo envia as informações de registro para ON24. Nenhum outro status empurrará a pessoa.

* **Enviar Email** - Email de confirmação. Defina este email como **Operacional** para que as pessoas que se inscreveram ainda o recebam.

O **Enviar Email** a etapa de fluxo DEVE ser a segunda etapa. O email de confirmação contém a variável `{{member.webinar url}}`, que é preenchida com informações enviadas de volta ao Marketo a partir de ON24.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>A ordem dessas etapas do fluxo é importante por causa da ordem em que as ações são executadas no Marketo. O **Alterar status do programa** Esta etapa envia a pessoa para o ON24 para se registrar e um URL único é gerado. Depois que isso ocorrer, você poderá enviar o email de confirmação que inclui esse URL exclusivo usando o `{{member.webinar URL}}` token.
>
>Se a pessoa for retornada com um erro de registro, ela não receberá a confirmação do email.

O próximo passo é [teste sua integração de evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md).

>[!MORELIKETHIS]
>
>* [Noções básicas sobre os eventos do adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
>* [Exemplo de integração de evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [Noções básicas sobre os status do programa do webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)

