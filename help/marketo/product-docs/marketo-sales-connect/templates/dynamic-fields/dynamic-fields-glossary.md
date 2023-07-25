---
unique-page-id: 14352509
description: Glossário de campos dinâmicos - Documentação do Marketo - Documentação do produto
title: Glossário de campos dinâmicos
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 2%

---

# Glossário de campos dinâmicos {#dynamic-fields-glossary}

Ao criar um modelo no Sales Connect, sempre recomendamos integrar campos dinâmicos, usando o **Campos dinâmicos do MSE** botão.

Esta ferramenta é usada para `auto-personalize your email` e poupe muito tempo até `pulling information from the People page`.

| Campo dinâmico | Exemplo do que aparece no email |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Se você não quiser ouvir mais nada, por favor, avise-me |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Escritor técnico sênior |
| `{{work_website}}` | https://www.marketo.com |

**Itens a serem observados**:

* Se as informações de um contato forem inseridas incorretamente ou estiverem ausentes na página Pessoas, elas não serão inseridas corretamente no modelo.
* A diferença entre `{{company}}` e `{{company_friendly}}` é isso `{{company_friendly}}` removerá qualquer título formal, como Inc., LLC., etc., do nome da empresa do seu contato.
* Ao usar `{{company_friendly}}`, separe a Inc. ou a Co. com uma vírgula nos detalhes de contato. É assim que o Sales Connect sabe o que remover ao obter o valor.

>[!TIP]
>
>Você pode criar o seu próprio [campo dinâmico personalizado](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) para qualquer coisa que você gostaria de receber automaticamente em seus emails
