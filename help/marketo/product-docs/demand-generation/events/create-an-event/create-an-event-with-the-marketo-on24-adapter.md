---
unique-page-id: 10096656
description: Crie um Evento com o adaptador Marketo ON24 - Documentos do Marketing Cloud - Documentação do produto
title: Crie um Evento com o adaptador Marketo ON24
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---


# Crie um Evento com o adaptador Marketo ON24 {#create-an-event-with-the-marketo-on-adapter}

## Antes de começar {#before-you-begin}

Familiarize-se com os blocos componentes e a sequência recomendada para a criação de Eventos no Marketo. Você também deve ter conhecimento prático dos seguintes conceitos de marketing:

* [Os ](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md) programas de marketing, bem como os Eventos, e as diferenças entre eles
* [Canais](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)
* [Ativos locais](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md)
* [Campanhas secundárias ](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md) e status  [do Programa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)

>[!NOTE]
>
>Consulte a [documentação da API de marketing](https://developers.marketo.com/documentation/rest/) para obter mais informações sobre as APIs de marketing.

## Pré-requisitos {#prerequisites}

Os seguintes itens são necessários para usar a integração com o Marketing ON24:

* **Subscrição em webcasts**  ON24 - Se você não tiver uma subscrição atual, entre em contato diretamente com a ON24. **NOTA**: ON24 Hosted Edition é necessário. Não é necessário o gerenciamento de Eventos ON24.

* **Direitos de administrador para ON24**  - será necessário usar esse conector e criar convidados no sistema ON24.
* **Credenciais**  de conexão ON24 - É necessário inserir essas informações no Marketo para habilitar a integração: Nome de usuário, Senha, ID do cliente e Chave do cliente. Entre em contato com seu gerente de conta ON24 ou com o suporte ON24 se precisar de ajuda com suas credenciais.
* **Formulário**  de registro - Use um formulário Marketo ou um formulário não Marketo junto com a API adequada para garantir que os dados de registro e as informações do registrante sejam passados para o Marketo.
* **Campanha**  filho do registro - Uma campanha filho do registro no Evento do Marketing deve ser criada e configurada corretamente para que a integração do Parceiro do Evento funcione.

## Fluxo de Processo {#process-flow}

Siga estas etapas para criar um Evento com o adaptador Marketo On24:

1. [Insira suas credenciais ON24 no Marketo](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/enter-your-on24-credentials-in-marketo.md)
1. [Criar seu Evento de Webinar no ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md)
1. [Configure as configurações do Evento e sincronize o marketing com seu webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md)
1. [Criar Campanhas secundárias e ativos locais](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md)
1. [Teste sua integração de Evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)
1. [Exemplo de integração de Evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
1. [Entendendo os status dos Programas do webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)
1. [Atualizações de registro do Evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md)
