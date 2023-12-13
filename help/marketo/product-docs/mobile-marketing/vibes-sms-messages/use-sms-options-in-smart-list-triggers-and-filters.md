---
description: Usar opções de SMS em Acionadores e filtros de Smart List - Documentação do Marketo - Documentação do produto
title: Usar opções de SMS em Acionadores e Filtros de Smart List
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 8e56b571a34451d6b0436dc041efaf0fd575db36
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Usar opções de SMS em Acionadores e Filtros de Smart List {#use-sms-options-in-smart-list-triggers-and-filters}

NOVO DOCUMENTO

Depois que você [criar uma mensagem SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}, você deverá usar os acionadores e filtros de Smart List em uma Campanha inteligente para obter os benefícios.

>[!PREREQUISITES]
>
>Os acionadores/filtros de SMS só aparecerão se a variável [O serviço Vibes foi ativado](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md).

## Acionadores de SMS {#sms-triggers}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-1.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-2.png"></td>
  </tr>
</table>

Veja alguns exemplos:

A variável **Rejeições de mensagens SMS** O acionador inicia um fluxo, como o envio de um email, quando uma mensagem SMS é rejeitada.

A variável **Inscreve-se na lista de vibrações** acionador inicia um fluxo quando uma pessoa se inscreve.

A variável **Link de cliques em mensagem SMS** O acionador inicia um fluxo quando uma pessoa clica em um link na mensagem SMS.

## Filtros de SMS {#sms-filters}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-3.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-4.png"></td>
  </tr>
</table>

Também é possível usar os filtros de Vibes nas Smart Lists. A variável **Inscrito na lista de vibrações** o filtro localiza qualquer pessoa que tenha *sempre* assinou o Vibes. Isso inclui pessoas canceladas e excluídas, mesmo que as pessoas excluídas sejam omitidas do fluxo. Esse filtro é mais adequado para relatórios.

Em contrapartida, a **Membro da lista de vibrações** o filtro localiza _qualquer pessoa_ No momento, está inscrito no Vibes e é mais adequado para uso em Campanhas inteligentes ou listas.

>[!NOTE]
>
>Todos os filtros SMS incluem o **Data da atividade** restrição por padrão.

Depois de configurar acionadores e filtros de Vibes na sua Smart List, você pode [definir o fluxo](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Enviar uma mensagem SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md)
>* [Definir lista inteligente para o Smart Campaign | Acionador](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Localizar e adicionar filtros a uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
