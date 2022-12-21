---
unique-page-id: 7514151
description: Exemplo de atribuição 4 - Documentação do Marketo - Documentação do produto
title: Exemplo de atribuição 4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 5%

---

# Exemplo de atribuição 4 {#attribution-example}

Leia o seguinte cenário e tente determinar os números que devem estar na grade.

* 11 de abril | Michelle baixa eBook (Conteúdo) - Êxito
* 15 de abril | Participantes do John (Webinar) - Êxito
* 22 de abril | (Oportunidade 1) criada por US$ 3.000
* 24 de abril | (Oportunidade 2) criada por US$ 5.000
* 25 de abril | John e Michelle estão associados a **both** Óptias
* 29 de abril | [Opção 1] is Closed-Won

| Nome do programa | (Conteúdo) | (Webinar) |
|---|---|---|
|  | (Opção 1) | (Opção 2) | (Opção 1) | (Opção 2) |
| (MT) Opção criada | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Planejamento criado | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT) Receita obtida | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**Mostrar respostas**

>[!NOTE]
>
>**Explicação**
>
>Quando você tem várias oportunidades e várias pessoas com sucesso no programa, você precisa dividir o crédito entre as pessoas e os programas. Contudo, é de notar que o crédito relativo à oportunidade 1 e 2 não é combinado. Cada uma é uma avaliação de crédito distinta.
>
>Quando muitas pessoas estiverem envolvidas, a Marketo calculará automaticamente as frações de uma oportunidade para dar crédito.

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
>* [Exemplo de atribuição 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Exemplo de atribuição 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)

