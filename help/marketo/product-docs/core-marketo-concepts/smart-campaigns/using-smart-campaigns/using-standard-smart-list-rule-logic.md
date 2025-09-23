---
unique-page-id: 1147001
description: Utilização Da Lógica Padrão De Regras Da Smart List - Documentação Do Marketo - Documentação Do Produto
title: Uso da lógica de regra de lista inteligente padrão
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 9%

---

# Uso da lógica de regra de lista inteligente padrão {#using-standard-smart-list-rule-logic}

Você pode ter notado a opção &quot;Usar filtros&quot; ao criar Smart Lists do Campaign. Essa configuração permite decidir se os filtros precisam ser avaliados com um operador AND ou OR.

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>A alteração da lógica da regra de lista inteligente se aplica somente a filtros, _não_ acionadores.

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

Portanto, se uma pessoa preencher o formulário _ou_ visitar a página, a campanha avaliará essa pessoa com base em _todos_ ou _qualquer_ dos filtros subsequentes, dependendo da configuração usada.

>[!MORELIKETHIS]
>
>[Usando a Lógica de Regra Avançada da Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"}
