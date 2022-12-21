---
unique-page-id: 1147001
description: Usar a lógica de regra da Smart List padrão - Documentos do Marketo - Documentação do produto
title: Usando a Lógica de Regra de Smart List Padrão
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Usando a Lógica de Regra de Smart List Padrão {#using-standard-smart-list-rule-logic}

Você pode ter notado a opção &quot;Usar filtros&quot; ao criar listas inteligentes de campanha. Essa configuração permite decidir se os filtros precisam ser avaliados com um operador AND ou OR.

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>A alteração da lógica da regra da lista inteligente se aplica somente a filtros, **not** acionadores.

Os acionadores são sempre avaliados como OU, mesmo se a configuração acima estiver definida como TODOS.  Veja um exemplo:

![](assets/image2014-9-22-14-3a12-3a57.png)

A lista inteligente acima, em palavras:

```box
IF person fills out My Form
OR
IF person visits My Page 
AND 
Industry is Marketing 
AND 
Country is USA 
THEN follow the campaign's flow step(s)
```

Então, se uma pessoa preencher o formulário **ou** visita a página, a campanha avaliará essa pessoa com base em **all** ou **any** dos filtros subsequentes, dependendo da configuração usada.

>[!MORELIKETHIS]
>
>[Usando a Lógica de Regra de Smart List Avançada](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
