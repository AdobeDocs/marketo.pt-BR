---
unique-page-id: 2953465
description: Sincronização SFDC - Converter um cliente potencial em um contato no Salesforce - Documentos do Marketing - Documentação do produto
title: Sincronização SFDC - Convertendo um cliente potencial em um contato no Salesforce
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Sincronização SFDC: Convertendo um cliente potencial em um contato no Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imaginem três cenários diferentes em Salesforce: (não está usando a etapa [de fluxo](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) Converter pessoa em Marketo)

1. Converter um cliente potencial em um **novo contato e uma nova conta**
1. Converter um cliente potencial em um **novo contato** em uma conta **existente**

1. Converter um cliente potencial para um contato **** existente em uma conta **** existente (isso funciona idêntico à [mesclagem](sfdc-sync-merging-a-lead-contact-person.md))

Em todos os três casos, você acaba com **1 contato e nenhum contato em Salesforce e 1 contato e nenhuma pessoa em Marketo.**

No Marketo, o registro agora terá um Tipo SFDC = Contato.

>[!TIP]
>
>Ao converter no Salesforce, verifique se seus campos personalizados [principais estão bem](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm)mapeados. Você não quer perder nenhum dado.

Você pode acionar e filtrar usando: &quot;O cliente potencial é convertido&quot; e &quot;o cliente potencial foi convertido.&quot;