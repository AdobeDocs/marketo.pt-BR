---
unique-page-id: 14352602
description: Meus campos dinâmicos não estão sendo preenchidos - Documentação do Marketo - Documentação do produto
title: Meus campos dinâmicos não estão sendo preenchidos
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 4%

---

# Meus campos dinâmicos não estão sendo preenchidos {#my-dynamic-fields-arent-filling-out}

Os campos dinâmicos só funcionarão quando você estiver usando um modelo. Emails únicos individuais que você escreve não vão preencher isso.

## O que verificar {#what-to-check}

Há três tipos de campos dinâmicos em [!DNL Sales Connect]: Básico, Personalizado e [!DNL Salesforce]. Básico e Personalizado, ambos procuram obter informações do [aplicativo Web](https://toutapp.com/login). Se as informações não existirem no aplicativo web, os campos estarão em branco. Os campos [!DNL Salesforce] extraem informações do [Salesforce.com](https://salesforce.com).

**Solução de problemas de [!DNL Salesforce] Campos**

[!DNL Salesforce] Campos: ex.: `{{sfdc_account_name}}`

* Verifique se ele está conectado corretamente a [!DNL Sales Connect]. Vá para a página [Configurações](https://toutapp.com/login) e clique em **[!UICONTROL Gerenciar]** ao lado do seu CRM.

**Solução de problemas de campos básicos e personalizados**

Campos Básicos de Tout: ex.: `{{company}}`

Tout de Campos Personalizados: ex.: `{{custom_field_favorite_movie}}`

* O campo correspondente precisa ser salvo para o seu contato na [página Pessoas](https://toutapp.com/next#relationships) para que o nosso campo dinâmico faça referência. Por exemplo, se você estiver enviando um email para Mary e estiver usando o campo `{{company}}`, mas o registro de contato dela não listar uma empresa, não poderemos preenchê-lo.

## Por Que Meu Email Foi Enviado Sem Preencher Todos Os Campos Dinâmicos? {#why-did-my-email-send-without-populating-all-dynamic-fields}

O [!DNL Sales Connect] impedirá que seus emails sejam enviados se não for possível preencher todos os campos dinâmicos no email. **No entanto**, há algumas exceções a esta regra. Alguns campos enviarão um valor em branco ou preencherão automaticamente se for possível encontrar um. Esses campos e como eles reagirão se não puderem preencher o campo estão listados abaixo.

`{{first_name}}` = EM BRANCO

`{{last_name}}` =EM BRANCO

`{{title}}` = EM BRANCO

`{{company}}` = &quot;sua empresa&quot;

`{{friendly_company}}` = &quot;sua empresa&quot;

>[!NOTE]
>
>O campo `{{first_name}}` procurará [!DNL Sales Connect] e [!DNL Salesforce] para tentar obter informações. Todos os outros campos desta lista só estão procurando em [!DNL Sales Connect] para preencher o campo.
