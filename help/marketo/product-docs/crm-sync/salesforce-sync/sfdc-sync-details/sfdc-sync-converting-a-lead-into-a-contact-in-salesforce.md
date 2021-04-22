---
unique-page-id: 2953465
description: Sincronização SFDC - Converter um lead em um contato no Salesforce - Documentos da Marketo - Documentação do produto
title: Sincronização SFDC -Converter um lead em um contato no Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Sincronização SFDC: Converter um lead em um contato no Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imagine três cenários diferentes em Salesforce: (não usando a etapa [Converter fluxo de pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) no Marketo)

1. Converter um cliente potencial em **novo contato e nova conta**
1. Converter um lead em um **novo contato** em uma **conta existente**

1. Converter um lead para um **contato existente** em uma **conta existente** (isso funciona idêntico a [mesclar](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

Em todos os três casos, você acaba com **1 contato e nenhum lead no Salesforce e 1 contato e nenhuma pessoa no Marketo.**

No Marketo, o registro agora terá um Tipo SFDC = Contato.

>[!TIP]
>
>Ao converter no Salesforce, verifique se os campos personalizados de [lead estão mapeados bem](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). Você não quer perder dados.

Você pode acionar e filtrar usando: &quot;O lead é convertido&quot; e &quot;O lead foi convertido.&quot;
