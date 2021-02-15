---
unique-page-id: 14352509
description: Glossário de Campos Dinâmicos - Documentos do Marketing - Documentação do Produto
title: Glossário de Campos Dinâmicos
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Glossário de Campos Dinâmicos {#dynamic-fields-glossary}

Ao criar um modelo no Sales Connect, recomendamos sempre a integração de campos dinâmicos usando o botão **MSE Dynamic Fields**.

Esta ferramenta é usada para `auto-personalize your email` e economiza tempo em `pulling information from the People page`.

| Campo dinâmico | Exemplo do que aparece no seu email |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Se você não quiser ouvir de mim novamente, por favor, me avise aqui |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Escritor técnico sênior |
| `{{work_website}}` | https://www.marketo.com |

**Observação**:

* Se as informações de um contato forem inseridas incorretamente ou estiverem ausentes na página Pessoas, ele não será transferido corretamente para o modelo.
* A diferença entre `{{company}}` e `{{company_friendly}}` é que `{{company_friendly}}` removerá qualquer título formal, como Inc., LLC., etc., do nome da empresa do contato.
* Ao usar `{{company_friendly}}`, certifique-se de separar Inc. ou Co. com uma vírgula nos detalhes do contato. É assim que o Sales Connect sabe o que remover ao obter o valor.

>[!TIP]
>
>Você pode criar seu próprio [campo dinâmico personalizado](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) para qualquer item que você gostaria de ter inserido automaticamente em seus emails
