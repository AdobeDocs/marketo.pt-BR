---
unique-page-id: 2950799
description: Visão geral dos tokens - Documentos do Marketing - Documentação do produto
title: Visão geral dos tokens
translation-type: tm+mt
source-git-commit: efadb7eb3845012c273e1a60f9cd98ac884eb543
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---


# Visão geral dos tokens {#tokens-overview}

Um token é uma variável que pode ser usada em etapas de fluxo de campanha [inteligente do Marketo,](http://docs.marketo.com/display/DOCS/Smart+Campaigns) emails [,](http://docs.marketo.com/display/DOCS/General)landings page [,](http://docs.marketo.com/display/DOCS/Landing+Pages)trechos [e campanhas](http://docs.marketo.com/display/DOCS/Segmentation+and+Snippets)[](http://docs.marketo.com/display/public/DOCS/Using+the+Web+Personalization+Rich+Text+Editor)da Web.

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Como entender os valores padrão {#understanding-default-values}

Quando você usa um token, também deseja fornecer um valor padrão. Este é o texto que mostra se uma pessoa não tem um valor para o campo que você está referenciando.

![](assets/image2014-12-2-13-3a16-3a48.png)

Neste exemplo, o e-mail dirá &quot;Saudações, (nome)&quot; ou &quot;Saudações, Disparo&quot; (valor padrão).

![](assets/two.png)

>[!CAUTION]
>
>Os tokens não funcionam no precabeçalho ao usar o editor de email do Marketo. Para usar um token no pré-cabeçalho, ele deve estar em seu próprio HTML em um modelo de email.

>[!NOTE]
>
>Esta lista não é exaustiva. Tokens também são criados para cada campo personalizado que você tem no Marketo.

## Tokens da Pessoa {#person-tokens}

* `{{lead.Acquisition Date}}`
* `{{lead.Acquisition Program Name}}`
* `{{lead.Acquisition Program}}`
* `{{lead.Address}}`
* `{{lead.Anonymous IP}}`
* `{{lead.Black Listed}}`
* `{{lead.City}}`
* `{{lead.Country}}`
* `{{lead.Created At}}`
* `{{lead.Date of Birth}}`
* `{{lead.Department}}`
* `{{lead.Do Not Call}}`
* `{{lead.Do Not Call Reason}}`
* `{{lead.Email Address}}`
* `{{lead.Email Invalid}}`
* `{{lead.Email Invalid Cause}}`
* `{{lead.Fax Number}}`
* `{{lead.First Name}}`
* `{{lead.Full Name}}`
* `{{lead.Id}}`
* `{{lead.Inferred City}}`
* `{{lead.Inferred Company}}`
* `{{lead.Inferred Country}}`
* `{{lead.Inferred Metropolitan Area}}`
* `{{lead.Inferred Phone Area Code}}`
* `{{lead.Inferred Postal Code}}`
* `{{lead.Inferred State Region}}`
* `{{lead.Is Customer}}`
* `{{lead.Is Employee}}`
* `{{lead.Is Partner}}`
* `{{lead.Job Title}}`
* `{{lead.Last Name}}`
* `{{lead.Lead Source}}`
* `{{lead.Marketing Suspended}}`
* `{{lead.Middle Name}}`
* `{{lead.Mobile Phone Number}}`
* `{{lead.Original Referrer}}`
* `{{lead.Original Search Engine}}`
* `{{lead.Original Search Phrase}}`
* `{{lead.Original Source Info}}`
* `{{lead.Original Source Type}}`
* `{{lead.Person Notes}}`
* `{{lead.Phone Number}}`
* `{{lead.Registration Source Info}}`
* `{{lead.Registration Source Type}}`
* `{{lead.Salutation}}`
* `{{lead.SFDC Created Date}}`
* `{{lead.SFDC Is Deleted}}`
* `{{lead.SFDC Type}}`
* `{{lead.Unsubscribed}}`
* `{{lead.Unsubscribed Reason}}`
* `{{lead.Updated At}}`
* Os campos personalizados de pessoa também funcionam se você usar seu nome de exibição, por exemplo, `{{lead.Custom Field Name}}`

## Tokens de empresa {#company-tokens}

* `{{Company.Account Owner Email Address}}`
* `{{Company.Address}}`
* `{{Company.Annual Revenue}}`
* `{{Company.City}}`
* `{{Company.Company Name}}`
* `{{Company.Company Notes}}`
* `{{Company.Country}}`
* `{{Company.Industry}}`
* `{{Company.Main Phone}}`
* `{{Company.Num Employees}}`
* `{{Company.Parent Company Name}}`
* `{{Company.Postal Code}}`
* `{{Company.SFDC Account Num}}`
* `{{Company.SFDC Created Date}}`
* `{{Company.SFDC Type}}`
* `{{Company.SIC Code}}`
* `{{Company.Site}}`
* `{{Company.State}}`
* `{{Company.Website}}`
* Os campos de empresa personalizados também funcionam se você usar o nome de exibição ex. `{{Company.Custom Field Name}}`

## Tokens de campanha {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## Tokens do sistema {#system-tokens}

>[!NOTE]
>
>Saiba mais sobre esses tokens no Glossário [de Tokens do Sistema](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md).

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## Tokens do acionador {#trigger-tokens}

* `{{trigger.Trigger Name}}`
* `{{trigger.Name}}`
* `{{trigger.Link}}`
* `{{trigger.Subject}}`
* `{{trigger.Category}}`
* `{{trigger.Details}}`
* `{{trigger.Web Page}}`
* `{{trigger.Client IP Address}}`
* `{{trigger.Sent By}}`
* `{{trigger.Received By}}`
* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!NOTE]
>
>Encontre mais detalhes sobre [tokens para momentos](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/tokens-for-interesting-moments.md) interessantes com base em acionadores usados em uma campanha inteligente.

## Tokens de programa {#program-tokens}

* `{{program.Name}}`

* `{{program.Description}}`

* `{{program.id}}`

## Meus Tokens {#my-tokens}

Meus tokens são definidos em um programa e começam com `{{my.` o nome que você criou para o token. Saiba mais sobre [Meus tokens em um programa](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md).

## Token de membro {#member-token}

Tokens de membros são usados para inserir valores únicos de parceiros de serviços integrados. Um uso comum dos Tokens de Membro é para URLs exclusivos para participantes de webinar. Cada pessoa tem um URL exclusivo para acessar o webinar que pode ser inserido usando um `{{member.webinar url}}` token. O `{{member.webinar url}}` token resolve automaticamente o URL de confirmação exclusivo da pessoa gerado pelo provedor de serviço.

* `{{member.webinar url}}`

>[!CAUTION]
>
>O `{{member.webinar url}}` token só será preenchido se a campanha inteligente que envia o email for um ativo filho do Programa do Evento.
