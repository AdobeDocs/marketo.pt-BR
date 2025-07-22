---
unique-page-id: 10096675
description: Criar campanhas secundárias e Assets local — Documentação do Marketo — Documentação do produto
title: Criar campanhas secundárias e Assets local
exl-id: 272105e1-43d6-455c-a533-aae65e859384
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 1%

---

# Criar campanhas secundárias e Assets local {#create-child-campaigns-and-local-assets}

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
>Para popular seu email de confirmação com esta URL exclusiva, use o seguinte token no email: `{{member.webinar url}}`. Ao enviar o URL de confirmação, esse token é resolvido automaticamente para o URL de confirmação exclusivo da pessoa.
>
>Defina o tipo do seu email de confirmação como **Operacional** para garantir que as pessoas que se registrarem recebam suas informações de confirmação, mesmo que tenham a assinatura cancelada.

>[!TIP]
>
>Você pode configurar o ON24 para enviar emails de confirmação, lembrete ou acompanhamento. Consulte o [Site de Ajuda do ON24](https://support.on24.com/hc/en-us/categories/26127314569115-Webcast-Elite){target="_blank"} para obter mais informações.

## Requisitos de Campanha Secundária de Registro {#registration-child-campaign-requirements}

Os eventos contêm uma ou mais campanhas filho que trabalham juntas para mover as pessoas pelos status do programa e permitem acompanhar o desempenho do evento.

Exemplos de campanhas filho são uma campanha por convite, uma campanha de registro e campanhas de acompanhamento.

>[!CAUTION]
>
>Para que o adaptador faça seu trabalho, VOCÊ DEVE criar uma campanha de registro. Esta campanha deve ser acionada pela pessoa que preenche um formulário e a primeira etapa deve alterar o status do programa da pessoa para **Registrada**. A campanha envia um email de confirmação. Consulte o restante deste artigo para obter detalhes.

**Registro/Confirmação (Campanha de Gatilho)**

* Lista inteligente
* Acionar com base em **Preenche o Formulário**. Certifique-se de incluir a página de aterrissagem em que o formulário está usando **Adicionar restrição**, especialmente se o mesmo formulário for usado em várias páginas de aterrissagem.

>[!CAUTION]
>
>Você deve usar um formulário do Marketo para registrar seus funcionários para o evento ou um formulário que não seja do Marketo com a integração de API adequada para enviar dados de registro para o Marketo. Isso é essencial para o sucesso da integração do parceiro de eventos.

>[!NOTE]
>
>Se você estiver usando um formulário do Marketo em uma página de aterrissagem que não seja da Marketo, seu acionador será **[!UICONTROL Preenche o formulário]** com o [!UICONTROL Nome do formulário].

![](assets/image2015-12-22-15-3a20-3a51.png)

**Fluxo**

* **[!UICONTROL Alterar Status do Programa]** - Defina como Webinar -> Registrado.

Essa etapa do fluxo é necessária como a PRIMEIRA ETAPA DO FLUXO ao configurar sua campanha filho. Quando o status do programa de uma pessoa muda para Registrado, o Marketo envia as informações de registro para ON24. Nenhum outro status enviará a pessoa.

* **[!UICONTROL Enviar Email]** - Email de confirmação. Defina este email como **Operacional** para que as pessoas que cancelaram sua inscrição e que se registraram ainda o recebam.

A etapa de fluxo **[!UICONTROL Enviar Email]** DEVE ser a segunda etapa. O email de confirmação contém o `{{member.webinar url}}`, que é preenchido com informações enviadas de volta para o Marketo do ON24.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>A ordem dessas etapas de fluxo é importante devido à ordem em que as ações são executadas no Marketo. A etapa **[!UICONTROL Alterar Status do Programa]** envia a pessoa para ON24 para se registrar e uma URL exclusiva é gerada. Depois disso, você poderá enviar o email de confirmação que inclui essa URL exclusiva usando o token `{{member.webinar URL}}`.
>
>Se a pessoa retornar com um erro de registro, ela não receberá o email de confirmação.

A próxima etapa é [testar a integração de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Noções Básicas sobre os Eventos do Adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
>* [Exemplo de Integração de Eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Noções básicas sobre os status do programa de webinário](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
