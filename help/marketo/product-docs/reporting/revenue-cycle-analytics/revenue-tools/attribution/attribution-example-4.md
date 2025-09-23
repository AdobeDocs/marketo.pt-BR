---
unique-page-id: 7514151
description: Exemplo 4 de atribuição - Documentação do Marketo - Documentação do produto
title: Atribuição - Exemplo 4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 6%

---

# Atribuição - Exemplo 4 {#attribution-example}

Leia o cenário a seguir e tente determinar os números que devem estar na grade.

* Abril de 11 | Michelle baixa e-Book (Conteúdo) - Sucesso
* Abril de 15 | John comparece (webinário) - Sucesso
* Abril de 22 | (Oportunidade 1) criada por US$ 3.000
* Abril de 24 | (Oportunidade 2) criada por US$ 5.000
* Abril de 25 | John e Michelle estão associados a **ambos** opções
* Abril de 29 | [A opção 1] está fechada

| Nome do programa | (Conteúdo) | (Webinário) |
|---|---|---|
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
