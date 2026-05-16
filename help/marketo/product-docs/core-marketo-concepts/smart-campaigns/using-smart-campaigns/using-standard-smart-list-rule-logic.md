---
unique-page-id: 1147001
description: Saiba como usar a lógica padrão da regra de Smart List em uma Campanha inteligente. Combine filtros com lógica AND para qualificação.
title: Uso da lógica de regra de lista inteligente padrão
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/hRPdzjEUOeC2PZK2YlO1IPZOPoPOfo7CHJu2yUtU0qc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 138
ht-degree: 10%

---

# Uso da lógica de regra de lista inteligente padrão {#using-standard-smart-list-rule-logic}

Você pode ter notado a opção &quot;Usar filtros&quot; ao criar Smart Lists do Campaign. Essa configuração permite decidir se os filtros precisam ser avaliados com um operador AND ou OR.

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>A alteração da lógica da regra de lista inteligente se aplica somente a filtros, _não_ acionadores.

Os acionadores são sempre avaliados como OU, mesmo se a configuração acima estiver definida como ALL. Por exemplo:

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
