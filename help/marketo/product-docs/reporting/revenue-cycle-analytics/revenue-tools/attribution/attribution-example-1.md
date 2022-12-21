---
unique-page-id: 7514126
description: Exemplo de atribuição 1 - Documentação do Marketo - Documentação do produto
title: Exemplo de atribuição 1
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 5%

---

# Exemplo de atribuição 1 {#attribution-example}

Leia o seguinte cenário e tente determinar os números que devem estar na grade.

* 11 de abril | Fred é adquirido pela (feira)
* 15 de abril | Participantes da Margo (Webinar) - sucesso
* 22 de abril | Fred está associado (papel) à oportunidade
* 22 de abril | A oportunidade é criada por US$ 3.000

| Nome do programa | (Evento comercial) | (Webinar) |
|---|---|---|
| (FT) Opção criada | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT) Planejamento criado | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT) Opty Won | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT) Receita obtida | `<pre>0</pre>` | `<pre>0</pre>` |

**Mostrar respostas**

>[!NOTE]
>
>**Explicação**
>
>O primeiro é entender que alguns tipos são CONTAGENS e outros são MOEDA. A opção Criada é uma contagem, um número inteiro. O pipeline é uma moeda. No Marketo, a moeda estará em conformidade com as configurações de local do administrador.
>
>A razão pela qual a feira recebeu todo o crédito foi porque a Margo não estava associada a um papel na oportunidade. Sem função, sem crédito.

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
>* [Exemplo de atribuição 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Exemplo de atribuição 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Exemplo de atribuição 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

