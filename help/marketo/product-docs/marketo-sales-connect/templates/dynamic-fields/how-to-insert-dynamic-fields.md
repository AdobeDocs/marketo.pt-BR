---
unique-page-id: 14352592
description: Como inserir campos dinâmicos - Documentos do Marketing - Documentação do produto
title: Como inserir campos dinâmicos
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# Como inserir campos dinâmicos {#how-to-insert-dynamic-fields}

Nós permitimos que você personalize seus modelos de e-mail com atributos predefinidos, como `{{first_name}}` ou `{{company}}`. Esses campos permitem que você envie vários contatos por email e preencha automaticamente esses campos sem precisar digitar separadamente para cada contato.

>[!TIP]
>
>Os campos &quot;first_name&quot; e &quot;empresa&quot; são o `only fields that will look to both Sales Connect and Salesforce.` que significa que, se um contato não existir no aplicativo [](http://toutapp.com/login)Web, procuramos no Salesforce para ver se conseguimos encontrar um contato/registro de cliente potencial com um endereço de email correspondente. Em seguida, usamos informações desse registro para preencher o campo.

## Inserir um campo dinâmico em um modelo {#insert-a-dynamic-field-into-a-template}

1. Em **Modelos e Campanhas**, localize o modelo que deseja editar e clique em **Editar modelo**.
1. Clique em Campos dinâmicos **de flutuação**.

   >[!NOTE]
   >
   >Ao enviar contatos por email que existem no Sales Connect, você pode usar os campos dinâmicos básicos. Eles sairão diretamente do contato.

Se você enviar contatos por email existentes no Salesforce, poderá aproveitar os campos dinâmicos do Salesforce. Tudo começa com &quot;sfdc&quot;. Desde que você tenha uma conexão com o Salesforce, esses campos chamarão diretamente para o cliente potencial/contato no Salesforce para preencher informações no modelo.

## Inserir campos dinâmicos em uma linha de assunto {#insert-dynamic-fields-in-a-subject-line}

Basta copiá-los e colá-los manualmente no campo de assunto de um email, tomando cuidado para garantir que você tenha a formatação correta.
