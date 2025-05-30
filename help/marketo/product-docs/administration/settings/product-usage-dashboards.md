---
description: Painéis de uso de produtos - Documentação do Marketo - Documentação do produto
title: Painéis de uso do produto
hide: true
hidefromtoc: true
feature: Administration
source-git-commit: f3bc58c0d65e8110c5366269fdb4abf817370aee
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Painéis de uso do produto {#product-usage-dashboards}

Os painéis de uso do produto Marketo Engage oferecem a capacidade de visualizar o uso do produto e da plataforma em relação a determinados limites ou backlog de taxa de transferência de dados, uso em relação à cota diária e métricas principais em uma assinatura. A infraestrutura é alocada para fornecer limites de desempenho definidos para os níveis de produto para atributos específicos. Alguns desses limites, como o uso da API, são limites contratados comprados como parte do pacote ou da Camada do produto.

## Como acessar {#how-to-access}

1. No Marketo Engage, clique em **Admin**.

   ![](assets/product-usage-dashboards-1.png)

1. Na árvore à esquerda, role para baixo e selecione **Painéis de Uso de Produtos**.

   ![](assets/product-usage-dashboards-2.png)

## Painel de Uso da Atividade {#activity-usage-dashboard}

### Média de atividades semanais {#average-weekly-activities}

O painel Uso semanal de atividade fornece uma contagem semanal de Tipos de atividade em um período contínuo de 52 semanas. As atividades produzidas semanalmente são um bom indicador de quanto marketing você está fazendo no Marketo Engage. As atividades servem como um proxy para os vários processos do sistema e eventos rastreáveis que ocorrem no Marketo.

Os Tipos de atividade incluem contagens de atividades capturadas quando as pessoas interagem com eventos de marketing, bem como atividades baseadas no sistema acionadas por Ações de fluxo. Alguns exemplos de atividades iniciadas por pessoas são quando uma pessoa abre um email ou clica em um link em um email. Um exemplo de atividades baseadas no sistema acionadas por uma Ação de fluxo é &quot;Enviar para o SFDC&quot; quando o acionador é iniciado. Para exibir uma contagem dos tipos de atividade para uma semana específica, passe o mouse sobre uma semana e exiba a contagem.

![](assets/product-usage-dashboards-3.png){width="800" zoomable="yes"}

#### Perguntas frequentes {#faq}

**Quais Tipos de Atividade são contados?**

Ela depende das atividades incluídas no pipeline.

**As atividades de cliente potencial/pessoa conhecidas e anônimas estão incluídas?**

Somente pessoas/clientes em potencial conhecidos.

**Com que frequência os dados são atualizados?**

As contagens de atividades são atualizadas todas as manhãs.

## Detalhamento de atividade {#activity-breakdown}

Aqui obtemos contagens de atividades dos últimos sete dias com base em fatias significativas dos dados. Agrupar atividades pelos tipos de atividades mais comuns observados nos últimos sete dias. Isso pode incluir categorias como &quot;Alterar valor dos dados&quot;, &quot;Adicionar à lista&quot; ou &quot;Enviar email&quot;. Isso permite que você veja quais tipos de atividades estão acontecendo com mais frequência no sistema. O uso do Tipo de atividade é um indicador importante para determinar o crescimento ou se são necessárias otimizações para reduzir o uso.

>[!NOTE]
>
>* Todos os detalhamentos abaixo são uma soma &quot;acumulada de sete dias&quot; e **não** incluem o dia atual. Então pense nisso como &quot;ontem + seis dias antes disso.&quot;
>
>* O painel mostra apenas os 20 principais tipos de atividade, enquanto o restante é classificado em uma categoria chamada &quot;Outros&quot;.

![](assets/product-usage-dashboards-4.png){width="800" zoomable="yes"}

O uso da atividade é um indicador principal de quanto marketing está sendo realizado e ajuda a visualizar o crescimento em relação ao nível de produto contratado para o. Os painéis também podem ser usados como guia para determinar a otimização que pode/deve ser feita ao reduzir os campos que estão sendo atualizados.

### Por tipo {#by-type}

Agrupar atividades pelos tipos de atividades mais comuns observados nos últimos sete dias. Isso pode incluir categorias como _Alterar Valor dos Dados_, _Adicionar à Lista_ ou _Enviar Email_. Isso permite ver quais tipos de atividades estão acontecendo com mais frequência no Marketo Engage.

### Por atributo de valor de dados de alteração {#by-change-data-value-attribute}

_Alterar Valor de Dados_ é o tipo de atividade mais comum. Indica quando uma parte das informações em um registro de pessoa/cliente potencial é atualizada. Aqui, agrupamos pelos campos que são alterados com mais frequência para que você possa determinar se quais informações são úteis para suas operações de marketing, se há oportunidades para otimizar o uso da plataforma etc.

### Por campanha {#by-campaign}

Grupo pelo qual as campanhas estão produzindo mais atividades. Isso oferece ao insight ver se você tem campanhas particularmente &quot;barulhentas&quot; que criam mais atividade do que o necessário. Aprenda rapidamente sobre campanhas que devem ser desativadas ou campanhas que estão fazendo mais trabalho do que o esperado.

### Por Source (EM BREVE) {#by-source}

Agrupe pela origem das atividades (_Sincronização de CRM_, _Ação de fluxo de campanha_, _Upload de API_, _Preenchimento de formulário de landing page_ etc.). Isso ajuda você a entender se a maioria das suas atividades está sendo produzida por ações de marketing, sincronizações de CRM ou pelas próprias pessoas/leads.
