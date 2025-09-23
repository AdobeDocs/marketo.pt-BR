---
unique-page-id: 7514149
description: Exemplo 3 de atribuição - Documentação do Marketo - Documentação do produto
title: Atribuição - Exemplo 3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 6%

---

# Atribuição - Exemplo 3 {#attribution-example}

Leia o cenário a seguir e tente determinar os números que devem estar na grade.

* Abril de 11 | Downloads do Steve (Conteúdo) - sucesso
* Abril de 22 | A oportunidade é criada por US$ 3 mil (Steve e Jason têm funções)
* Abril de 25 | Jason participa (webinário) - sucesso
* 30 de abril | A oportunidade foi fechada

| Métrica de atribuição | (Conteúdo) | (Webinário) |
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
>Lembrar regra de atribuição #3. Jason teve sucesso no programa DEPOIS que a propriedade foi criada. Portanto, o webinário não pode receber crédito pela criação da oportunidade. Só crédito pelo Opty ganhou.
>
>Portanto, (Conteúdo) tem 100% de crédito para a criação e o pipeline de opções, mas apenas 50% de crédito pela opção ganhou.

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
>* [Exemplo de atribuição 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
