---
unique-page-id: 7514151
description: Saiba mais sobre o exemplo de atribuição 4 no Marketo Engage, incluindo o exemplo de atribuição 4 exemplo de atribuição. Use este guia para concluir a próxima etapa.
title: Atribuição - Exemplo 4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
feature: Reporting, Revenue Cycle Analytics
source-git-commit: f6893edbfe85d1d6e0958b5a3029d8fd404b1311
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 6%

---

# Atribuição - Exemplo 4 {#attribution-example}

Leia o cenário a seguir e tente determinar os números que devem estar na grade.

* 11 de abril | Michelle baixa e-Book (Conteúdo) - Sucesso
* 15 de abril | John participa (webinário) - Sucesso
* 22 de abril | (Oportunidade 1) criada por US$ 3.000
* 24 de abril | (Oportunidade 2) criada por US$ 5.000
* 25 de abril | John e Michelle estão associados a **ambos** opções
* 29 de abril | [A opção 1] está fechada

| Nome do programa | (Conteúdo) | (Webinário) | | |
|---|---|---|---|---|
|   | (Opção 1) | (Opção 2) | (Opção 1) | (Opção 2) |
| (MT) Opção criada | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Planejamento criado | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT) Receita obtida | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**Mostrar respostas**

>[!NOTE]
>
>**Explicação**
>
>Quando você tem várias oportunidades e várias pessoas com sucesso no programa, você precisa dividir o crédito entre as pessoas e os programas. No entanto, observe que o crédito para a oportunidade 1 e 2 não é combinado. Cada uma é uma avaliação de crédito distinta.
>
>Quando muitas pessoas estiverem envolvidas, o Marketo calculará automaticamente as frações de uma oportunidade para dar crédito.

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
>* [Exemplo de atribuição 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Exemplo de atribuição 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
