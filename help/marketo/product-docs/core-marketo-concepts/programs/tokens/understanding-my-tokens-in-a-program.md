---
unique-page-id: 1147114
description: Entendendo meus tokens em um programa - Documentação do Marketo - Documentação do produto
title: Compreender meus tokens em um programa
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
feature: Tokens
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 3%

---

# Compreender meus tokens em um programa {#understanding-my-tokens-in-a-program}

Um token é uma variável que pode ser usada em emails, Landing Pages e Campanhas inteligentes para facilitar sua vida.

Além de Meus tokens, também é possível usar qualquer um dos tokens incorporados em seus programas. Confira a [Visão geral dos tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}.

## Meus tokens  {#my-tokens}

Meus tokens são variáveis personalizadas que podem ser criadas por qualquer pessoa. Localmente, eles são [criados](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"} em pastas de campanha ou programas.

Meus tokens são exibidos assim: `{{my.Name Of Token}}`

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
   <td>Use este token para <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">adicionar um arquivo de evento de calendário (.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a> aos seus emails e landing pages.</td>
  </tr>
  <tr>
   <td><p>Data <img alt="--" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td>
   <td>Esse token contém um valor de data. A data é exibida como ano-mês-dia (por exemplo, 23-05-2016).</td>
  </tr>
  <tr>
   <td>Script de e-mail <img alt="--" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>Use esse token para executar um script do Velocity em seus emails. Saiba mais <a href="https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/email-scripting" title="Seguir link" rel="nofollow">aqui</a>. </td>
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
   <td>Use este token na <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">etapa de fluxo de pontuação de alteração</a>. </td>
  </tr>
  <tr>
   <td colspan="1">SFDC - Campanha <img alt="--" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="--"></td>
   <td colspan="1">Use esse token para permitir que clientes em potencial que se tornam parte de um Programa Marketo também sejam adicionados a qualquer campanha do SFDC adicionada.</td>
  </tr>
  <tr>
   <td>Texto <img alt="--" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td>
   <td>Só uma mensagem. Use-o quando o HTML for excessivo. O limite de tamanho para tokens de texto é de 524.288 caracteres (UTF-8) ou 2 MB.</td>
  </tr>
 </tbody>
</table>

>[!CAUTION]
>
>Meus Tokens não serão resolvidos ao enviar um email do Sales Insight em [!DNL Microsoft Dynamics] ou [!DNL Salesforce]; somente os tokens padrão serão preenchidos (Cliente Potencial, Empresa, etc.). No entanto, os valores padrão para os tokens _funcionarão_.

## Aninhamento de tokens {#nesting-tokens}

Quando você cria um novo token, ele pode ser referenciado por outros objetos na árvore. Há uma estrutura de nomenclatura para a qual o token foi criado para facilitar o gerenciamento.

* **Token Local:** O token foi criado diretamente nesse programa ou pasta.
* **Token Herdado:** O token foi criado na árvore em algum lugar em um programa ou pasta de nível superior.
* **Token Substituído:** O token foi herdado e alguém fez uma exceção neste programa ou pasta.

Você pode criar variáveis globais e depois substituí-las em níveis inferiores na árvore.

A movimentação de programas e pastas também afeta tokens. Sempre verifique se as referências não foram quebradas durante a movimentação.

>[!IMPORTANT]
>
>Não há suporte para tokens aninhados em [Campanhas em lote](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/understanding-batch-and-trigger-smart-campaigns.md#batch-campaign){target="_blank"}.

>[!NOTE]
>
>Se o email enviado de um programa de engajamento for um email secundário de um programa padrão (não local para o seu programa de engajamento), quaisquer Meus tokens usados no email serão resolvidos no programa padrão em que o email secundário reside.

>[!MORELIKETHIS]
>
>* [Visão geral dos tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}
>* [Gerenciando Meus Tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
