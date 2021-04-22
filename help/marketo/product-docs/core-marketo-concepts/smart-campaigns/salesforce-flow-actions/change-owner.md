---
unique-page-id: 1147021
description: Alterar proprietário - Documentos do Marketo - Documentação do produto
title: Alterar proprietário
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 2%

---

# Alterar proprietário {#change-owner}

Se você tiver pessoas já atribuídas a um proprietário, poderá usar essa etapa de fluxo para reatribuí-las a outro proprietário.

![](assets/image2014-9-22-15-3a1-3a3.png)

**Uso**

1. Basta escolher o proprietário ou a fila de lead para a qual deseja alterar e ir!

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >O Salesforce não permite que contatos sejam atribuídos a filas de lead. Para um registro que é um contato SFDC:
   >
   >1. O Marketo criará um lead duplicado **somente** quando o contato for sincronizado com o Salesforce. Em outras palavras, se você usar a etapa de fluxo **[Sincronizar pessoa com SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** com `AssignTo=<a lead queue>`, o Marketo criará um lead duplicado no Salesforce e o atribuirá à fila de lead.
      >
      >
   1. Se você tentar usar a etapa de fluxo **Alterar proprietário** em um contato, nenhuma duplicata será criada no Salesforce.


   >[!NOTE]
   >
   >Se o registro ainda não existir em sua conta do Salesforce, o sincronizaremos e o atribuiremos ao usuário selecionado.
