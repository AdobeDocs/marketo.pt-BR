---
description: Campos dinâmicos - Documentos do Marketo - Documentação do produto
title: Campos dinâmicos
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Campos dinâmicos {#dynamic-fields}

Nós permitimos que você personalize seus modelos de email com atributos predefinidos, como `{{first_name}}` ou `{{company}}`. Esses campos permitem enviar por email vários contatos e preencher automaticamente esses campos sem precisar digitar separadamente para cada contato.

>[!TIP]
>
>Os campos &quot;first_name&quot; e &quot;company&quot; são os únicos campos que irão procurar pelas Ações de Insight de Vendas e pelo Salesforce. Isso significa que se um contato não existir no [aplicação web](https://toutapp.com/login), buscamos no Salesforce para ver se podemos encontrar um registro de contato/lead com um endereço de email correspondente. Em seguida, usamos informações desse registro para preencher o campo.

## Inserir um campo dinâmico em um modelo {#insert-a-dynamic-field-into-a-template}

1. Em **Modelos e campanhas**, encontre o modelo que deseja editar e clique em **Editar modelo**.

1. Clique em **Inserir campo dinâmico**.

   >[!NOTE]
   >
   >Ao enviar contatos por email existentes em Ações de informações de vendas, você pode usar os campos dinâmicos básicos. Eles se retirarão diretamente do contato.

Se você estiver enviando contatos por email existentes no Salesforce, poderá aproveitar os campos dinâmicos do Salesforce. Tudo começa com &quot;sfdc&quot;. Desde que tenha uma conexão com o Salesforce, esses campos chamarão diretamente o lead/contato no Salesforce para preencher informações no modelo.

## Inserir Campos Dinâmicos em uma Linha de Assunto {#insert-dynamic-fields-in-a-subject-line}

Basta copiar e colar manualmente no campo de assunto de um email, com cautela para garantir que você tenha a formatação correta.

## Glossário de campos dinâmicos {#dynamic-fields-glossary}

Ao criar um modelo em Ações de insight de vendas, sempre recomendamos integrar campos dinâmicos usando o **Inserir campo dinâmico** botão.

Esta ferramenta é usada para `auto-personalize your email` e economize toneladas de tempo `pulling information from the People page`.

| Campo dinâmico | Exemplo do que aparece no email |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Se você não quiser ouvir de mim novamente, por favor, me informe aqui |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Escritor Técnico Sênior |
| `{{work_website}}` | https://www.marketo.com |

**O que registrar**:

* Se as informações de um contato forem inseridas incorretamente ou estiverem ausentes na página Pessoas, elas não serão inseridas corretamente no modelo.
* A diferença entre `{{company}}` e `{{company_friendly}}` é que `{{company_friendly}}` removerá qualquer título formal, como Inc., LLC. etc., do nome da empresa do seu contato.
* Ao usar `{{company_friendly}}`, certifique-se de separar Inc. ou Co. por uma vírgula nos detalhes do contato. É assim que as ações de insight de vendas sabem o que remover ao obter o valor.
* Nós permitimos que você personalize seus modelos de email com atributos predefinidos, como `{{my_name}}` ou `{{my_title}}`. Esses campos permitem que você faça referência a si mesmo rapidamente em seus modelos de email.

>[!TIP]
>
>Se os campos dinâmicos não estiverem sendo preenchidos, confira [este artigo](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
