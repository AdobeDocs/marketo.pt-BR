---
unique-page-id: 7514126
description: Exemplo 1 de atribuição - Documentação do Marketo - Documentação do produto
title: Exemplo de atribuição 1
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 4%

---

# Exemplo de atribuição 1 {#attribution-example}

Leia o cenário a seguir e tente determinar os números que devem estar na grade.

* Abril de 11 | Fred é adquirido pela (Tradeshow)
* Abril de 15 | Margo comparece (webinário) - sucesso
* Abril de 22 | Fred está associado (função) à oportunidade
* Abril de 22 | A oportunidade é criada por US$ 3.000

| Nome do programa | (Feira) | (Webinário) |
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
>A primeira é entender que alguns tipos são CONTAGENS e outros são MOEDA. A opção Criada é uma contagem, um número inteiro. Pipeline é uma moeda. No Marketo, a moeda estará em conformidade com as configurações do local do administrador.
>
>O motivo pelo qual o Tradeshow recebeu todo o crédito é porque Margo não estava associado a um papel na oportunidade. Sem papel, sem crédito.

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
>* [Exemplo de atribuição 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Exemplo de atribuição 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Exemplo de atribuição 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
