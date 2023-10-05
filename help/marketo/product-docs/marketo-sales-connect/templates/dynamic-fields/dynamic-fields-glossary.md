---
unique-page-id: 14352509
description: Glossário de campos dinâmicos - Documentação do Marketo - Documentação do produto
title: Glossário de campos dinâmicos
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: cffe7a8734f79f887f3aad017a16fad4f04cda74
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 1%

---

# Glossário de campos dinâmicos {#dynamic-fields-glossary}

Ao criar um modelo no Sales Connect, sempre recomendamos integrar campos dinâmicos, usando o **Campos dinâmicos do MSE** botão.

Esta ferramenta é usada para `auto-personalize your email` e poupe muito tempo até `pulling information from the People page`.

| Campo dinâmico | Exemplo do que aparece no email |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | Se você não deseja mais receber emails conosco, clique aqui |
| `{{friendly_unsubscribe}}` | Cansado de todos os emails? Por favor, avise-me aqui |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | Keith Flynn, Escritor Técnico Sênior - Adobe |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Escritor técnico sênior |
| `{{work_website}}` | https://www.adobe.com |

**Itens a serem observados**:

* Se as informações de um contato forem inseridas incorretamente ou estiverem ausentes na página Pessoas, elas não serão inseridas corretamente no modelo.
* A diferença entre `{{company}}` e `{{company_friendly}}` é isso `{{company_friendly}}` removerá qualquer título formal, como Inc., LLC., etc., do nome da empresa do seu contato.
* Ao usar `{{company_friendly}}`, separe a Inc. ou a Co. com uma vírgula nos detalhes de contato. É assim que o Sales Connect sabe o que remover ao obter o valor.
* O sistema anexa automaticamente a assinatura do usuário a cada email enviado. Se o usuário estiver usando um modelo com a variável `{{my_signature}}` dinâmico, o sistema preencherá a assinatura onde a variável `{{my_signature}}` o campo dinâmico foi colocado. Ele só é adicionado lá para evitar duplicação. O sistema tratará `{{team_unsubscribe}}` da mesma forma que quando a configuração global de cancelamento de inscrição de acréscimo está ativada.

>[!TIP]
>
>Você pode criar o seu próprio [campo dinâmico personalizado](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) para qualquer coisa que você gostaria de receber automaticamente em seus emails
