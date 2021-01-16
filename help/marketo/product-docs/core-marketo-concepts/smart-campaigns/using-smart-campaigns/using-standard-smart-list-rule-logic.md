---
unique-page-id: 1147001
description: Usando a lógica padrão da regra de Lista inteligente - Documentos do Marketing - Documentação do produto
title: Usando a lógica da regra de Lista inteligente padrão
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---


# Usando a lógica da regra de Lista inteligente padrão {#using-standard-smart-list-rule-logic}

Você pode ter notado a opção &quot;Usar filtros&quot; ao criar listas inteligentes de campanha. Essa configuração permite que você decida se os filtros precisam ser avaliados com um operador E ou OU.

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>A alteração da lógica da regra de lista inteligente só se aplica a filtros, **e não** acionadores.

Os acionadores são sempre avaliados como OU mesmo se a configuração acima estiver definida como ALL.  Veja um exemplo:

![](assets/image2014-9-22-14-3a12-3a57.png)

A lista inteligente acima em palavras:

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

Portanto, se uma pessoa preencher o formulário **ou** visitar a página, a campanha avaliará essa pessoa com base em **all** ou **qualquer** dos filtros subsequentes, dependendo da configuração usada.

>[!MORELIKETHIS]
>
>[Usando a lógica avançada da regra de Lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
