---
unique-page-id: 14352602
description: Meus campos dinâmicos não estão sendo preenchidos - Documentação do Marketo - Documentação do produto
title: Meus Campos Dinâmicos Não Estão Sendo Preenchidos
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Meus Campos Dinâmicos Não Estão Sendo Preenchidos {#my-dynamic-fields-arent-filling-out}

Os campos dinâmicos só funcionarão quando você estiver usando um modelo. Emails únicos individuais que você escreve não vão preencher isso.

## O que verificar {#what-to-check}

Há três tipos de campos dinâmicos no Sales Connect: Básico, Personalizado e Salesforce. Básico e Personalizado, ambos procuram obter informações do [aplicativo Web](https://toutapp.com/login). Se as informações não existirem no aplicativo web, os campos estarão em branco. Os campos do Salesforce extraem informações do [Salesforce.com](https://salesforce.com).

**Solução de problemas de campos do Salesforce**

Campos do Salesforce: ex.: `{{sfdc_account_name}}`

* Verifique se ele está conectado corretamente ao Sales Connect. Vá para a página [Configurações](https://toutapp.com/login) e clique em **Gerenciar** ao lado do seu CRM.

**Solução de problemas de campos básicos e personalizados**

Campos Básicos de Tout: ex.: `{{company}}`

Tout de Campos Personalizados: ex.: `{{custom_field_favorite_movie}}`

* O campo correspondente precisa ser salvo para o seu contato na [página Pessoas](https://toutapp.com/next#relationships) para que o nosso campo dinâmico faça referência. Por exemplo, se você estiver enviando um email para Mary e estiver usando o campo `{{company}}`, mas o registro de contato dela não listar uma empresa, não poderemos preenchê-lo.

## Por Que Meu Email Foi Enviado Sem Preencher Todos Os Campos Dinâmicos? {#why-did-my-email-send-without-populating-all-dynamic-fields}

O Sales Connect impedirá que seus emails sejam enviados se não for possível preencher todos os campos dinâmicos no email. **No entanto**, há algumas exceções a esta regra. Alguns campos enviarão um valor em branco ou preencherão automaticamente se for possível encontrar um. Esses campos e como eles reagirão se não puderem preencher o campo estão listados abaixo.

`{{first_name}}` = EM BRANCO

`{{last_name}}` =EM BRANCO

`{{title}}` = EM BRANCO

`{{company}}` = &quot;sua empresa&quot;

`{{friendly_company}}` = &quot;sua empresa&quot;

>[!NOTE]
>
>O campo `{{first_name}}` procurará tanto no Sales Connect quanto no Salesforce para tentar obter informações. Todos os outros campos desta lista só estão procurando no Sales Connect para preencher o campo.
