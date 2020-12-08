---
unique-page-id: 7514149
description: Exemplo de atribuição 3 - Documentos de marketing - Documentação do produto
title: Exemplo de atribuição 3
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---


# Exemplo de atribuição 3 {#attribution-example}

Leia o seguinte cenário e tente determinar os números que devem estar na grade.

* 11 de abril | Steve downloads (conteúdo) - sucesso
* 22 de abril | A oportunidade é criada por US$ 3.000 (Steve e Jason têm papéis)
* 25 de abril | Jason participa (Webinar) - sucesso
* 30 de abril | A oportunidade está fechada

| Métrica de atribuição | (Conteúdo) | (Webinar) |
|---|---|---|
| (MT) Opção criada | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT) Gasoduto criado | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Ganho de receita | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**Mostrar respostas**

>[!NOTE]
>
>**Explicação**
>
>Lembre-se da regra de atribuição nº 3. Jason teve programa sucesso DEPOIS que a propriedade foi criada. Portanto, o webinar não pode receber crédito pela criação da oportunidade. Só o crédito pela Opty ganhou.
>
>Portanto, (Conteúdo) tem 100% de crédito pela criação e pipeline da Opty, mas apenas 50% de crédito pela propriedade ganhou.

>[!NOTE]
>
>**Regras de atribuição**
>
>1. O crédito é dividido uniformemente
>1. Você não pode dar mais crédito do que você ganhou
>1. Você não pode dar crédito por algo que aconteceu no passado

>



<br> 

Experimente todos os exemplos e você será um pro atribuição!

>[!NOTE]
>
>**Artigos relacionados**
>
>* [Exemplo de atribuição 1](attribution-example-1.md)
>* [Exemplo de atribuição 2](attribution-example-2.md)
>* [Exemplo de atribuição 4](attribution-example-4.md)

