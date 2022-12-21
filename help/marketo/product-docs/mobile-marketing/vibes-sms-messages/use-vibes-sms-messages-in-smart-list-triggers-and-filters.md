---
unique-page-id: 11378871
description: Usar mensagens SMS Vibes em acionadores e filtros de Smart List - Documentos do Marketo - Documentação do produto
title: Usar mensagens SMS de Vibes em Triggers e Filtros da Smart List
exl-id: 9a629a39-fddc-4ec5-b1c5-d5053d676594
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Usar mensagens SMS de Vibes em Triggers e Filtros da Smart List {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Depois de [criar uma mensagem SMS do Vibes](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md), você deve usar acionadores e filtros de listas inteligentes em uma campanha inteligente para obter os benefícios. Veja como.

1. Em Minha Marketo, clique em **Atividades de marketing**.

   ![](assets/image2016-7-28-9-3a48-3a32.png)

1. Escolha uma campanha inteligente na qual deseja usar seu ativo SMS. Arraste sobre um acionador, como o **Preenche Formulário**.

   ![](assets/fills-out-form-pull-over.jpg)

## Triggers de SMS {#sms-triggers}

Há outros acionadores de SMS disponíveis. Os acionadores de SMS aparecem somente se o serviço Vibes estiver ativado.

![](assets/new-sms-search2.png)

Veja alguns exemplos:

O acionador de Rejeições da mensagem SMS inicia um fluxo, como o envio de um email, quando uma mensagem SMS é rejeitada.

![](assets/sms-message-bounces-real.jpg)

O **Subscreve a Lista de Vibes** trigger inicia um fluxo quando uma pessoa se inscreve.

![](assets/subscribes-to-vibes-list-real.jpg)

O **Link de cliques na mensagem SMS** trigger inicia um fluxo quando uma pessoa clica em um link na mensagem SMS.

![](assets/clicks-link-in-sms-message.jpg)

## Filtros de SMS {#sms-filters}

Também é possível usar filtros Vibes em listas inteligentes. O **Inscrito na Lista de Vibes** o filtro encontra qualquer pessoa que tenha *ever* subscritos no Vibes. Isso inclui pessoas canceladas e excluídas, mesmo que as pessoas excluídas sejam omitidas do fluxo. Esse filtro é mais adequado para relatórios.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

Por outro lado, a variável **Membro da Lista de Víbios** filter found _any_ Atualmente, está inscrito no Vibes e é mais adequado para uso em campanhas ou listas inteligentes.

![](assets/image001.png)

>[!NOTE]
>
>Todos os filtros de SMS incluem o **Data da atividade** restrição por padrão.

Depois de configurar os acionadores e filtros do Vibes na sua lista inteligente, você pode [definir o fluxo](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Definir Smart List para Smart Campaign | Acionador](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Localizar e adicionar filtros a uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)

