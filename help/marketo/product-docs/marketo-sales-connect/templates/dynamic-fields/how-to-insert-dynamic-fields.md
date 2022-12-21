---
unique-page-id: 14352592
description: Como inserir campos dinâmicos - Documentos do Marketo - Documentação do produto
title: Como inserir campos dinâmicos
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Como inserir campos dinâmicos {#how-to-insert-dynamic-fields}

Nós permitimos que você personalize seus modelos de email com atributos predefinidos, como `{{first_name}}` ou `{{company}}`. Esses campos permitem enviar por email vários contatos e preencher automaticamente esses campos sem precisar digitar separadamente para cada contato.

>[!TIP]
>
>Os campos &quot;first_name&quot; e &quot;company&quot; são os únicos campos que irão procurar pelo Sales Connect e pelo Salesforce. Isso significa que se um contato não existir no [aplicação web](https://toutapp.com/login), buscamos no Salesforce para ver se podemos encontrar um registro de contato/lead com um endereço de email correspondente. Em seguida, usamos informações desse registro para preencher o campo.

## Inserir um campo dinâmico em um modelo {#insert-a-dynamic-field-into-a-template}

1. Em **Modelos e campanhas**, encontre o modelo que deseja editar e clique em **Editar modelo**.

1. Clique em **Campos dinâmicos de layout**.

   >[!NOTE]
   >
   >Ao enviar contatos por email existentes no Sales Connect, você pode usar os campos dinâmicos básicos. Eles se retirarão diretamente do contato.

Se você estiver enviando contatos por email existentes no Salesforce, poderá aproveitar os campos dinâmicos do Salesforce. Tudo começa com &quot;sfdc&quot;. Desde que tenha uma conexão com o Salesforce, esses campos chamarão diretamente o lead/contato no Salesforce para preencher informações no modelo.

## Inserir Campos Dinâmicos em uma Linha de Assunto {#insert-dynamic-fields-in-a-subject-line}

Basta copiar e colar manualmente no campo de assunto de um email, com cautela para garantir que você tenha a formatação correta.
