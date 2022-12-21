---
unique-page-id: 7514149
description: Exemplo de atribuição 3 - Documentação do Marketo - Documentação do produto
title: Exemplo de atribuição 3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 4%

---

# Exemplo de atribuição 3 {#attribution-example}

Leia o seguinte cenário e tente determinar os números que devem estar na grade.

* 11 de abril | Downloads de Steve (Conteúdo) - sucesso
* 22 de abril | A oportunidade é criada por US$ 3.000 (Steve e Jason têm papéis)
* 25 de abril | Jason participa (Webinar) - sucesso
* 30 de abril | Oportunidade fechada-vencedora

| Métrica de atribuição | (Conteúdo) | (Webinar) |
|---|---|---|
| (MT) Opção criada | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT) Planejamento criado | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Receita obtida | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**Mostrar respostas**

>[!NOTE]
>
>**Explicação**
>
>Lembre-se da regra de atribuição nº 3. Jason teve sucesso no programa APÓS a criação da propriedade. Portanto, o webinário não pode receber crédito pela criação da oportunidade. Apenas crédito para o Opty ganhou.
>
>Portanto, (Conteúdo) tem 100% do crédito pela criação e pipeline da Opção, mas apenas 50% do crédito pela opção venceu.

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
>* [Exemplo de atribuição 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

