---
unique-page-id: 1146999
description: Tokens de acionador para momentos interessantes - Documentação do Marketo - Documentação do produto
title: Tokens acionadores de momentos interessantes
exl-id: 666a6eed-c432-4088-b4f1-54c996eca64c
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 68%

---

# Tokens acionadores de momentos interessantes {#trigger-tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>Saiba como usar a [etapa do fluxo de Momento interessante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md).

## Tokens disponíveis {#available-tokens}

Confira [Visão geral dos tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) para ver todos os tokens que você pode colocar em um momento interessante.

## Tokens de acionador {#trigger-tokens}

Com base no acionador usado em uma campanha inteligente, os Tokens de acionador adicionais são disponibilizados.

* `{{trigger.Trigger Name}}` que é sempre o próprio gatilho real. Por exemplo: cliques em Link no email.
* `{{trigger.Name}}` é o nome do ativo que disparou a campanha. Por exemplo: o link de cliques na página da Web é o próprio URL, assunto dos acionadores do Salesforce etc.
* Os acionadores adicionais estão disponíveis com base nas restrições, que estão listadas abaixo.

### Acionadores de email {#email-triggers}

<table style="table-layout:auto">
 <colgroup>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <th><br></th>
   <th><code>{{trigger.Trigger Name}}</code></th>
   <th><code>{{trigger.Name}}</code></th>
   <th><code>{{trigger.Link}}</code></th>
   <th><code>{{trigger.Subject}}</code></th>
   <th><code>{{trigger.Category}}</code></th>
   <th><code>{{trigger.Details}}</code></th>
   <th><code>{{trigger.Web Page}}</code></th>
   <th><code>{{trigger.Client IP Address}}</code></th>
   <th><code>{{trigger.Sent By}}</code></th>
   <th><code>{{trigger.Received By}}</code></th>
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr>
  <tr>
   <td>Clica em link de e-mail</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Rejeições permanentes de email</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>E-mail é devolvido temporariamente</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>O Email É Entregue</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Abre e-mail</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
    <tr>
   <td>Recebeu e-mail de "Encaminhar para amigo"</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
    <tr>
   <td>Enviou e-mail de "Encaminhar para amigo"</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
  </tr>
  <tr>
   <td>Cancela inscrição do e-mail</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
 </tbody>
</table>

### Salesforce Triggers {#salesforce-triggers}

<table style="table-layout:auto">
 <colgroup>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <th><br></th>
   <th><code>{{trigger.Trigger Name}}</code></th>
   <th><code>{{trigger.Name}}</code></th>
   <th><code>{{trigger.Link}}</code></th>
   <th><code>{{trigger.Subject}}</code></th>
   <th><code>{{trigger.Category}}</code></th>
   <th><code>{{trigger.Details}}</code></th>
   <th><code>{{trigger.Web Page}}</code></th>
   <th><code>{{trigger.Client IP Address}}</code></th>
   <th><code>{{trigger.Sent By}}</code></th>
   <th><code>{{trigger.Received By}}</code></th>
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr>
  <tr>
   <td>Clica em link de e-mail de vendas</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>É e-mail de vendas enviado</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Abre e-mail de vendas</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>E-mail de vendas é devolvido</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>E-mail de vendas é recebido</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
    <tr>
   <td>A oportunidade é atualizada</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
    <tr>
   <td>Alterações do proprietário</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>A pessoa é convertida</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>A pessoa é excluída da SFDC</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>A pessoa é sincronizada com a SFDC</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Removido da oportunidade</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Removido da campanha da SFDC</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>A atividade é registrada</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>A atividade é atualizada</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Adicionado à oportunidade</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Adicionado à campanha da SFDC</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>O status é alterado na campanha da SFDC</td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
 </tbody>
</table>

### Acionadores da conexão de vendas {#sales-connect-triggers}

