---
unique-page-id: 14352592
description: Como inserir campos dinâmicos - Documentação do Marketo - Documentação do produto
title: Como inserir campos dinâmicos
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---

# Como inserir campos dinâmicos {#how-to-insert-dynamic-fields}

Permitimos que você personalize seus modelos de email com atributos predefinidos como `{{first_name}}` ou `{{company}}`. Esses campos permitem enviar um email para vários contatos e preencher automaticamente esses campos sem precisar digitá-los separadamente para cada contato.

>[!TIP]
>
>Os campos &quot;first_name&quot; e &quot;company&quot; são os únicos campos que serão exibidos para o Sales Connect e o Salesforce. Isso significa que, se um contato não existir no [aplicativo Web](https://toutapp.com/login), procuraremos no Salesforce para ver se podemos encontrar um registro de contato/cliente potencial com um endereço de email correspondente. Em seguida, usamos as informações desse registro para preencher o campo.

## Inserir um campo dinâmico em um modelo {#insert-a-dynamic-field-into-a-template}

1. Em **Modelos e Campanhas**, encontre o modelo que deseja editar e clique em **Editar Modelo**.

1. Clique Em **Tout Campos Dinâmicos**.

   >[!NOTE]
   >
   >Ao enviar contatos por email que existem no Sales Connect, você pode usar os campos dinâmicos básicos. Eles extrairão diretamente do contato.

Se estiver enviando emails para contatos existentes no Salesforce, você poderá aproveitar os campos dinâmicos do Salesforce. Todos eles começam com &quot;sfdc&quot;. Desde que você tenha uma conexão com o Salesforce, esses campos chamarão diretamente o cliente potencial/contato no Salesforce para preencher as informações no modelo.

## Inserir Campos Dinâmicos em uma Linha de Assunto {#insert-dynamic-fields-in-a-subject-line}

Basta copiá-los e colá-los manualmente no campo de assunto de um email, tomando cuidado para garantir que você tenha a formatação adequada.
