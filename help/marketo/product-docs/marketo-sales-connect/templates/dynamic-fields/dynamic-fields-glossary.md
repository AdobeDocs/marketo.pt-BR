---
unique-page-id: 14352509
description: Glossário de Campos Dinâmicos - Documentos do Marketing - Documentação do Produto
title: Glossário de Campos Dinâmicos
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '173'
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
| `{{personal_email}}` | [[protegido por email]](http://docs.marketo.com/cdn-cgi/l/email-protection) |
| `{{title}}` | Escritor técnico sênior |
| `{{work_website}}` | https://www.marketo.com |

**Observação**:

* Se um contato for `information is entered incorrectly` ou estiver faltando na página Pessoas, ele será `will not pull over correctly` inserido em seu modelo.

* A diferença entre `{{company}}` e `{{company_friendly}}` é que `{{company_friendly}}` irá `remove any formal title`, como Inc., LLC., etc., a partir do nome da empresa do seu contato.
* Ao usar `{{company_friendly}}`, certifique-se de separar Inc. ou Co. com uma vírgula nos detalhes do contato. É assim que o Sales Connect sabe o que remover ao obter o valor.

>[!TIP]
>
>Você pode criar seu próprio [campo dinâmico personalizado](http://docs.marketo.com/x/fADb) para qualquer item que você gostaria de ter inserido automaticamente em seus emails

