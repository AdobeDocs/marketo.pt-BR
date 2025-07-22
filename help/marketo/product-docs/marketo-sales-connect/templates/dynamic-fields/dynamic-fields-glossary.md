---
unique-page-id: 14352509
description: Glossário de campos dinâmicos - Documentação do Marketo - Documentação do produto
title: Glossário de campos dinâmicos
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 2%

---

# Glossário de campos dinâmicos {#dynamic-fields-glossary}

Ao criar um modelo em [!DNL Sales Connect], sempre recomendamos a integração de campos dinâmicos, usando o botão **[!UICONTROL Campos Dinâmicos do MSE]**.

Esta ferramenta é usada para `auto-personalize your email` e poupar toneladas de tempo até `pulling information from the [!UICONTROL People] page`.

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

**Observações**:

* Se as informações de um contato forem inseridas incorretamente ou estiverem ausentes na página Pessoas, elas não serão inseridas corretamente no modelo.
* A diferença entre `{{company}}` e `{{company_friendly}}` é que `{{company_friendly}}` removerá qualquer título formal, como Inc., LLC., etc., do nome da empresa do seu contato.
* Ao usar o `{{company_friendly}}`, separe a Inc. ou a Co. com uma vírgula nos detalhes de contato. É assim que o Sales Connect sabe o que remover ao obter o valor.
* O sistema anexa automaticamente a assinatura do usuário a cada email enviado. Se o usuário estiver usando um modelo com o campo dinâmico `{{my_signature}}`, o sistema preencherá a assinatura onde o campo dinâmico `{{my_signature}}` foi colocado. Ele só é adicionado lá para evitar duplicação. O sistema tratará `{{team_unsubscribe}}` da mesma maneira quando a configuração global de cancelamento de inscrição de acréscimo estiver habilitada.

>[!TIP]
>
>Você pode criar seu próprio [campo dinâmico personalizado](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) para qualquer item que desejar obter automaticamente em seus emails
