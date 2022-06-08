---
unique-page-id: 2953465
description: Sincronização SFDC - Converter um lead em um contato no Salesforce - Documentos da Marketo - Documentação do produto
title: Sincronização SFDC - Convertendo um lead em um contato no Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Sincronização SFDC: Conversão de um lead em um contato no Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imagine três cenários diferentes em Salesforce: (não usar a variável [Etapa de fluxo Converter pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) no Marketo)

1. Conversão de um lead em um **novo contato e nova conta**
1. Conversão de um lead em um **novo contato** em um **conta existente**

1. Conversão de um lead para um **contato existente** em um **conta existente** (funciona de forma idêntica ao [mesclagem](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

Em todos os três casos, você acaba com **1 contato e nenhum cliente potencial em Salesforce e 1 contato e nenhuma pessoa no Marketo.**

No Marketo, o registro agora terá um Tipo SFDC = Contato.

>[!TIP]
>
>Ao converter no Salesforce, verifique se [campos personalizados de lead são bem mapeados](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). Você não quer perder dados.

Você pode acionar e filtrar usando: &quot;O lead é convertido&quot; e &quot;O lead foi convertido.&quot;
