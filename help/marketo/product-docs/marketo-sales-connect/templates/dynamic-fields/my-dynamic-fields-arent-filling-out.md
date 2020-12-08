---
unique-page-id: 14352602
description: Meus campos dinâmicos não estão preenchendo - Documentos do Marketing - Documentação do produto
title: Meus campos dinâmicos não estão preenchendo
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# Meus campos dinâmicos não estão preenchendo {#my-dynamic-fields-arent-filling-out}

Os campos dinâmicos só funcionarão quando você estiver usando um modelo. Os emails individuais únicos que você escreve não vão preenchê-los.

## O que verificar {#what-to-check}

Há três tipos de campos dinâmicos no Sales Connect: Básico, Personalizado e Salesforce. Básico e Personalizado parecem obter informações do aplicativo [da](http://toutapp.com/login)Web. Se as informações não existirem no aplicativo da Web, os campos ficarão em branco. Os campos do Salesforce extraem informações do [Salesforce.com](http://salesforce.com).

`**Troubleshooting Salesforce Fields**`

Campos do Salesforce: por exemplo, `{{sfdc_account_name}}`

* Verifique se ele está conectado corretamente ao Sales Connect. Vá para a página [Configurações](http://toutapp.com/next#settings) e clique em **Gerenciar** ao lado do CRM.

**Solução de problemas de campos básicos e personalizados**

Campos básicos de texto explicativo: por exemplo, `{{company}}`

Campos personalizados de tempo limite: por exemplo, `{{custom_field_favorite_movie}}`

* T `he corresponding field needs to be saved for your contact` na página [](http://toutapp.com/next#relationships) Pessoas para referência do nosso campo dinâmico. Por exemplo, se você estiver enviando um email para Mary e usando o `{{company}}` campo, mas o registro de contato dela não lista uma empresa, nós não seremos capazes de preencher isso.

## Por Que Meu Email Foi Enviado Sem Preencher Todos Os Campos Dinâmicos? {#why-did-my-email-send-without-populating-all-dynamic-fields}

O Sales Connect impedirá que seus e-mails sejam enviados se não for possível preencher todos os campos dinâmicos no e-mail. **No entanto**, existem algumas exceções a esta regra. Alguns campos enviarão um valor em branco ou preencherão automaticamente se for possível encontrar um. Esses campos e como eles reagirão se não conseguirem preencher os campos estão listados abaixo.

`{{first_name}}` = EM BRANCO

`{{last_name}}` =EM BRANCO

`{{title}}` = EM BRANCO

`{{company}}` = &quot;sua empresa&quot;

`{{friendly_company}}` = &quot;sua empresa&quot;

>[!NOTE]
>
>O `{{first_name}}` campo procurará no Sales Connect e no Salesforce para tentar obter informações. Todos os outros campos nesta lista estão apenas procurando no Sales Connect para preencher o campo.

