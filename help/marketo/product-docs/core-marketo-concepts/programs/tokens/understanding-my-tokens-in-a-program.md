---
unique-page-id: 1147114
description: Noções básicas sobre meus tokens em um programa - Documentos do Marketo - Documentação do produto
title: Noções básicas sobre meus tokens em um programa
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 3%

---

# Noções básicas sobre meus tokens em um programa {#understanding-my-tokens-in-a-program}

Um token é uma variável que pode ser usada em emails, landing pages e campanhas inteligentes para facilitar a vida.

Além de Meus tokens, você também pode usar qualquer um dos tokens incorporados em seus programas. Confira o [Visão geral de tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md).

## Meus tokens  {#my-tokens}

Meus tokens são variáveis personalizadas que qualquer pessoa pode criar. Eles são [criado](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) em pastas ou programas de campanha.

Meus tokens são exibidos desta forma: `{{my.Name Of Token}}`

Exemplos:

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

<table> 
 <thead> 
  <tr> 
   <th>Tipo de token</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Arquivo de calendário <img alt="—" src="assets/image2014-9-25-16-3a44-3a19.png" data-linked-resource-id="3083230" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Usar este token para <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">adicionar um arquivo de evento de calendário (.i)</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a> para seus emails e landing pages.</td> 
  </tr> 
  <tr> 
   <td><p>Data <img alt="--" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>Esse token mantém um valor de data. A data é exibida como dia do mês do ano (por exemplo, 2016-05-23).</td> 
  </tr> 
  <tr> 
   <td>Script de e-mail <img alt="--" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Use esse token para executar um script do Velocity em seus emails. Saiba mais <a href="https://developers.marketo.com/documentation/email-scripting/" title="Seguir link" rel="nofollow">here</a>. </td> 
  </tr> 
  <tr> 
   <td>Número<span> <img alt="--" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>Qualquer número inteiro. Pode até ser negativo.</td> 
  </tr> 
  <tr> 
   <td>Texto formatado <img alt="--" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Este é o HTML. Use-o em emails e landing pages.</td> 
  </tr> 
  <tr> 
   <td>Pontuação <img alt="--" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Use esse token no <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">etapa do fluxo de pontuação de alteração</a>. </td> 
  </tr> 
  <tr> 
   <td colspan="1">SFDC - Campanha <img alt="--" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="--"></td> 
   <td colspan="1">Use esse token para permitir que leads que se tornam parte de um Programa Marketo também sejam adicionados a qualquer Campanha SFDC adicionada.</td> 
  </tr> 
  <tr> 
   <td>Texto <img alt="--" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Apenas um texto. Use-o quando o HTML for demais. O limite de tamanho para tokens de texto é de 524.288 caracteres (UTF-8) ou 2 MB.</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>Meus tokens não serão resolvidos ao enviar um email do Sales Insight no Microsoft Dynamics ou no Salesforce; somente os tokens padrão serão preenchidos (lead, empresa etc.). Valores padrão para tokens _will_ , no entanto.

## Aninhamento de tokens {#nesting-tokens}

Quando você faz um novo token, ele pode ser referenciado por outros objetos na árvore. Existe uma estrutura de nomenclatura para a qual o token foi criado para facilitar o gerenciamento.

* **Token local:** O token foi criado diretamente nesse programa ou pasta.
* **Token herdado:** O token foi criado na árvore em algum lugar em um programa ou pasta de nível superior.
* **Token substituído:** O token foi herdado e alguém fez uma exceção neste programa ou pasta.

Você pode fazer variáveis globais e depois substituí-las em níveis inferiores na árvore.

Mover programas e pastas afeta tokens também. Sempre verifique se as referências não estão quebradas durante a movimentação.

>[!NOTE]
>
>Se o email enviado de um programa de envolvimento for um email filho de um programa padrão (não local para o programa de envolvimento), todos os Meus tokens usados no email serão resolvidos do programa padrão em que o email filho reside.

>[!MORELIKETHIS]
>
>* [Visão geral de tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)
>* [Gerenciar meus tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)

