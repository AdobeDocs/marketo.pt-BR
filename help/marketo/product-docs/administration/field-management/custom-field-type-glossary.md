---
unique-page-id: 2951259
description: Glossário de tipo de campo personalizado - Documentação do Marketo - Documentação do produto
title: Glossário de tipo de campo personalizado
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
source-git-commit: 20c41143d1e7839352dddbfea0951c2633987692
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
>A maioria dos campos não atinge o número máximo de caracteres, mas a quantidade de bytes. Por esse motivo, não podemos fornecer um limite de caracteres definitivo para cada campo. A exceção é **String**, que tem no máximo 255 caracteres.

## Booleano {#boolean}

**Nome do exemplo:** É cliente - Marque suas pessoas como clientes

**Valores de exemplo:** Verdadeiro (marcado) / Falso (desmarcado)

**Operadores**: Nenhuma

## Moeda {#currency}

**Nome do exemplo:** Orçamento - Armazena um valor numérico para o orçamento de uma empresa

**Valores de exemplo:** 100

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Data {#date}

**Nome do exemplo:** Data de renovação - armazene as datas de renovação dos clientes

**Valores de exemplo:** 19/08/14

**Operadores**: é, não é, entre, no passado, no passado antes, no futuro, no futuro depois, no intervalo de tempo, depois, antes, em ou depois, em ou antes, está vazio, não está vazio

## Datetime {#datetime}

**Nome do exemplo:** Data de criação - Armazena a data e a hora em que uma pessoa é criada

**Valores de exemplo:** 19/08/14 2:00

**Operadores**: é, não é, entre, no passado, no passado antes, no futuro, no futuro depois, no intervalo de tempo, depois, antes, em ou depois, em ou antes, está vazio, não está vazio

## Email {#email}

**Nome do exemplo:** Email alternativo - Mantenha um endereço de email alternativo para sua equipe (na verdade, o não pode enviar emails para esse campo, como o campo de endereço de email padrão, esse é especial)

**Valores de exemplo:** name@company.com

**Operadores**: é, não é, começa com, não começa com, contém, não contém, está vazio, não está vazio

## Flutuante {#float}

**Nome do exemplo:** Média de Ponto de Grau - Mantenha a média de ponto de grau de uma pessoa ou qualquer outro valor numérico que tenha decimais

**Valores de exemplo:** 2,47

**Operadores**: entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Fórmula {#formula}

**Nome do exemplo:** Saudações - use este campo especial em uma [solução para obter a saudação certa](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) com base no gênero

**Valores de exemplo:** verifique a solução vinculada

## Inteiro {#integer}

**Nome do exemplo:** Número de Funcionários - armazene um valor numérico que não exige decimais

**Valores de exemplo:** 600

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Percentual {#percent}

**Nome do exemplo:** Probabilidade de compra - armazene um valor percentual (talvez calculado no lado do CRM)

**Valores de exemplo:** 85%

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Telefone {#phone}

**Nome do exemplo:** Telefone Alternativo - armazene um número de telefone adicional para sua equipe

**Exemplo de valor:** 650 555 555

**Operadores**: é, não é, começa com, não começa com, contém, não contém, está vazio, não está vazio

## Pontuação {#score}

**Nome do exemplo:** Pontuação comportamental/Pontuação demográfica - crie vários campos de pontuação para rastrear atributos diferentes

**Exemplo de valor:** 14

**Operadores**: é, não é, entre, maior que, menor que, pelo menos, no máximo, está vazio, não está vazio

## Sequência de caracteres {#string}

**Nome do exemplo:** Nome do meio - armazena um atributo de texto adicional

**Exemplo de valor:** Rosa

**Operadores**: é, não é, começa com, não começa com, contém, não contém, está vazio, não está vazio

## Área de texto {#text-area}

**Nome do exemplo:** Comentários - adicione um campo de comentários aos formulários para permitir a entrada de texto multilinha

**Exemplo de valor:** Este artigo é fantástico!

**Operadores**: é, não é, começa com, não começa com, contém, não contém, está vazio, não está vazio

## URL {#url}

**Nome do exemplo:** Blog - criar um campo para armazenar URLs de blog de pessoas

**Exemplo de valor:** www.myblog.com

**Operadores**: é, não é, começa com, não começa com, contém, não contém, está vazio, não está vazio
