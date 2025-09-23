---
unique-page-id: 7514146
description: Exemplo 2 de atribuição - Documentação do Marketo - Documentação do produto
title: Atribuição - Exemplo 2
exl-id: 8f00abb5-85f8-4f05-874e-57aa6442548c
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 7%

---

# Atribuição - Exemplo 2 {#attribution-example}

Leia o cenário a seguir e tente determinar os números que devem estar na grade.

* Abril de 11 | O título é adquirido por (Tradeshow)
* Abril de 15 | Joan é adquirida pela (Webinar)
* Abril de 22 | (Oportunidade 1) criada por US$ 6.000
* Abril de 24 | (Oportunidade 2) criada por US$ 10.000
* Abril de 25 | Bill e Joan estão associados com as funções de **BOTH** Optys
* Abril de 29 | (Oportunidade 1) é Conquistado

| Nome do programa | (Feira) | (Webinário) |
|---|---|---|
| (FT) Opção criada | `<pre>1</pre>` | `<pre>1</pre>` |
| (FT) Planejamento criado | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT) Receita obtida | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**Mostrar respostas**

>[!NOTE]
>
>**Explicação**
>
>Como Bill e Joan foram associados com funções a **AMBOS** oportunidades, o sistema (de acordo com as regras) divide o crédito igualmente entre eles.
>
>Pipeline criado para cada programa (US$ 8 mil) é metade do total (US$ 16 mil) disponível para dar como crédito.

>[!NOTE]
>
>**Regras de atribuição**
>
>1. O crédito é dividido uniformemente
>1. Você não pode dar mais crédito do que ganhou
>1. Não dá crédito por algo que aconteceu no passado

Experimente todos os exemplos e você será um profissional de atribuição.

>[!MORELIKETHIS]
>
>* [Exemplo de atribuição 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Exemplo de atribuição 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Exemplo de atribuição 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
