---
unique-page-id: 14352592
description: Como inserir campos dinâmicos - Documentação do Marketo - Documentação do produto
title: Como inserir campos dinâmicos
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 4%

---

# Como inserir campos dinâmicos {#how-to-insert-dynamic-fields}

Permitimos que você personalize seus modelos de email com atributos predefinidos como `{{first_name}}` ou `{{company}}`. Esses campos permitem enviar um email para vários contatos e preencher automaticamente esses campos sem precisar digitá-los separadamente para cada contato.

>[!TIP]
>
>Os campos &quot;first_name&quot; e &quot;company&quot; são os únicos campos que serão exibidos para [!DNL Sales Connect] e [!DNL Salesforce]. Isso significa que, se um contato não existir no [aplicativo Web](https://toutapp.com/login), procuraremos em [!DNL Salesforce] se é possível encontrar um registro de contato/cliente potencial com um endereço de email correspondente. Em seguida, usamos as informações desse registro para preencher o campo.

## Inserir um campo dinâmico em um modelo {#insert-a-dynamic-field-into-a-template}

1. Em **[!UICONTROL Modelos e Campanhas]**, encontre o modelo que deseja editar e clique em **[!UICONTROL Editar Modelo]**.

1. Clique Em **[!UICONTROL Tout Campos Dinâmicos]**.

   >[!NOTE]
   >
   >Ao enviar por email contatos que existem no [!DNL Sales Connect], você pode usar os campos dinâmicos básicos. Eles extrairão diretamente do contato.

Se estiver enviando emails para contatos existentes no [!DNL Salesforce], você poderá aproveitar os campos dinâmicos do [!DNL Salesforce]. Todos eles começam com &quot;sfdc&quot;. Desde que você tenha uma conexão com [!DNL Salesforce], esses campos chamarão diretamente o cliente potencial/contato em [!DNL Salesforce] para preencher as informações no modelo.

## Inserir Campos Dinâmicos em uma Linha de Assunto {#insert-dynamic-fields-in-a-subject-line}

Basta copiá-los e colá-los manualmente no campo de assunto de um email, tomando cuidado para garantir que você tenha a formatação adequada.
