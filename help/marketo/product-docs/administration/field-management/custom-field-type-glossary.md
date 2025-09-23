---
unique-page-id: 2951259
description: Glossário de tipo de campo personalizado - Documentação do Marketo - Documentação do produto
title: Glossário de tipos de campos personalizados
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 3%

---

# Glossário de tipos de campos personalizados {#custom-field-type-glossary}

Ao criar um campo personalizado no Marketo, você tem uma lista de tipos para escolher.

>[!PREREQUISITES]
>
>[Criar um campo personalizado no Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>Dependendo do tipo de campo, o filtro/gatilho [operadores](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) será diferente.

>[!NOTE]
>
>A maioria dos campos não atinge o número máximo de caracteres, mas a quantidade de bytes. Por esse motivo, não podemos fornecer um limite de caracteres definitivo para cada campo. A exceção é **String**, que tem no máximo 255 caracteres.

## Booleano {#boolean}

**Nome de Exemplo:** É Cliente - Marque seus funcionários como clientes

**Valores de Exemplo:** Verdadeiro (marcado) / Falso (desmarcado)

**Operadores**: nenhum

## Moeda {#currency}

**Nome do Exemplo:** Orçamento - Armazena um valor numérico para o orçamento de uma empresa

**Valores de Exemplo:** 100

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Data {#date}

**Nome do Exemplo:** Data de Renovação - Armazene as datas de renovação de seus clientes

**Valores de Exemplo:** 19/08/14

**Operadores**: é, não está, entre, no passado, no passado antes, no futuro, no futuro depois, no intervalo de tempo, depois, antes, em ou depois, em ou antes, está vazio, não está vazio

## Data/hora {#datetime}

**Nome do Exemplo:** Data de Criação - Armazena a data e a hora em que uma pessoa é criada

**Valores de Exemplo:** 19/08/14 2:00

**Operadores**: é, não está, entre, no passado, no passado antes, no futuro, no futuro depois, no intervalo de tempo, depois, antes, em ou depois, em ou antes, está vazio, não está vazio

## Email {#email}

**Nome de Exemplo:** Email Alternativo - Mantenha um endereço de email alternativo para sua equipe (na verdade, não é possível enviar emails para este campo, como o campo de endereço de email padrão, pois esse é especial)

**Valores de Exemplo:** <name@company.com>

**Operadores**: é, não é, começa com, não começa com, contém, não contém, está vazio, não está vazio

## Flutuante {#float}

**Exemplo de Nome:** Média de Ponto de Grade - Mantenha a média de ponto de grade de uma pessoa ou qualquer outro valor numérico que tenha decimais

**Valores de Exemplo:** 2.47

**Operadores**: entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Fórmula {#formula}

**Nome de Exemplo:** Saudações - use este campo especial em uma solução [ para obter a saudação correta](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) com base no sexo

**Valores de Exemplo:** verifique a solução vinculada

## Inteiro {#integer}

**Nome de Exemplo:** Número de Funcionários - armazene um valor numérico que não exige decimais

**Valores de Exemplo:** 600

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Porcentagem {#percent}

**Nome de Exemplo:** Probabilidade de Compra - armazene um valor percentual (talvez calculado no lado do CRM)

**Valores de Exemplo:** 85%

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Telefone {#phone}

**Exemplo de Nome:** Telefone Alternativo - armazene um número de telefone adicional para sua equipe

**Exemplo de valor:** 650-555-5555

**Operadores**: é, não é, começa com, não começa com, contém, não contém, está vazio, não está vazio

## Pontuação {#score}

**Nome do Exemplo:** Pontuação Comportamental/Pontuação Demográfica - crie vários campos de pontuação para acompanhar atributos diferentes

**Valor de Exemplo:** 14

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## String {#string}

**Nome do Exemplo:** Nome do Meio - armazenar um atributo de texto adicional

**Exemplo de valor:** Rose

**Operadores**: é, não é, começa com, não começa com, contém, não contém, está vazio, não está vazio

## Área de texto {#text-area}

**Nome de Exemplo:** Comentários - adicione um campo de comentários aos seus formulários para permitir a entrada de texto multilinha

**Exemplo de valor:** este artigo é fantástico!

**Operadores**: é, não é, começa com, não começa com, contém, não contém, está vazio, não está vazio

## URL {#url}

**Nome de Exemplo:** Blog - criar um campo para armazenar URLs de blogs de pessoas

**Valor de Exemplo:** &lt;www.myblog.com>

**Operadores**: é, não é, começa com, não começa com, contém, não contém, está vazio, não está vazio
