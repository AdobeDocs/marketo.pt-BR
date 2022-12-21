---
unique-page-id: 14352509
description: Glossário de campos dinâmicos - Documentos do Marketo - Documentação do produto
title: Glossário de campos dinâmicos
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 2%

---

# Glossário de campos dinâmicos {#dynamic-fields-glossary}

Ao criar um modelo no Sales Connect, sempre recomendamos a integração de campos dinâmicos usando o **Campos dinâmicos do MSE** botão.

Esta ferramenta é usada para `auto-personalize your email` e economize toneladas de tempo `pulling information from the People page`.

| Campo dinâmico | Exemplo do que aparece no email |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Se você não quiser ouvir de mim novamente, por favor, me informe aqui |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Escritor Técnico Sênior |
| `{{work_website}}` | https://www.marketo.com |

**O que registrar**:

* Se as informações de um contato forem inseridas incorretamente ou estiverem ausentes na página Pessoas, elas não serão inseridas corretamente no modelo.
* A diferença entre `{{company}}` e `{{company_friendly}}` é que `{{company_friendly}}` removerá qualquer título formal, como Inc., LLC. etc., do nome da empresa do seu contato.
* Ao usar `{{company_friendly}}`, certifique-se de separar Inc. ou Co. por uma vírgula nos detalhes do contato. É assim que o Sales Connect sabe o que remover ao obter o valor.

>[!TIP]
>
>Você pode criar seu próprio [campo dinâmico personalizado](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) para qualquer item que você gostaria de ter enviado automaticamente para seus emails