<table style="table-layout:auto">
 <colgroup>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <th><br></th>
   <th><code>{{trigger.Trigger Name}}</code></th>
   <th><code>{{trigger.Name}}</code></th>
   <th><code>{{trigger.Link}}</code></th>
   <th><code>{{trigger.Subject}}</code></th>
   <th><code>{{trigger.Category}}</code></th>
   <th><code>{{trigger.Details}}</code></th>
   <th><code>{{trigger.Web Page}}</code></th>
   <th><code>{{trigger.Client IP Address}}</code></th>
   <th><code>{{trigger.Sent By}}</code></th>
   <th><code>{{trigger.Received By}}</code></th>
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr>
  <tr>
   <td>Clica em link de e-mail de vendas</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>É e-mail de vendas enviado</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Abre e-mail de vendas</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>E-mail de vendas é devolvido</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>E-mail de vendas é recebido</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Está adicionado à campanha de vendas</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Alterações do proprietário</td>
   <td>Está removido de campanha de vendas</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Recebida chamada de vendas</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
 </tbody>
</table>

### Tokens de acionador do Dynamic Chat {#dynamic-chat-trigger-tokens}

<table>
<thead>
  <tr>
    <th> </th>
    <th><code>{{trigger.Agent Email}}</code></th>
    <th><code>{{trigger.Agent Name}}</code></th>
    <th><code>{{trigger.Conversation Status}}</code></th>
    <th><code>{{trigger.Conversation Summary}}</code></th>
    <th><code>{{trigger.Conversation Transcript}}</code></th>
    <th><code>{{trigger.Document Downloaded}}</code></th>
    <th><code>{{trigger.Document Name}}</code></th>
    <th><code>{{trigger.Document Opened}}</code></th>
    <th><code>{{trigger.Document URL}}</code></th>
    <th><code>{{trigger.Goal name}}</code></th>
    <th><code>{{trigger.meeting status}}</code></th>
    <th><code>{{trigger.Name}}</code></th>
    <th><code>{{trigger.Page URL}}</code></th>
    <th><code>{{trigger.routing queue name}}</code></th>
    <th><code>{{trigger.Scheduled For}}</code></th>
    <th><code>{{trigger.source name}}</code></th>
    <th><code>{{trigger.source type}}</code></th>
    <th><code>{{trigger.Trigger Name}}</code></th>
    <th><code>{{trigger.ui type}}</code></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Interagiu com um diálogo</td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Interagiu com um formulário de conversação</td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
  </tr>
  <tr>
    <td>Interagiu com um agente no diálogo</td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Interagiu com um agente no formulário de conversação</td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Agendou reunião no diálogo</td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Reunião agendada no formulário de conversação</td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Atingiu a meta do diálogo</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Meta de formulário de conversação alcançada</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Interagiu com o documento no diálogo</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Interagiu com o documento no formulário de conversação</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
</tbody>
</table>

### Diversos {#miscellaneous}

<table style="table-layout:auto">
 <colgroup>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <th><br></th>
   <th><code>{{trigger.Trigger Name}}</code></th>
   <th><code>{{trigger.Name}}</code></th>
   <th><code>{{trigger.Link}}</code></th>
   <th><code>{{trigger.Subject}}</code></th>
   <th><code>{{trigger.Category}}</code></th>
   <th><code>{{trigger.Details}}</code></th>
   <th><code>{{trigger.Web Page}}</code></th>
   <th><code>{{trigger.Client IP Address}}</code></th>
   <th><code>{{trigger.Sent By}}</code></th>
   <th><code>{{trigger.Received By}}</code></th>
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr>
  <tr>
   <td>Preenche o formulário</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Visita a página da web</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
  </tr>
  <tr>
   <td>Clica no link na página da Web</td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><img src="assets/check.png" alt="check"></td>
   <td><br></td>
   <td><br></td>
   <td><br></td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>Se ele não tiver uma verificação ![(tick)](assets/check.png) então ele retornaria uma string vazia (nada) no momento interessante.

&#42;A **Página da Web de Visitas** do Acionador tem alguns tokens adicionais:

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>Sempre teste seus momentos interessantes para garantir que eles renderizem da maneira que você pretende.
>
>Além disso, certifique-se de que seja interessante para o vendedor, não apenas para você!
