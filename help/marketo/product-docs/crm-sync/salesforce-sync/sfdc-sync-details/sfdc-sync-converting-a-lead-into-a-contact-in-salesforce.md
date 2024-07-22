---
unique-page-id: 2953465
description: Sincronização do SFDC - Conversão de um lead em um contato no Salesforce - Documentação do Marketo - Documentação do produto
title: Sincronização do SFDC - Convertendo um lead em um contato no Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---

# Sincronização do SFDC: Convertendo um lead em um contato no Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imagine três cenários diferentes no Salesforce: (não usar a [etapa Converter fluxo de pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} no Marketo Engage)

1. Convertendo um cliente em potencial em um **novo contato e nova conta**
1. Convertendo um cliente em potencial em um **novo contato** em uma **conta existente**

1. Convertendo um cliente potencial em um **contato existente** em uma **conta existente** (funciona de forma idêntica à [mesclagem](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"})

Nos três casos, você tem **1 contato e nenhum cliente em potencial no Salesforce e 1 contato e nenhuma pessoa no Marketo.**

No Marketo, o registro agora terá um SFDC Type = Contact.

>[!TIP]
>
>Ao converter no Salesforce, certifique-se de que seus [campos personalizados de cliente potencial estejam bem mapeados](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm){target="_blank"}. Você não quer perder nenhum dado.

Você pode acionar e filtrar usando: &quot;O lead é convertido&quot; e &quot;O lead foi convertido&quot;.
