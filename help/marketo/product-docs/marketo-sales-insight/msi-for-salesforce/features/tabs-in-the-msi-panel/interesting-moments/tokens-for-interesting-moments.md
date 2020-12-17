---
unique-page-id: 1146999
description: Tokens para momentos interessantes - Documentos de marketing - Documentação do produto
title: Tokens para momentos interessantes
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Tokens para Momentos Interessantes {#tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>* Saiba como usar a [Etapa de fluxo de Momento Interessante](../../../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md).
>* Saiba mais sobre [tokens](http://docs.marketo.com/display/docs/tokens).

>



## Tokens disponíveis {#available-tokens}

Confira [Visão geral dos tokens](../../../../../../product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) para ver todos os tokens que você pode colocar em um momento interessante.

## Tokens de acionamento {#trigger-tokens}

Com base no acionador usado em uma campanha inteligente, tokens de acionador adicionais são disponibilizados.

* `{{trigger.Trigger Name}}` que é sempre o próprio gatilho. Por exemplo: Clique em Link no email.
* `{{trigger.Name}}` é o nome do ativo que acionou a campanha. Por exemplo: O link de cliques na página da Web é o próprio URL, sujeito a acionadores do Salesforce etc.
* Adicionais acionadores estão disponíveis com base em restrições, listadas abaixo:

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
  </tr> 
  <tr> 
   <td>Cliques em links no email</td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Rejeições de e-mail difíceis</td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Rejeições de email suaves</td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>O email é entregue</td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Abre email</td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Cancela a assinatura do email</td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Link de cliques no email de vendas</td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Email de vendas enviadas</td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Abre email de vendas</td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Email de vendas recebido</td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
  </tr> 
  <tr> 
   <td colspan="1">E-mail de vendas retorcido</td> 
   <td colspan="1"><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td colspan="1"><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
  </tr> 
  <tr> 
   <td>Preencher formulário</td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td><br></td> 
   <td><p><br></p></td> 
  </tr> 
  <tr> 
   <td colspan="1">Página da Web de visitas*</td> 
   <td colspan="1"><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><img src="assets/check.svg" alt="(assinalar)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Se ele não tiver uma marca ![(tick)](assets/check.svg), retornará uma sequência vazia (nada) no momento interessante.

*O acionador **Visitas à página da Web** tem alguns tokens adicionais:

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>Sempre teste seus momentos interessantes para garantir que eles renderizem a maneira como você pretende.
>
>Além disso, certifique-se de que seja interessante para o vendedor, não apenas para você. ![(piscar)](assets/wink.svg)>

