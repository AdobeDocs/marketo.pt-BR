---
unique-page-id: 1147001
description: Utilização Da Lógica Padrão De Regras Da Smart List - Documentação Do Marketo - Documentação Do Produto
title: Utilização da Lógica Padrão de Regras de Smart List
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 3916413a90e52a3423a8d7f78ad1c9eb45c2a219
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Utilização da Lógica Padrão de Regras de Smart List {#using-standard-smart-list-rule-logic}

Você pode ter notado a opção &quot;Usar filtros&quot; ao criar Smart Lists do Campaign. Essa configuração permite decidir se os filtros precisam ser avaliados com um operador AND ou OR.

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>A alteração da lógica da regra da lista inteligente se aplica somente a filtros, **não** acionadores.

Os acionadores são sempre avaliados como OU, mesmo se a configuração acima estiver definida como ALL. Veja um exemplo:

![](assets/using-standard-smart-list-rule-logic-2.png)

A lista inteligente acima em palavras:

```box
IF person fills out Great Form
OR
IF person visits Keith's Landing Page 
AND 
Industry is Energy 
AND 
Country is US 
THEN follow the campaign's flow step(s)
```

Então, se uma pessoa preenche o formulário **ou** visita a página, a campanha avaliará essa pessoa com base em **all** ou **qualquer** dos filtros subsequentes, dependendo da configuração usada.

>[!MORELIKETHIS]
>
>[Utilização da Lógica de Regra Avançada da Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
