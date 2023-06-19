---
description: Por que meus campos dinâmicos não estão sendo preenchidos? - Documentação do Marketo - Documentação do produto
title: Por que meus campos dinâmicos não estão sendo preenchidos?
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%

---

# Por que meus campos dinâmicos não estão sendo preenchidos? {#why-arent-my-dynamic-fields-filling-out}

Os campos dinâmicos só funcionarão quando você estiver usando um modelo. Emails únicos individuais que você escreve não vão preencher isso.

## O que verificar {#what-to-check}

Há três tipos de campos dinâmicos em Ações do Sales Insight: Básico, Personalizado e Salesforce. Básico e personalizado, ambos procuram obter informações do [aplicativo web](https://toutapp.com/login){target="_blank"}. If the information does not exist in the web application, the fields will be blank. Salesforce fields pull information from [Salesforce.com](https://salesforce.com){target="_blank"}.

**Solução de problemas de campos do Salesforce**

Campos do Salesforce: ex. `{{sfdc_account_name}}`

* Verifique se ele está conectado corretamente às Ações do Sales Insight. Vá para a [Configurações](https://toutapp.com/login{target="_blank"} e clique em **Gerenciar** ao lado do seu CRM.

**Solução de problemas de campos básicos e personalizados**

Campos básicos de ações do Marketo Sales Insight: por exemplo, `{{company}}`

Campos personalizados de ações do Marketo Sales Insight: por exemplo, `{{custom_field_favorite_movie}}`

* O campo correspondente precisa ser salvo para o contato na variável [Página Pessoas](https://toutapp.com/next#relationships){target="_blank"} para que nosso campo dinâmico faça referência. Por exemplo, se você estiver enviando um email para Mary e estiver usando o `{{company}}` mas seu registro de contato não lista uma empresa, não poderemos preencher isso.

## Por Que Meu Email Foi Enviado Sem Preencher Todos Os Campos Dinâmicos? {#why-did-my-email-send-without-populating-all-dynamic-fields}

As ações de insight de vendas impedirão que seus emails sejam enviados se não for possível preencher todos os campos dinâmicos no email. **No entanto** No entanto, há algumas exceções a essa regra. Alguns campos enviarão um valor em branco ou preencherão automaticamente se for possível encontrar um. Esses campos e como eles reagirão se não puderem preencher o campo estão listados abaixo.

`{{first_name}}` = EM BRANCO

`{{last_name}}` =EM BRANCO

`{{title}}` = EM BRANCO

`{{company}}` = &quot;sua empresa&quot;

`{{friendly_company}}` = &quot;sua empresa&quot;

>[!NOTE]
>
>A variável `{{first_name}}` procura em Ações de Insight de vendas e Salesforce para tentar obter informações. Todos os outros campos dessa lista só estão procurando nas Ações de Insight de vendas para preencher o campo.
