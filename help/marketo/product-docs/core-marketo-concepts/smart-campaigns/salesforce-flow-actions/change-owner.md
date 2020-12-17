---
unique-page-id: 1147021
description: Alterar proprietário - Documentos do Marketing - Documentação do produto
title: Alterar proprietário
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# Alterar proprietário {#change-owner}

Se você tiver pessoas já atribuídas a um proprietário, poderá usar essa etapa de fluxo para atribuí-las novamente a outro proprietário.

![](assets/image2014-9-22-15-3a1-3a3.png)

**Uso**

1. Basta escolher o proprietário ou a fila de cliente potencial para a qual deseja mudar e ir!

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >O Salesforce não permite que contatos sejam atribuídos a filas de cliente potencial. Para um registro que seja um contato com a SFDC:
   >
   >1. O Marketo criará um cliente potencial de duplicado **only** quando o contato for sincronizado com o Salesforce. Em outras palavras, se você usar a etapa de fluxo **[Sincronizar Pessoa com SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** com `AssignTo=<a lead queue>`, o Marketo criará um cliente potencial de duplicado no Salesforce e o atribuirá à fila de cliente potencial.
      >
      >
   2. Se você tentar usar a etapa de fluxo **Alterar proprietário** em um contato, nenhum duplicado será criado no Salesforce.


   >[!NOTE]
   >
   >Se o registro ainda não existir em sua conta do Salesforce, ele será sincronizado e, em seguida, atribuído ao usuário selecionado.
