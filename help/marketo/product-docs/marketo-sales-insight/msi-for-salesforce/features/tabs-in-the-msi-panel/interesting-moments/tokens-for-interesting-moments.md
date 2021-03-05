---
unique-page-id: 1146999
description: Tokens para momentos interessantes - Documentos do Marketo - Documentação do produto
title: Tokens para Momentos Interessantes
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---


# Tokens para Momentos Interessantes {#tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>Saiba como usar o [passo de fluxo de Momento Interessante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md).

## Tokens disponíveis {#available-tokens}

Confira [Visão geral de tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) para ver todos os tokens que você pode colocar em um momento interessante.

## Tokens do acionador {#trigger-tokens}

Com base no acionador usado em uma campanha inteligente, tokens de acionador adicionais são disponibilizados.

* `{{trigger.Trigger Name}}` que é sempre o próprio acionador. Por exemplo: Cliques em Email.
* `{{trigger.Name}}` é o nome do ativo que acionou a campanha. Por exemplo: O Link de cliques na página da Web é o próprio URL, sujeito a acionadores do Salesforce etc.
* Os acionadores adicionais estão disponíveis com base em restrições, listadas abaixo.

**Acionadores de email**

<table> 
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
   <td>Link de cliques no email</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Rejeições de email intensas</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Rejeições de email suaves</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Abre Email</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Enviar para o Amigo Recebido</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Enviado para o Email Amigo</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td>
  </tr> 
  <tr> 
   <td>Cancela a assinatura do email</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**Salesforce Triggers**

<table> 
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
   <td>Link de cliques no email de vendas</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>É Enviado Email De Vendas</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Abre Email de Vendas</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Devoluções de email de vendas</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Email de Vendas é Recebido</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>A oportunidade é atualizada</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Alterações de Proprietário</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>A pessoa é Excluída do SFDC</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>A pessoa está sincronizada com o SFDC</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Removido da Oportunidade</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Removido da Campanha SFDC</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Atividade registrada</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Atividade atualizada</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Adicionado à Oportunidade</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Adicionado à Campanha SFDC</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>O status é alterado na campanha SFDC</td> 
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

**Acionadores da Conexão de Vendas**

<table> 
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
   <td>Link de cliques no email de vendas</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>É Enviado Email De Vendas</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Abre Email de Vendas</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Devoluções de email de vendas</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Email de Vendas é Recebido</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>É adicionado à campanha de vendas</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Alterações de Proprietário</td> 
   <td>É Removido Da Campanha De Vendas</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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
   <td>Chamada de Vendas Recebidas</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
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

**Diversos**

<table> 
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
   <td>Preenche Formulário</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Página da Web Visitas</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Link de cliques na página da Web</td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(marca de verificação)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Se não tiver uma marca ![(tick)](assets/check.svg) então ela retornará uma sequência vazia (nada) no momento interessante.

*O Acionador **Visitas Web Page** tem alguns tokens adicionais:

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>Sempre teste seus momentos interessantes para garantir que eles renderizem a maneira como você pretende.
>
>Além disso, certifique-se de que seja interessante para o vendedor, não apenas para você. ![(piscar)](assets/wink.svg)>
