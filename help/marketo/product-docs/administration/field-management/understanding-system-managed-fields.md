---
unique-page-id: 5472615
description: Noções básicas sobre campos gerenciados pelo sistema - Documentação do Marketo - Documentação do produto
title: Noções básicas sobre campos gerenciados pelo sistema
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 16%

---

# Noções básicas sobre campos gerenciados pelo sistema {#understanding-system-managed-fields}

Você deve ter notado que a variável [página de detalhes da pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} O tem uma série de campos não editáveis criados pela Marketo. Esses dados vêm de várias fontes e há inúmeros valores que podem ser exibidos.

## Tipos de campos {#field-types}

| **Nome do campo** | **Definição** |
|---|---|
| Tipo de fonte original | O local em que uma pessoa ou visitante do site foi descoberto pela primeira vez (Exemplo: Importação de lista, Visita de página da Web) |
| Informações da fonte original | Informações específicas sobre esse local (Exemplo: Nome da lista, URL da página da Web) |
| Mecanismo de pesquisa original | Se aplicável, o mecanismo de pesquisa que encaminhou a pessoa para a origem de entrada original |
| Frase de pesquisa original | Se aplicável, o termo de pesquisa usado que indicou a pessoa à fonte de entrada original |
| Referenciador original | URL que hospedava a fonte de entrada original |
| Tipo de fonte de registro | O local em que uma atividade se tornou uma pessoa pela primeira vez (Exemplo: Importação de lista, Visita de página da Web) |
| Informações da fonte de registro | Informações específicas sobre esse local (Exemplo: Nome da lista, URL da página da Web) |
| IP anônimo | Indica o endereço IP de uma pessoa |
| Empresa inferida | A melhor estimativa da Marketo (com base no IP) da empresa da pessoa |
| Cidade inferida | A melhor estimativa da Marketo (com base no IP) da cidade da pessoa |
| Região inferida | A melhor estimativa da Marketo (com base no IP) do estado ou região da pessoa |
| Código postal inferido | Melhor estimativa da Marketo (com base no IP) do código postal da pessoa |
| País inferido | A melhor estimativa da Marketo (com base no IP) do país da pessoa |
| Área metropolitana inferida | A melhor estimativa da Marketo (com base no IP) da área metropolitana da pessoa |
| Código de área telefônica inferido | A melhor estimativa da Marketo (com base no IP) do código de área da pessoa |

## Valores possíveis para o original e o tipo de origem do registro {#possible-values-for-original-and-registration-source-type}

Abaixo estão alguns valores possíveis e o que eles significam.

| **Tipo de fonte original** | **Definição** |
|---|---|
| Salesforce.com | A pessoa foi descoberta de um [!DNL Webhook] sincronizar |
| Visitas à página da Web | A pessoa foi descoberta de uma página da Web |
| Preenchimento de formulário da Web | A pessoa foi descoberta depois de preencher um formulário |
| Importação de lista | A pessoa foi descoberta em uma importação de lista |
| Nova pessoa | A pessoa foi inserida manualmente no banco de dados |
| Clique em links da Web | A pessoa foi descoberta depois de clicar em um link |
| E-mail de vendas | Uma pessoa recebeu um email via [!DNL Sales Insight] Suplemento de email |
| Pessoa | A pessoa foi sincronizada a partir de [!DNL Salesforce] como pessoa |
| Contato | A pessoa foi sincronizada a partir de [!DNL Webhook] como contato |
| [!DNL Munchkin] API | A pessoa foi descoberta pelo Marketo Engage [!DNL Munchkin] API |
| Aplicativo social | A pessoa foi descoberta por um widget de redes sociais |
| API de serviço Web | A pessoa foi descoberta por uma API de serviço Web |
| Parceiro de evento | A pessoa foi descoberta por meio de um serviço de webinário sincronizado |
| Associar lead | Pessoa que foi mesclada por meio de chamada à API Associar lead |

| **Tipo de fonte de registro** | **Definição** |
|---|---|
| Importação de lista | Tornou-se uma pessoa por meio de uma importação de lista |
| Salesforce.com | Tornou-se uma pessoa através de um [!DNL Webhook] sincronizar |
| Preenchimento de formulário da Web | Tornou-se uma pessoa após preencher um formulário |
| E-mail de vendas | Uma pessoa recebeu um email via [!DNL Webhook] Suplemento de email |
| API de serviço Web | A pessoa foi criada por meio da API SOAP/REST |
| Nova pessoa | A pessoa foi inserida manualmente no banco de dados |
| [!DNL Munchkin] API | Tornou-se uma pessoa pelo Marketo [!DNL Munchkin] API |
| Aplicativo social | Tornou-se uma pessoa através de um widget social |
| Parceiro de evento | Tornou-se uma pessoa por meio de um serviço de webinário vinculado |
