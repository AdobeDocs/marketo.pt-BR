---
description: Uso das opções de SMS em uma campanha inteligente - Documentação do Marketo - Documentação do produto
title: Utilização das opções de SMS em uma campanha inteligente
feature: Mobile Marketing
source-git-commit: 5e2d1979abcafd8e4a37e55b843be932125c954e
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 2%

---

# Utilização das opções de SMS em uma campanha inteligente {#using-sms-options-in-a-smart-campaign}

Depois que você [criar uma mensagem SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}, você deverá usar os acionadores e filtros de Smart List em uma Campanha inteligente para obter os benefícios.

>[!NOTE]
>
>Se você deseja enviar uma mensagem SMS, temos uma [artigo específico](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"} por isso.

>[!PREREQUISITES]
>
>Os acionadores/filtros de SMS só aparecerão se a variável [O serviço Vibes foi ativado](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}.

## Acionadores de SMS {#sms-triggers}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-1.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-2.png"></td>
  </tr>
</table>

Veja alguns exemplos:

A variável **Rejeições de mensagens SMS** O acionador inicia um fluxo, como o envio de um email, quando uma mensagem SMS é rejeitada.

A variável **Inscreve-se na lista de vibrações** acionador inicia um fluxo quando uma pessoa se inscreve.

A variável **Link de cliques em mensagem SMS** O acionador inicia um fluxo quando uma pessoa clica em um link na mensagem SMS.

## Filtros de SMS {#sms-filters}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-3.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-4.png"></td>
  </tr>
</table>

A variável **Inscrito na lista de vibrações** o filtro localiza qualquer pessoa que tenha *sempre* assinou o Vibes. Isso inclui pessoas canceladas e excluídas, mesmo que as pessoas excluídas sejam omitidas do fluxo. Esse filtro é mais adequado para relatórios.

Em contrapartida, a **Membro da lista de vibrações** o filtro localiza _qualquer pessoa_ No momento, está inscrito no Vibes e é mais adequado para uso em Campanhas inteligentes ou listas.

>[!NOTE]
>
>Todos os filtros SMS incluem o **Data da atividade** restrição por padrão.

## Etapas de fluxo de SMS {#sms-flow-steps}

Há três etapas de fluxo de SMS para escolher.

![](assets/using-sms-options-in-a-smart-campaign-5.png)

<table>
<tbody>
  <tr>
    <td style="width:20%"><b>Enviar mensagem de SMS</b></td>
    <td>Essa ação de fluxo envia mensagens para pessoas da Smart List do Marketo que estão inscritas em uma lista de inscrição de vibrações de opt-in do usuário. Ele não inicia o processo de assinatura. <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md">Saiba mais</a>.</td>
  </tr>

<tr>
    <td style="width:20%"><b>Assinar a lista do Vibes</b></td>
    <td>Essa ação de fluxo inicia o processo de assinatura do SMS por meio de uma campanha de aquisição de Vibes selecionada pelo usuário. A Vibes envia uma mensagem de confirmação, e o recipient deve responder com "Y" dentro de 24 horas para confirmar a aceitação. Depois que o usuário aceitar, ele se tornará membro da lista de inscrição do Vibes associada.</td>
  </tr>
  <tr>
    <td style="width:20%"><b>Cancelar inscrição da lista do Vibes</b></td>
    <td>Essa ação de fluxo cancela a assinatura de cada pessoa em uma lista de assinaturas de Vibes de opt-in do usuário. Quando um usuário envia um texto "PARAR" para o seu código, o registro pessoal dele é atualizado para refletir que não é mais membro da lista de assinaturas do Vibes.</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>A variável **Inscrever-se na lista de visibilidade** e **Cancelar inscrição na lista de vibrações** Os fluxos de trabalho têm requisitos diferentes. Para **Assinar**, você deve selecionar a lista Vibes e a campanha de aquisição Vibes. Para **Cancelar inscrição**, somente a lista Vibes é necessária.

>[!MORELIKETHIS]
>
>* [Enviar uma mensagem SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}
>* [Definir lista inteligente para o Smart Campaign | Acionador](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
>* [Definir lista inteligente para o Smart Campaign | Lote](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}
