---
unique-page-id: 2951259
description: Glossário de tipo de campo personalizado - Documentos do Marketo - Documentação do produto
title: Glossário de tipo de campo personalizado
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 2%

---

# Glossário de tipo de campo personalizado {#custom-field-type-glossary}

Ao criar um campo personalizado no Marketo, você tem uma lista de tipos para escolher.

>[!PREREQUISITES]
>
>[Criar um campo personalizado no Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>Dependendo do tipo de campo, filtro/acionador [operadores](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) será diferente.

>[!NOTE]
>
>A maioria dos campos não atinge o máximo em número de caracteres, mas sim em quantidade de bytes. Por causa disso, não podemos fornecer um limite de caracteres definitivo para cada campo. A exceção é **String**, que atinge 255 caracteres.

## Booleano {#boolean}

**Nome do exemplo:** É cliente - Marque suas pessoas como clientes

**Valores de exemplo:** True (marcado) / False (desmarcado)

**Operadores**: Nenhum

## Moeda {#currency}

**Nome do exemplo:** Orçamento - Armazene um valor numérico para o orçamento de uma empresa

**Valores de exemplo:** 100

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Data {#date}

**Nome do exemplo:** Data de renovação - Armazene as datas de renovação dos clientes

**Valores de exemplo:** 19/8/14

**Operadores**: é, não é, entre, no passado, antes, no futuro, no futuro, depois, no período de tempo, depois, antes, depois, em ou depois, em ou antes, está vazio, não está vazio

## Datetime {#datetime}

**Nome do exemplo:** Data de criação - Armazena a data e a hora em que uma pessoa é criada

**Valores de exemplo:** 19/8/14 2:00

**Operadores**: é, não é, entre, no passado, antes, no futuro, no futuro, depois, no período de tempo, depois, antes, depois, em ou depois, em ou antes, está vazio, não está vazio

## E-mail {#email}

**Nome do exemplo:** Email alternativo - Mantenha um endereço de email alternativo para sua pessoa (na verdade, não é possível enviar emails para esse campo, como o campo de endereço de email padrão, este é especial)

**Valores de exemplo:** name@company.com

**Operadores**: é, não é, começa com, não começa com, contém, não contém, está vazio, não está vazio

## Flutuante {#float}

**Nome do exemplo:** Média de Ponto de Grau - Mantenha a média do ponto de grade de uma pessoa ou qualquer outro valor numérico que tenha decimais

**Valores de exemplo:** 2,47

**Operadores**: entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Fórmula {#formula}

**Nome do exemplo:** Saudações - use este campo especial em um [solução para obter a saudação correta](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) com base no sexo

**Valores de exemplo:** verifique a solução vinculada

## Inteiro {#integer}

**Nome do exemplo:** Número de funcionários - armazene um valor numérico que não requer decimais

**Valores de exemplo:** 600

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Percentual {#percent}

**Nome do exemplo:** Probabilidade de comprar - armazene um valor percentual (talvez calculado no lado do CRM)

**Valores de exemplo:** 85%

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Telefone {#phone}

**Nome do exemplo:** Telefone alternativo - armazene um número de telefone adicional para o seu pessoal

**Exemplo de valor:** 650-555-5555

**Operadores**: é, não é, começa com, não começa com, contém, não contém, está vazio, não está vazio

## Pontuação {#score}

**Nome do exemplo:** Pontuação comportamental / Pontuação demográfica - crie vários campos de pontuação para rastrear atributos diferentes.

**Exemplo de valor:** 14.

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Sequência de caracteres {#string}

**Nome do exemplo:** Nome do meio - armazene um atributo de texto adicional

**Exemplo de valor:** Rosa

**Operadores**: é, não é, começa com, não começa com, contém, não contém, está vazio, não está vazio

## Área de texto {#text-area}

**Nome do exemplo:** Comentários - adicione um campo de comentários aos formulários para permitir a entrada de texto de várias linhas

**Exemplo de valor:** Este artigo é fantástico!

**Operadores**: é, não é, começa com, não começa com, contém, não contém, está vazio, não está vazio

## URL {#url}

**Nome do exemplo:** Blog - crie um campo para armazenar urls de blog de pessoas

**Exemplo de valor:** www.myblog.com

**Operadores**: é, não é, começa com, não começa com, contém, não contém, está vazio, não está vazio
