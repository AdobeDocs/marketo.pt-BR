---
unique-page-id: 10096656
description: Crie um evento com o adaptador Marketo ON24 - Documentos Marketo - Documentação do produto
title: Crie um evento com o adaptador Marketo ON24
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
source-git-commit: 0c6c119f5be6e2ac3db7d99f7e8623d8aaa3555c
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Crie um evento com o adaptador Marketo ON24 {#create-an-event-with-the-marketo-on-adapter}

Familiarize-se com os blocos de construção e a sequência recomendada para criar Eventos no Marketo. Você também deve ter conhecimento prático dos seguintes conceitos do Marketo:

* [Programas do Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target=&quot;_blank&quot;}, bem como Eventos, e as diferenças entre eles
* [Canais](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target=&quot;_blank&quot;}
* [Ativos locais](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target=&quot;_blank&quot;}
* [Campanhas filhas](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target=&quot;_blank&quot;} e [Status do programa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target=&quot;_blank&quot;}

>[!NOTE]
>
>Consulte a [Documentação da API do Marketo](https://developers.marketo.com/documentation/rest/){target=&quot;_blank&quot;} para obter mais informações sobre APIs do Marketo.

## Pré-requisitos {#prerequisites}

Os seguintes itens são necessários para usar a integração do Marketo ON24:

* **Assinatura de webcasts ON24** - Se você não tiver uma assinatura atual, entre em contato diretamente com o ON24. **OBSERVAÇÃO**: A ON24 Hosted Edition é necessária. Não é necessário o ON24 Event Management.

* **Direitos de administrador para ON24** - Você precisará disso para usar esse conector e criar convidados no sistema ON24.
* **Credenciais de ligação ON24** - É necessário inserir essas informações no Marketo para habilitar a integração: Nome de usuário, senha, ID do cliente e chave do cliente. Entre em contato com o Gerente de Conta ON24 ou com o Suporte ON24 se precisar de ajuda com suas credenciais.
* **Formulário de registro** - Use um formulário Marketo ou um formulário não Marketo junto com a API adequada para garantir que os dados de registro e as informações do registrando sejam passadas para o Marketo.
* **Campanha filho de registro** - Uma campanha filho de registro no Evento do Marketo deve ser criada e configurada corretamente para que a integração do Parceiro de evento funcione.

## Fluxo do processo {#process-flow}

Siga estas etapas para criar um evento com o adaptador Marketo On24:

1. [Criar seu evento de webinar no ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target=&quot;_blank&quot;}
1. [Configurar configurações do evento e sincronizar o Marketo com seu webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target=&quot;_blank&quot;}
1. [Criar campanhas filhas e ativos locais](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target=&quot;_blank&quot;}
1. [Teste sua integração de evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target=&quot;_blank&quot;}
1. [Exemplo de integração de evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target=&quot;_blank&quot;}
1. [Noções básicas sobre os status do programa do webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target=&quot;_blank&quot;}
1. [Atualizações do registro de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target=&quot;_blank&quot;}
