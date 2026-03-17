---
unique-page-id: 2950799
description: Saiba mais sobre tokens para personalizar páginas de aterrissagem do Marketo. Use tokens para inserir conteúdo dinâmico e personalizar a experiência.
title: Visão geral dos tokens
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
feature: Landing Pages
source-git-commit: 031eb5f3ff8aac185ce496664f984a4c745c6e44
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 94%

---

# Visão geral dos tokens {#tokens-overview}

Um token é uma variável que pode ser usada em etapas de fluxo de campanha inteligente do Marketo, emails, páginas de destino, trechos e campanhas da web.

## Noções básicas dos valores padrão {#understanding-default-values}

Ao usar um token, também é uma boa ideia fornecer um valor padrão. Trata-se do texto que aparece quando uma pessoa não tem um valor para o campo que você está referenciando.

![](assets/image2014-12-2-13-3a16-3a48.png)

Neste exemplo, o email dirá “Olá, (nome)” ou “Olá, terráqueo” (valor padrão).

![](assets/two.png)

>[!CAUTION]
>
>Os tokens não funcionam no pré-cabeçalho ao usar o editor de email do Marketo. Para usar um token no pré-cabeçalho, ele precisa ser enviado por meio do seu próprio HTML em um modelo de email.

>[!NOTE]
>
>Esta lista não é exaustiva. Também são criados tokens para cada campo personalizado existente no Marketo.

## Tokens de pessoas {#person-tokens}

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
* Campos de pessoa personalizados também funcionam se você usar o nome de exibição da pessoa, como, por exemplo, `{{lead.Custom Field Name}}`

## Tokens de empresas {#company-tokens}

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
* Campos personalizados de empresa também funcionam se você usar o nome de exibição da empresa, como, por exemplo, `{{Company.Custom Field Name}}`

## Tokens de campanhas {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## Tokens do sistema {#system-tokens}

>[!NOTE]
>
>Saiba mais sobre esses tokens no [Glossário de tokens do sistema](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md).

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## Tokens de acionadores {#trigger-tokens}

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
>Encontre mais detalhes sobre [tokens para momentos interessantes](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) com base nos acionadores usados em uma campanha inteligente.

## Tokens de programa {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## [!UICONTROL Meus tokens] {#my-tokens}

[!UICONTROL Meus tokens] são definidos em um programa e começam com `{{my.` seguido pelo nome que você criou para o token. Saiba mais sobre [Meus tokens em um programa](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md).

## Token de membro {#member-token}

Os tokens de membro são usados para inserir valores exclusivos de parceiros de serviços integrados. Um uso comum de tokens de membros é para URLs exclusivos de participantes de webinários. Cada pessoa tem um URL exclusivo para acessar o webinário, que pode ser inserido por meio de um token de `{{member.webinar url}}`. O token de `{{member.webinar url}}` resolve automaticamente o URL de confirmação exclusivo da pessoa gerado pelo prestador de serviços.

* `{{member.webinar url}}`

>[!CAUTION]
>
>O token de `{{member.webinar url}}` só é preenchido se a campanha inteligente que enviou o email for um ativo secundário do programa do evento.
