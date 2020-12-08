---
unique-page-id: 2951259
description: Glossário de tipo de campo personalizado - Documentos do Marketing - Documentação do produto
title: Glossário de tipo de campo personalizado
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---


# Glossário de tipo de campo personalizado {#custom-field-type-glossary}

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Ao criar um campo personalizado no Marketo, você tem uma lista de tipos para escolher.

>[!NOTE]
>
>**Pré-requisitos**
>
>* [Criar um campo personalizado no Marketo](create-a-custom-field-in-marketo.md)

>



>[!TIP]
>
>Dependendo do tipo de campo, [os operadores](https://docs.marketo.com/display/public/DOCS/Smart+List+Filter+Operators+Glossary) de filtro/acionador serão diferentes.

>[!NOTE]
>
>A maioria dos campos não atinge o limite máximo em número de caracteres, mas sim em quantidade de bytes. Por causa disso, não é possível fornecer um limite de caracteres definitivo para cada campo. A exceção é **String**, que atinge 255 caracteres.

## Booleano {#boolean}

**Nome do exemplo:** É cliente - Marque suas pessoas como clientes

**Valores de exemplo:** True (marcado) / False (desmarcado)

**Operadores**: Nenhum

## Moeda {#currency}

**Nome do exemplo:** Orçamento - Armazenar um valor numérico para um orçamento de empresa

**Valores de exemplo:** 100

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Data {#date}

**Nome do exemplo:** Data de renovação - Armazene as datas de renovação dos clientes

**Valores de exemplo:** 19/08/14

**Operadores**: é, não é, entre, no passado, no passado, no futuro, no futuro, depois, no futuro, depois, no tempo, depois, antes, depois, em ou antes, está vazio, não está vazio

## Data e hora {#datetime}

**Nome do exemplo:** Data de criação - Armazena a data e a hora em que uma pessoa é criada

**Valores de exemplo:** 19/08/14 2:00

**Operadores**: é, não é, entre, no passado, no passado, no futuro, no futuro, depois, no futuro, depois, no tempo, depois, antes, depois, em ou antes, está vazio, não está vazio

## Email {#email}

**Nome do exemplo:** E-mail alternativo - Mantenha um endereço de e-mail alternativo para seu pessoal (não é possível enviar e-mails para esse campo como o campo de endereço de e-mail padrão, este é especial)

**Valores de exemplo:** [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#335d525e5673505c5e43525d4a1d505c5e)

**Operadores**: is, is not, start com, not start com, contém, não contém, está vazio, não está vazio

## Flutuar {#float}

**Nome do exemplo:** Média de Ponto de Grau - Mantenha a média de ponto de grade de uma pessoa ou qualquer outro valor numérico que tenha decimais

**Valores de exemplo:** 2,47

**Operadores**: entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Fórmula {#formula}

**Nome do exemplo:** Saudações - use este campo especial em uma [solução para obter a saudação](create-and-use-a-concatenated-string-formula-field.md) correta com base no gênero

**Valores de exemplo:** verifique a solução vinculada

## Número inteiro {#integer}

**Nome do exemplo:** Número de funcionários - armazene um valor numérico que não exija decimais

**Valores de exemplo:** 600

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Porcentagem {#percent}

**Nome do exemplo:** Provavelmente Comprar - armazene um valor percentual (talvez calculado no lado do CRM)

**Valores de exemplo:** 85%

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Telefone {#phone}

**Nome do exemplo:** Telefone alternativo - armazene um número de telefone adicional para a sua pessoa

**Exemplo de valor:** 650-555-5555

**Operadores**: is, is not, start com, not start com, contém, não contém, está vazio, não está vazio

## Pontuação {#score}

**Nome do exemplo:** Pontuação comportamental / Pontuação demográfica - crie vários campos de pontuação para acompanhar atributos diferentes.

**Exemplo de valor:** 14

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## String {#string}

**Nome do exemplo:** Nome do meio - armazene um atributo de texto adicional

**Exemplo de valor:** Rosa

**Operadores**: is, is not, start com, not start com, contém, não contém, está vazio, não está vazio

## Área de texto {#text-area}

**Nome do exemplo:** Comentários - adicione um campo de comentários aos formulários para permitir a entrada de texto de várias linhas

**Exemplo de valor:** Este artigo é fantástico!

**Operadores**: is, is not, start com, not start com, contém, não contém, está vazio, não está vazio

## URL {#url}

**Nome do exemplo:** Blog - crie um campo para armazenar urls de blog de pessoas

**Exemplo de valor:** www.myblog.com

**Operadores**: is, is not, start com, not start com, contém, não contém, está vazio, não está vazio
