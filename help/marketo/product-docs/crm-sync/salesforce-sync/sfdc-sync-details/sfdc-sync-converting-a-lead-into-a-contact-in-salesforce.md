---
unique-page-id: 2953465
description: Sincronização do SFDC - Conversão de um lead em um contato no Salesforce - Documentação do Marketo - Documentação do produto
title: Sincronização do SFDC - Convertendo um lead em um contato no Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---

# Sincronização do SFDC: Convertendo um lead em um contato no Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imagine três cenários diferentes no Salesforce: (sem usar o [Etapa Converter fluxo de pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} in Marketo Engage)

1. Conversão de um lead em um **novo contato e nova conta**
1. Conversão de um lead em um **novo contato** em um **conta existente**

1. Conversão de um lead em um **contato existente** em um **conta existente** (isso funciona de forma idêntica a [mesclagem](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"})

Nos três casos você acaba tendo **1 contato e nenhum cliente potencial no Salesforce e 1 contato e nenhuma pessoa no Marketo.**

No Marketo, o registro agora terá um SFDC Type = Contact.

>[!TIP]
>
>Ao converter no Salesforce, verifique se [os campos personalizados principais são bem mapeados](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm){target="_blank"}. Você não quer perder nenhum dado.

Você pode acionar e filtrar usando: &quot;O lead é convertido&quot; e &quot;O lead foi convertido&quot;.
