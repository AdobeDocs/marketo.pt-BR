---
description: Por que meus campos dinâmicos não estão sendo preenchidos? - Documentação do Marketo - Documentação do produto
title: Por que meus campos dinâmicos não estão sendo preenchidos?
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Por que meus campos dinâmicos não estão sendo preenchidos? {#why-arent-my-dynamic-fields-filling-out}

Os campos dinâmicos só funcionarão quando você estiver usando um modelo. Emails únicos individuais que você escreve não vão preencher isso.

## O que verificar {#what-to-check}

Há três tipos de campos dinâmicos em Ações do Sales Insight: Básico, Personalizado e Salesforce. Básico e Personalizado, ambos procuram obter informações do [aplicativo Web](https://toutapp.com/login){target="_blank"}. Se as informações não existirem no aplicativo web, os campos estarão em branco. Os campos do Salesforce extraem informações do [Salesforce.com](https://salesforce.com){target="_blank"}.

**Solução de problemas de campos do Salesforce**

Campos do Salesforce: ex.: `{{sfdc_account_name}}`

* Verifique se ele está conectado corretamente às Ações do Sales Insight. Vá para a página [Configurações] (https://toutapp.com/login{target="_blank"} e clique em **Gerenciar** ao lado do seu CRM.

**Solução de problemas de campos básicos e personalizados**

Campos Básicos das Ações do Marketo Sales Insight: por exemplo, `{{company}}`

Campos Personalizados de Ações do Marketo Sales Insight: por exemplo, `{{custom_field_favorite_movie}}`

* O campo correspondente precisa ser salvo para o seu contato na [página Pessoas](https://toutapp.com/next#relationships){target="_blank"} para que o nosso campo dinâmico faça referência. Por exemplo, se você estiver enviando um email para Mary e estiver usando o campo `{{company}}`, mas o registro de contato dela não listar uma empresa, não poderemos preenchê-lo.

## Por Que Meu Email Foi Enviado Sem Preencher Todos Os Campos Dinâmicos? {#why-did-my-email-send-without-populating-all-dynamic-fields}

As ações de insight de vendas impedirão que seus emails sejam enviados se não for possível preencher todos os campos dinâmicos no email. **No entanto**, há algumas exceções a esta regra. Alguns campos enviarão um valor em branco ou preencherão automaticamente se for possível encontrar um. Esses campos e como eles reagirão se não puderem preencher o campo estão listados abaixo.

`{{first_name}}` = EM BRANCO

`{{last_name}}` =EM BRANCO

`{{title}}` = EM BRANCO

`{{company}}` = &quot;sua empresa&quot;

`{{friendly_company}}` = &quot;sua empresa&quot;

>[!NOTE]
>
>O campo `{{first_name}}` procurará em Ações do Sales Insight e no Salesforce para tentar obter informações. Todos os outros campos dessa lista só estão procurando nas Ações de Insight de vendas para preencher o campo.
