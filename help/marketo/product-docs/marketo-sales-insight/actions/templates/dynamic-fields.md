---
description: Campos dinâmicos - Documentação do Marketo - Documentação do produto
title: Campos dinâmicos
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
feature: Sales Insight Actions
source-git-commit: cffe7a8734f79f887f3aad017a16fad4f04cda74
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Campos dinâmicos {#dynamic-fields}

Permitimos que você personalize seus modelos de email com atributos predefinidos como `{{first_name}}` ou `{{company}}`. Esses campos permitem enviar um email para vários contatos e preencher automaticamente esses campos sem precisar digitá-los separadamente para cada contato.

>[!TIP]
>
>Os campos &quot;first_name&quot; e &quot;company&quot; são os únicos campos que analisarão as Ações do Sales Insight e o Salesforce. Isso significa que, se um contato não existir no [aplicativo Web](https://toutapp.com/login), procuraremos no Salesforce para ver se podemos encontrar um registro de contato/cliente potencial com um endereço de email correspondente. Em seguida, usamos as informações desse registro para preencher o campo.

## Inserir um campo dinâmico em um modelo {#insert-a-dynamic-field-into-a-template}

1. Em **Modelos e Campanhas**, encontre o modelo que deseja editar e clique em **Editar Modelo**.

1. Clique em **Inserir Campo Dinâmico**.

   >[!NOTE]
   >
   >Ao enviar e-mails para contatos existentes nas Ações do Sales Insight, é possível usar os campos dinâmicos básicos. Eles extrairão diretamente do contato.

Se estiver enviando emails para contatos existentes no Salesforce, você poderá aproveitar os campos dinâmicos do Salesforce. Todos eles começam com &quot;sfdc&quot;. Desde que você tenha uma conexão com o Salesforce, esses campos chamarão diretamente o cliente potencial/contato no Salesforce para preencher as informações no modelo.

## Inserir Campos Dinâmicos em uma Linha de Assunto {#insert-dynamic-fields-in-a-subject-line}

Basta copiá-los e colá-los manualmente no campo de assunto de um email, tomando cuidado para garantir que você tenha a formatação adequada.

## Valores padrão do campo dinâmico {#dynamic-field-default-values}

Ao adicionar campos dinâmicos a seus modelos de email, você pode adicionar um valor padrão para o qual o campo dinâmico resolverá se não houver outro valor disponível.

Para fazer isso, adicione &quot;|&quot; após o rótulo do campo dinâmico e, em seguida, adicione &quot;default:&quot; (ambos sem aspas). Em seguida, adicione o valor para o qual deseja que o campo resolva (entre aspas) se nenhum outro valor puder ser encontrado.

**Exemplo:**

`{{first name | default: "loyal customer"}}`

`{{sfdc_contact_account_name | default: "your company"}}`

## Glossário de campos dinâmicos {#dynamic-fields-glossary}

Ao criar um modelo em Ações do Sales Insight, sempre recomendamos a integração de campos dinâmicos, usando o botão **Inserir campo dinâmico**.

Esta ferramenta é usada para `auto-personalize your email` e poupar toneladas de tempo até `pulling information from the People page`.

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
* Ao usar o `{{company_friendly}}`, separe a Inc. ou a Co. com uma vírgula nos detalhes de contato. É assim que as Ações de Insight de vendas sabem o que remover ao obter o valor.
* Permitimos que você personalize seus modelos de email com atributos predefinidos como `{{my_name}}` ou `{{my_title}}`. Esses campos permitem que você faça referência a si mesmo rapidamente nos modelos de email.
* O sistema anexa automaticamente a assinatura do usuário a cada email enviado. Se o usuário estiver usando um modelo com o campo dinâmico `{{my_signature}}`, o sistema preencherá a assinatura onde o campo dinâmico `{{my_signature}}` foi colocado. Ele só é adicionado lá para evitar duplicação. O sistema tratará `{{team_unsubscribe}}` da mesma maneira quando a configuração global de cancelamento de inscrição de acréscimo estiver habilitada.

>[!TIP]
>
>Se os campos dinâmicos não estiverem sendo preenchidos, confira [este artigo](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
