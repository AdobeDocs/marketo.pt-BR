---
unique-page-id: 5472615
description: Entendendo os campos gerenciados pelo sistema - Documentos do Marketing - Documentação do produto
title: Noções básicas sobre campos gerenciados pelo sistema
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---


# Entendendo os campos gerenciados pelo sistema {#understanding-system-managed-fields}

Você pode ter notado que a [página de detalhes da pessoa](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) tem uma série de campos não editáveis criados pelo Marketo. Esses dados vêm de várias fontes, e há inúmeros valores que podem ser exibidos.

## Tipos de campo {#field-types}

| **Nome do campo** | **Definição** |
|---|---|
| Tipo de origem original | O local em que um visitante de pessoa ou site foi descoberto pela primeira vez (por exemplo: Importação de lista, Visita à página da Web) |
| Informações de origem originais | Especifica o local (exemplo: Nome da lista, URL da página da Web) |
| Mecanismo de pesquisa original | Se aplicável, o mecanismo de pesquisa que indicou a pessoa para a fonte de entrada original |
| Frase de pesquisa original | Se aplicável, o termo de pesquisa usado que indicou a pessoa para a fonte de entrada original |
| Quem indicou original | URL que hospedou a fonte de entrada original |
| Tipo de fonte de registro | O local em que uma atividade se tornou pela primeira vez uma pessoa (por exemplo: Importação de lista, Visita à página da Web) |
| Informações da Fonte de Registro | Especifica o local (exemplo: Nome da lista, URL da página da Web) |
| IP anônimo | Indica o endereço IP de uma pessoa |
| Empresa inferida | A melhor suposição de Marketo (baseada no IP) da empresa da pessoa |
| Cidade Inferida | Melhor suposição de Marketo (com base no IP) da cidade |
| Região do Estado Inferior | A melhor suposição de Marketo (baseada no IP) do estado ou região da pessoa |
| Código postal inferido | Melhor suposição do comerciante (com base no IP) do código postal da pessoa |
| País Inferior | Melhor suposição do comerciante (com base no IP) sobre o país da pessoa |
| Área metropolitana inferida | A melhor estimativa de Marketo (baseada no IP) da área metropolitana da pessoa |
| Código de área do telefone inferior | Melhor suposição do Marketo (com base no IP) do código de área da pessoa |

## Valores possíveis para o original e o tipo de fonte de registro {#possible-values-for-original-and-registration-source-type}

Abaixo estão alguns valores possíveis e o que eles significam.

| **Tipo de origem original** | **Definição** |
|---|---|
| Salesforce.com | A pessoa foi descoberta de uma sincronização do Salesforce |
| Visitas à página da Web | A pessoa foi descoberta de uma página da Web |
| Preenchimento de formulário da Web | A pessoa foi descoberta após preencher um formulário |
| Importação de lista | A pessoa foi descoberta de uma importação de lista |
| Nova pessoa | A pessoa foi inserida manualmente no banco de dados |
| Clique no link da Web | A pessoa foi descoberta após clicar em um link |
| Email de vendas | A pessoa recebeu um email por meio do suplemento de email do Sales Insight |
| Pessoa | A pessoa foi sincronizada do Salesforce como pessoa |
| Contato | A pessoa foi sincronizada do Salesforce como um contato |
| API Munchkin | Pessoa foi descoberta pela API Munchkin de Marketo |
| Aplicativo social | A pessoa foi descoberta por um widget social |
| API de serviço da Web | A pessoa foi descoberta por uma API de serviço da Web |
| Parceiro evento | A pessoa foi descoberta por meio de um serviço de webinar sincronizado |
| Associar cliente potencial | Pessoa que foi mesclada por meio da chamada Associate Lead API |

| **Tipo de fonte de registro** | **Definição** |
|---|---|
| Importação de lista | Tornou-se uma pessoa através de uma importação de lista |
| Salesforce.com | Tornou-se uma pessoa através de uma sincronização Salesforce |
| Preenchimento de formulário da Web | Tornou-se uma pessoa depois de preencher um formulário |
| Email de vendas | A pessoa recebeu um email por meio do suplemento de email do Sales Insight |
| API de serviço da Web | A pessoa foi criada por meio da API SOAP/REST |
| Nova pessoa | A pessoa foi inserida manualmente no banco de dados |
| API Munchkin | Tornou-se uma pessoa através da API Munchkin do Marketo |
| Aplicativo social | Torne-se uma pessoa através de um widget social |
| Parceiro evento | Tornou-se uma pessoa por meio de um serviço de webinar vinculado |

