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

Ao criar um modelo no Sales Connect, recomendamos sempre a integração de campos dinâmicos usando o botão Campos **dinâmicos do** MSE.

Esta ferramenta é usada para `auto-personalize your email` salvar você e economizar muito tempo por `pulling information from the People page`.

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

* Se um contato estiver ausente `information is entered incorrectly` ou estiver faltando na página Pessoas, ele será usado `will not pull over correctly` no modelo.

* A diferença entre `{{company}}` e `{{company_friendly}}` é que `{{company_friendly}}` irá `remove any formal title`, como Inc., LLC., etc., do nome da empresa do seu contato.
* Ao usar `{{company_friendly}}`, separe Inc. ou Co. com uma vírgula nos detalhes do contato. É assim que o Sales Connect sabe o que remover ao obter o valor.

>[!TIP]
>
>Você pode criar seu próprio campo [dinâmico](http://docs.marketo.com/x/fADb) personalizado para qualquer item que você gostaria de ter inserido automaticamente em seus emails

