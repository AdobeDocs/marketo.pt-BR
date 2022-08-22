---
unique-page-id: 1147021
description: Alterar proprietário - Documentos do Marketo - Documentação do produto
title: Alterar proprietário
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
source-git-commit: 44c134811242b4136a3137cdd60e60edeb838c8c
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

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
   >1. A Marketo criará um lead duplicado **only** quando o contato é sincronizado com o Salesforce. Em outras palavras, se você usar a variável **[Sincronizar pessoa com o SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** passo de fluxo com `AssignTo=<a lead queue>`, a Marketo criará um lead duplicado no Salesforce e o atribuirá à fila de lead.
   >
   >1. Se você usar a variável **Alterar proprietário** Em uma etapa de fluxo em um contato, a Marketo cria um lead duplicado no Salesforce. Para evitar isso, use um filtro no campo &quot;Tipo SFDC&quot; que limita a ação somente aos leads.


   >[!NOTE]
   >
   >Se o registro ainda não existir em sua conta do Salesforce, o sincronizaremos e o atribuiremos ao usuário selecionado.
