---
description: Por que meus campos dinâmicos não estão preenchendo - Documentos do Marketo - Documentação do produto
title: Por que meus campos dinâmicos não estão preenchendo
hide: true
hidefromtoc: true
source-git-commit: 8e31c2da9351d784e97d3d2bfe0d3d07dfab8961
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---

# Por que meus campos dinâmicos não estão preenchendo {#why-arent-my-dynamic-fields-filling-out}

Os campos dinâmicos só funcionarão quando você estiver usando um modelo. Emails individuais únicos gravados não preencherão esses itens.

## O que verificar {#what-to-check}

Existem três tipos de campos dinâmicos em Ações de insight de vendas: Básico, Personalizado e Salesforce. Básico e Personalizado são ambos para obter informações do [aplicação web](https://toutapp.com/login). Se as informações não existirem na aplicação web, os campos ficarão em branco. Campos do Salesforce extraem informações de [Salesforce.com](https://salesforce.com).

**Resolução de problemas de campos do Salesforce**

Campos do Salesforce: por exemplo `{{sfdc_account_name}}`

* Certifique-se de que esteja corretamente conectado às Ações de insight de vendas. Vá para o [Configurações](https://toutapp.com/login) e clique em **Gerenciar** ao lado do seu CRM.

**Solução de problemas de campos básicos e personalizados**

Campos Básicos de Tout: por exemplo `{{company}}`

Campos personalizados do layout: por exemplo `{{custom_field_favorite_movie}}`

* O campo correspondente precisa ser salvo para seu contato no [Página Pessoas](https://toutapp.com/next#relationships) para o nosso campo dinâmico fazer referência. Por exemplo, se você estiver enviando um email para Mary e usando a variável `{{company}}` mas o registro de contato dela não lista uma empresa, não poderemos preencher isso.

## Por Que Meu Email Foi Enviado Sem Preencher Todos Os Campos Dinâmicos? {#why-did-my-email-send-without-populating-all-dynamic-fields}

As ações de insight de vendas impedirão que seus emails sejam enviados se não pudermos preencher todos os campos dinâmicos no email. **No entanto**, há algumas exceções a essa regra. Alguns campos enviarão em branco ou um valor será preenchido automaticamente se houver um. Esses campos e como eles reagirão se não conseguirem preencher o campo estão listados abaixo.

`{{first_name}}` = EM BRANCO

`{{last_name}}` =BLANK

`{{title}}` = EM BRANCO

`{{company}}` = &quot;sua empresa&quot;

`{{friendly_company}}` = &quot;sua empresa&quot;

>[!NOTE]
>
>O `{{first_name}}` O campo procurará nas Ações de insight de vendas e no Salesforce para tentar obter informações. Todos os outros campos nesta lista estão apenas procurando ações de insight de vendas para preencher o campo.
