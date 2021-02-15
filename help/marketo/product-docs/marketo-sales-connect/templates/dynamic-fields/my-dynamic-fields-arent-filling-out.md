---
unique-page-id: 14352602
description: Meus campos dinâmicos não estão preenchendo - Documentos do Marketing - Documentação do produto
title: Meus campos dinâmicos não estão preenchendo
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---


# Meus campos dinâmicos não estão preenchendo {#my-dynamic-fields-arent-filling-out}

Os campos dinâmicos só funcionarão quando você estiver usando um modelo. Os emails individuais únicos que você escreve não vão preenchê-los.

## O que verificar {#what-to-check}

Há três tipos de campos dinâmicos no Sales Connect: Básico, Personalizado e Salesforce. Básico e Personalizado parecem obter informações do [aplicativo da Web](https://toutapp.com/login). Se as informações não existirem no aplicativo da Web, os campos ficarão em branco. Os campos do Salesforce extraem informações de [Salesforce.com](https://salesforce.com).

**Solução de problemas de campos do Salesforce**

Campos do Salesforce: por exemplo, `{{sfdc_account_name}}`

* Verifique se ele está conectado corretamente ao Sales Connect. Vá para a página [Configurações](https://toutapp.com/login) e clique em **Gerenciar** ao lado do CRM.

**Solução de problemas de campos básicos e personalizados**

Campos básicos de texto explicativo: por exemplo, `{{company}}`

Campos personalizados de tempo limite: por exemplo, `{{custom_field_favorite_movie}}`

* O campo correspondente precisa ser salvo para seu contato na [página de Pessoas](https://toutapp.com/next#relationships) para que nosso campo dinâmico faça referência. Por exemplo, se você estiver enviando um e-mail para Mary e usando o campo `{{company}}`, mas o registro de contato dela não lista uma empresa, nós não seremos capazes de preencher isso.

## Por Que Meu Email Foi Enviado Sem Preencher Todos Os Campos Dinâmicos? {#why-did-my-email-send-without-populating-all-dynamic-fields}

O Sales Connect impedirá que seus e-mails sejam enviados se não for possível preencher todos os campos dinâmicos no e-mail. **No entanto**, existem algumas exceções a esta regra. Alguns campos enviarão um valor em branco ou preencherão automaticamente se for possível encontrar um. Esses campos e como eles reagirão se não conseguirem preencher os campos estão listados abaixo.

`{{first_name}}` = EM BRANCO

`{{last_name}}` =EM BRANCO

`{{title}}` = EM BRANCO

`{{company}}` = &quot;sua empresa&quot;

`{{friendly_company}}` = &quot;sua empresa&quot;

>[!NOTE]
>
>O campo `{{first_name}}` observará o Sales Connect e o Salesforce para tentar obter informações. Todos os outros campos nesta lista estão apenas procurando no Sales Connect para preencher o campo.
