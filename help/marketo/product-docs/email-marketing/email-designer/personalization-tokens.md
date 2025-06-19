---
solution: Marketo Engage
product: marketo
title: Tokens do Personalization
description: Saiba como usar tokens de personalização no novo Marketo Engage Email Designer
level: Beginner, Intermediate
feature: Email Designer
exl-id: 4828e1a5-822f-48a9-bbb8-b1ffe8421e4f
source-git-commit: bfa1bc900c2adc263e634a81440b77bef2976d3b
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Tokens do Personalization {#personalization-tokens}

O designer de email tem um formato diferente do editor de email clássico quando se trata de tokens de personalização de email. A alteração foi implementada para melhorar a compatibilidade com o script do Handlebar e simplificar o processo de criação de email.

>[!AVAILABILITY]
>
>A partir de 23 de maio de 2025, esse recurso será provisionado para usuários do Marketo Engage em lotes, com uma região atualizada por semana. Durante a implantação, todos os emails criados usando o novo designer de email migrarão automaticamente os tokens existentes para o novo formato. Com esta atualização, todos os tokens estarão disponíveis somente em inglês.

## Caso de uso principal {#primary-use-case}

Esse aprimoramento beneficia principalmente as transições de [scripts do Velocity](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/email-scripting){target="_blank"} para scripts do Handlebar. O novo designer de email só oferece suporte ao novo formato de token. O formato atualizado elimina espaços e introduz uma estrutura de texto padrão revisada, garantindo uma experiência de script mais suave e eficiente.

## Experiência do token {#token-experience}

Uma análise da experiência de token, antiga e nova.

### Formato antigo {#old-format}

No editor de email clássico, você pode adicionar tokens com espaços, como `lead.Anonymous IP` ou `member.registration code`. O formato do texto padrão era: `{{lead.City:default=fallback}}`

![](assets/personalization-tokens-1.png){width="800" zoomable="yes"}

### Novo formato {#new-format}

No designer de email, você deve usar [camel case](https://developer.mozilla.org/en-US/docs/Glossary/Camel_case) ou sublinhados para tokens (por exemplo, `lead.anonymousIP` ou `member.registration_code`). O formato do texto padrão também é alterado para `{%=lead.city ?: "fallback" %}`.

![](assets/personalization-tokens-2.png){width="800" zoomable="yes"}

## Itens a Observar {#things-to-note}

* O editor de personalização também apresenta as seguintes funções para facilitar a criação:

   * Desfazer/refazer
   * Localizar/Localizar e substituir
   * Preenchimento automático

* **Todos** os tokens anteriormente suportados no Marketo Engage são suportados pelo novo editor de personalização.
