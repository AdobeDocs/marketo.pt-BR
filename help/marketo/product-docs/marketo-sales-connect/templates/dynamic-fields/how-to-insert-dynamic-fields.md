---
unique-page-id: 14352592
description: Saiba como inserir campos dinâmicos em modelos do Sales Connect. Adicione o nome, a empresa e outros campos de mesclagem no editor de modelo.
title: Como inserir campos dinâmicos
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/WwKaorfXBu5Ah9wD6pXf5U4YzlpP9MoUMg-TtDzXDRo
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 246
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

Se você estiver enviando emails para contatos existentes no [!DNL Salesforce], poderá aproveitar os campos dinâmicos do [!DNL Salesforce]. Todos eles começam com &quot;sfdc&quot;. Desde que você tenha uma conexão com [!DNL Salesforce], esses campos chamarão diretamente o cliente potencial/contato em [!DNL Salesforce] para preencher as informações no modelo.

## Inserir Campos Dinâmicos em uma Linha de Assunto {#insert-dynamic-fields-in-a-subject-line}

Basta copiá-los e colá-los manualmente no campo de assunto de um email, tomando cuidado para garantir que você tenha a formatação adequada.
