---
unique-page-id: 1147021
description: Saiba como alterar o proprietário do Salesforce em uma etapa de fluxo. Atribua um novo cliente potencial ou proprietário de contato quando as pessoas entrarem no fluxo.
title: Alterar proprietário
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
TQID: 'https://experienceleague.adobe.com/VU0fT4giNqfkF5g15q0IGIh8XuO2505nz89UuUfqZro'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 2%
---
# Alterar proprietário {#change-owner}

Se você tiver pessoas existentes que já estejam atribuídas a um proprietário, poderá usar essa etapa do fluxo para reatribuí-las a outro proprietário.

![](assets/change-owner-1.png)

1. Basta escolher o proprietário ou a fila de clientes potenciais para a qual deseja mudar e ir embora!

   ![](assets/change-owner-2.png)

   >[!CAUTION]
   >
   >[!DNL Salesforce] não permite que contatos sejam atribuídos a filas de clientes potenciais. Para um registro que é um contato da SFDC:
   >
   >* O Marketo criará um cliente em potencial duplicado **only** quando o contato for sincronizado com o Salesforce. Em outras palavras, se você usar a etapa de fluxo **[Sincronizar pessoa com o SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** com `AssignTo=<a lead queue>`, o Marketo criará um cliente potencial duplicado no Salesforce e o atribuirá à fila de clientes potenciais.
   >
   >* Se você usar a etapa de fluxo **[!UICONTROL Alterar Proprietário]** em um contato, a Marketo criará um cliente potencial duplicado no Salesforce. Para evitar isso, use um filtro no campo &quot;Tipo de SFDC&quot; que limite a ação somente a clientes potenciais.

   >[!NOTE]
   >
   >Se o registro ainda não existir em sua conta do [!DNL Salesforce], nós o sincronizaremos e o atribuiremos ao usuário selecionado.
