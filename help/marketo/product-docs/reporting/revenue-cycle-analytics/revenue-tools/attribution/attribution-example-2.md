---
unique-page-id: 7514146
description: Exemplo de atribuição 2 - Documentação do Marketo - Documentação do produto
title: Exemplo de atribuição 2
exl-id: 8f00abb5-85f8-4f05-874e-57aa6442548c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 6%

---

# Exemplo de atribuição 2 {#attribution-example}

Leia o seguinte cenário e tente determinar os números que devem estar na grade.

* 11 de abril | O projeto de lei é adquirido pela (Transmissão)
* 15 de abril | Joan é adquirida por (Webinar)
* 22 de abril | (Oportunidade 1) criada por US$ 6.000
* 24 de abril | (Oportunidade 2) criada por US$ 10.000
* 25 de abril | Bill e Joan estão associadas a funções para **AMBOS** Óptias
* 29 de abril | (Oportunidade 1) Está Fechada

| Nome do programa | (Evento comercial) | (Webinar) |
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
>Porque tanto Bill quanto Joan estavam associadas a funções para **AMBOS** oportunidades, o sistema (de acordo com as regras) divide o crédito uniformemente entre elas.
>
>O pipeline criado para cada programa (US$ 8.000) é metade do total (US$ 16.000) disponível para ser creditado.

>[!NOTE]
>
>**Regras de atribuição**
>
>1. O crédito é dividido uniformemente
>1. Você não pode dar mais crédito do que você ganhou
>1. Você não pode dar crédito por algo que aconteceu no passado


Tente todos os exemplos e você será um criador de atribuição!

>[!MORELIKETHIS]
>
>* [Exemplo de atribuição 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Exemplo de atribuição 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Exemplo de atribuição 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

