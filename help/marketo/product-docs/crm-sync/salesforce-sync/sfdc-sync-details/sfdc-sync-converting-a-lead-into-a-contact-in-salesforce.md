---
unique-page-id: 2953465
description: Sincronização do SFDC - Converter um lead em um contato no Salesforce - Documentação do Marketo - Documentação do produto
title: Sincronização do SFDC - Convertendo um lead em um contato no Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Sincronização com o SFDC: Convertendo um cliente potencial em um contato no [!DNL Salesforce] {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imagine três cenários diferentes em [!DNL Salesforce]: (não usando a [etapa Converter fluxo de pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) no Marketo)

1. Convertendo um cliente em potencial em um **novo contato e nova conta**
1. Convertendo um cliente em potencial em um **novo contato** em uma **conta existente**

1. Convertendo um cliente potencial em um **contato existente** em uma **conta existente** (funciona de forma idêntica à [mesclagem](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"})

Nos três casos, você acaba com **1 contato e nenhum cliente potencial em [!DNL Salesforce] e 1 contato e nenhuma pessoa no Marketo.**

No Marketo, o registro agora terá um Tipo de SFDC = Contato.

>[!TIP]
>
>Ao converter em [!DNL Salesforce], certifique-se de que seus [campos personalizados de cliente potencial estejam bem mapeados](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). Você não quer perder nenhum dado.

Você pode acionar e filtrar usando: &quot;[!UICONTROL O lead foi convertido]&quot; e &quot;[!UICONTROL O lead foi convertido].&quot;
