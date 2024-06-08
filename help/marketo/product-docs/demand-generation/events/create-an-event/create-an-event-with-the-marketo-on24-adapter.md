---
unique-page-id: 10096656
description: Crie um evento com o adaptador Marketo ON24 - Documentação do Marketo - Documentação do produto
title: Crie um evento com o adaptador Marketo ON24
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
feature: Events
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Crie um evento com o adaptador Marketo ON24 {#create-an-event-with-the-marketo-on-adapter}

Familiarize-se com os blocos de construção e a sequência recomendada para criar eventos no Marketo. Você também deve ter conhecimento prático dos seguintes conceitos do Marketo:

* [Programas do Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"} bem como Eventos, e as diferenças entre eles
* [Canais](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}
* [Ativos locais](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target="_blank"}
* [Campanhas secundárias](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"} e [Status do programa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}

>[!NOTE]
>
>Consulte a [Documentação da API do Marketo](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} para obter mais informações sobre as APIs do Marketo.

## Pré-requisitos {#prerequisites}

Para usar a integração do Marketo ON24, é necessário:

* **Assinatura de webcasts ON24** - Se você não tiver uma assinatura atual, contate a ON24 diretamente. **NOTA**: A Edição hospedada ON24 é necessária. O Gerenciamento de Eventos ON24 não é necessário.

* **Direitos de administrador para ON24** - Você precisará disso para usar esse conector e criar convidados no sistema ON24.
* **Credenciais de conexão ON24** - Você precisará inserir essas informações no Marketo para habilitar a integração: Nome de usuário, Senha, ID do cliente e Chave do cliente. Entre em contato com o Gerente de conta do ON24 ou com o Suporte do ON24 se precisar de ajuda com suas credenciais.
* **Formulário de registro** : use um formulário do Marketo ou um formulário que não seja da Marketo, juntamente com a API apropriada, para garantir que os dados de registro e as informações do inscrito sejam passados para a Marketo.
* **Campanha filho de registro** - Uma campanha filho de registro no Evento do Marketo deve ser criada e configurada corretamente para que a integração do Parceiro de evento funcione.

## Fluxo do processo {#process-flow}

Siga estas etapas para criar um Evento com o Adaptador Marketo On24:

1. [Criar seu evento de webinário no ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target="_blank"}
1. [Definir configurações de evento e sincronizar o Marketo com seu webinário](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"}
1. [Criar campanhas secundárias e ativos locais](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target="_blank"}
1. [Teste a integração do evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}
1. [Exemplo de integração de evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
1. [Noções básicas sobre os status do programa de webinário](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
1. [Atualizações de registro de evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}
