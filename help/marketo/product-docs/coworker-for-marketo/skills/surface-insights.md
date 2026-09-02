---
description: Converse com o Colaborador do Marketo Engage sobre seus dados de desempenho. Faça perguntas em linguagem simples e obtenha respostas com base no seu ambiente do Marketo Engage.
title: Insights de superfície
badge: Beta
hide: true
source-git-commit: 224dff93cda319bb6bb59fcbec4edb13cc940f4a
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# Insights de superfície {#surface-insights}

O Surface Insights permite conversar sobre os dados de desempenho do Marketo. Faça perguntas em linguagem simples e obtenha respostas com base no seu ambiente do Marketo.

>[!PREREQUISITES]
>
>* Para usar esse recurso, primeiro você deve concordar com os [termos principais da Gen-AI e os termos complementares](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Entre em contato com a Equipe de conta da Adobe (seu gerente de conta) para obter detalhes.
>
>* Você deve ter acesso aos programas e relatórios sobre os quais está consultando.

>[!AVAILABILITY]
>
>No momento, esse recurso está na versão beta fechada. Não divulgue esta documentação.

## Como usar {#how-to-use}

1. Em Meu Marketo, clique no bloco **Colaborador do Marketo Engage**.

1. Na janela do prompt, faça uma pergunta sobre o desempenho. Seja específico sobre o período ou programa, se você tiver um em mente.

1. Revise o resumo de colaborador para devoluções do Marketo Engage. Ele incluirá métricas principais como taxas de abertura, taxas de clique, taxas de conversão e contagens de clientes potenciais, dependendo do que você solicitou.

1. Faça perguntas complementares para explorar áreas específicas (por exemplo, &quot;Qual email naquele programa tinha a maior taxa de cliques?&quot;) ou &quot;Como isso se compara ao trimestre passado?&quot;).

## Casos de uso {#use-cases}

**Análise trimestral do programa**: um gerente de geração de demanda está se preparando para uma reunião de análise da campanha. Eles perguntam: &quot;Como meus programas de educação do segundo trimestre funcionaram em geral?&quot; O colaborador do Marketo Engage retorna taxas de abertura, taxas de clique para abertura, taxas de cancelamento de inscrição e o número de pessoas/leads que progrediram para MQL em todos os programas de criação do segundo trimestre, com uma observação sobre quais programas tiveram desempenho melhor que a média do grupo.

**Comparando duas campanhas**: um gerente de campanha executou duas versões de uma série de convites de webinário com linhas de assunto diferentes. Eles perguntam: &quot;Como o programa de webinário de abril se comparou com o de março em termos de taxa de inscrição?&quot; O colaborador do Marketo Engage retorna os números de registro para cada um e destaca a diferença, para que possam ver qual abordagem funcionou melhor.

**Encontrando conteúdo com melhor desempenho**: um especialista em operações de marketing quer saber quais ativos de email impulsionaram mais engajamento no mês passado. Eles perguntam: &quot;Quais emails tiveram as maiores taxas de cliques em maio?&quot; O Colaborador do Marketo Engage retorna uma lista classificada de ativos de email com taxas de clique, para que possa identificar o que aconteceu e informar as decisões de conteúdo futuras.

## Itens a serem observados {#things-to-note}

* Os insights de superfície são baseados nos dados disponíveis na instância do Marketo. Se um programa não for rastreado ou uma métrica não for capturada, o Co-worker para Marketo Engage não poderá relatar isso.
* Intervalos de datas muito grandes ou perguntas amplas podem retornar resumos de alto nível em vez de detalhes granulares. Por exemplo, &quot;Como foi o desempenho de todos os meus programas nos últimos dois anos?&quot;
* O colaborador do Marketo Engage pode exibir dados, mas não pode fazer alterações em seus programas ou relatórios com base no que encontrar.
* Para relatórios personalizados detalhados com filtros e detalhamentos específicos, as ferramentas de relatório integradas do Marketo ou uma integração de BI podem ser mais apropriadas.
* A atribuição em campanhas multitoque requer a configuração adequada do programa. O colaborador do Marketo Engage relata o que é rastreado, não deduz a atribuição que não foi configurada.
