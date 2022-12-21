---
unique-page-id: 5472615
description: Noções básicas sobre os campos gerenciados do sistema - Documentos do Marketo - Documentação do produto
title: Noções básicas sobre campos gerenciados do sistema
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 16%

---

# Noções básicas sobre campos gerenciados do sistema {#understanding-system-managed-fields}

Você pode ter notado que a variável [página de detalhes da pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) O tem uma série de campos não editáveis criados pelo Marketo. Esses dados vêm de várias fontes e há inúmeros valores que podem ser exibidos.

## Tipos de campos {#field-types}

| **Nome do campo** | **Definição** |
|---|---|
| Tipo de fonte original | O local em que uma pessoa ou um visitante do site foi descoberto pela primeira vez (por exemplo: Importação de lista, Visita à página da Web) |
| Informações da fonte original | Especifica o local (exemplo: Nome da lista, URL da página da Web) |
| Mecanismo de pesquisa original | Se aplicável, o mecanismo de pesquisa que remeteu a pessoa para a fonte de entrada original |
| Frase de pesquisa original | Se aplicável, o termo de pesquisa usado que fez referência à pessoa para a fonte de entrada original |
| Responsável pela indicação original | URL que hospedou a fonte de entrada original |
| Tipo de fonte de registro | O local em que uma atividade se tornou primeiro uma pessoa (exemplo: Importação de lista, Visita à página da Web) |
| Informações da fonte de registro | Especifica o local (exemplo: Nome da lista, URL da página da Web) |
| IP anônimo | Indica o endereço IP de uma pessoa |
| Empresa inferida | Melhor suposição da Marketo (com base no IP) da empresa da pessoa |
| Cidade inferida | Melhor suposição da Marketo (com base no IP) da cidade da pessoa |
| Região inferida | Melhor suposição da Marketo (com base no IP) do estado ou região da pessoa |
| Código postal inferido | Melhor suposição da Marketo (com base no IP) do código postal da pessoa |
| País inferido | A melhor suposição da Marketo (baseada no IP) do país da pessoa |
| Área metropolitana inferida | Melhor suposição da Marketo (com base no IP) da área metropolitana da pessoa |
| Código de área telefônica inferido | Melhor suposição da Marketo (com base no IP) do código de área da pessoa |

## Valores possíveis para o original e o tipo de fonte de registro {#possible-values-for-original-and-registration-source-type}

Abaixo estão alguns valores possíveis e o que eles significam.

| **Tipo de fonte original** | **Definição** |
|---|---|
| Salesforce.com | A pessoa foi descoberta de uma sincronização Salesforce |
| Visitas à página da Web | A pessoa foi descoberta de uma página da Web |
| Preenchimento do formulário Web | A pessoa foi descoberta após preencher um formulário |
| Importação de lista | A pessoa foi descoberta de uma importação de lista |
| Nova pessoa | A pessoa foi inserida manualmente no banco de dados |
| Clique no link da Web | A pessoa foi descoberta após clicar em um link |
| Email de vendas | A pessoa recebeu um email por meio do Suplemento de email Sales Insight |
| Pessoa | A pessoa foi sincronizada do Salesforce como pessoa |
| Contato | A pessoa foi sincronizada do Salesforce como um contato |
| API Munchkin | A pessoa foi descoberta pela API do Marketo Munchkin |
| Aplicativo social | A pessoa foi descoberta por um widget social |
| API de serviço Web | A pessoa foi descoberta por uma API de serviço da Web |
| Parceiro de evento | A pessoa foi descoberta por meio de um serviço de webinar sincronizado |
| Associar lead | Pessoa que foi mesclada por meio da chamada de API Associar lead |

| **Tipo de fonte de registro** | **Definição** |
|---|---|
| Importação de lista | Tornou-se uma pessoa por meio de uma importação de lista |
| Salesforce.com | Torne-se uma pessoa por meio de uma sincronização Salesforce |
| Preenchimento do formulário Web | Tornar-se uma pessoa depois de preencher um formulário |
| Email de vendas | A pessoa recebeu um email por meio do Suplemento de email Sales Insight |
| API de serviço Web | A pessoa foi criada por meio da API SOAP/REST |
| Nova pessoa | A pessoa foi inserida manualmente no banco de dados |
| API Munchkin | Torne-se uma pessoa por meio da API do Marketo Munchkin |
| Aplicativo social | Torne-se uma pessoa por meio de um widget social |
| Parceiro de evento | Torne-se uma pessoa por meio de um serviço de webinário vinculado |
