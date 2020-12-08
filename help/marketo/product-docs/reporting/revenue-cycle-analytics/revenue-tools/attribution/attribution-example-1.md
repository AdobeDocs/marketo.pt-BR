---
unique-page-id: 7514126
description: Exemplo de atribuição 1 - Documentos de marketing - Documentação do produto
title: Exemplo de atribuição 1
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# Exemplo de atribuição 1 {#attribution-example}

Leia o seguinte cenário e tente determinar os números que devem estar na grade.

* 11 de abril | Fred é adquirido por (Transmissão)
* 15 de abril | Participantes do Margo (Webinar) - sucesso
* 22 de abril | Fred está associado (função) à oportunidade
* 22 de abril | A oportunidade é criada para $3.000

| Nome do programa | (Apresentação) | (Webinar) |
|---|---|---|
| (FT) Opção criada | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT) Gasoduto criado | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT) Opty Won | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT) Ganho de Receita | `<pre>0</pre>` | `<pre>0</pre>` |

**Mostrar respostas**

>[!NOTE]
>
>**Explicação**
>
>Primeiro, entender que alguns tipos são CONTAGENS e outros são MOEDA. A opção Criada é uma contagem, um número inteiro. Pipeline é uma moeda. No Marketo, a moeda estará em conformidade com as configurações de local do administrador.
>
>A razão pela qual a apresentação recebeu todo o crédito é porque a Margo não estava associada a um papel na oportunidade. Nenhum papel, nenhum crédito.

>[!NOTE]
>
>**Regras de atribuição**
>
>1. O crédito é dividido uniformemente
>1. Você não pode dar mais crédito do que você ganhou
>1. Você não pode dar crédito por algo que aconteceu no passado


Experimente todos os exemplos e você será um pro atribuição!

>[!NOTE]
>
>**Artigos relacionados**
>
>* [Exemplo de atribuição 2](attribution-example-2.md)
>* [Exemplo de atribuição 3](attribution-example-3.md)
>* [Exemplo de atribuição 4](attribution-example-4.md)

