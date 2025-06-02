---
description: Painéis de uso de produtos - Documentação do Marketo - Documentação do produto
title: Painéis de uso do produto
hide: true
hidefromtoc: true
feature: Administration
exl-id: a0fa5cd0-a61d-4383-88c0-9f2a4b2c717a
source-git-commit: de396f08c50a1862fbdd3ae1e435ac5671d96b0e
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# Painéis de uso do produto {#product-usage-dashboards}

Os Painéis de uso de produtos do Marketo Engage permitem visualizar o uso do produto e da plataforma em relação a determinados limites ou backlog de taxa de transferência de dados, uso em relação à cota diária e às métricas principais da sua assinatura. A infraestrutura é alocada para fornecer limites de desempenho definidos para níveis de produto para atributos específicos. Alguns desses limites, como o uso da API, são limites contratados comprados como parte do pacote ou da Camada do produto.

## Como acessar {#how-to-access}

1. No Marketo Engage, clique em **Admin**.

   ![](assets/product-usage-dashboards-1.png)

1. Na árvore à esquerda, role para baixo e selecione **Painéis de Uso de Produtos**.

   ![](assets/product-usage-dashboards-2.png)

## Painel de Uso da Atividade {#activity-usage-dashboard}

### Média de atividades semanais {#average-weekly-activities}

O painel Uso semanal de atividade fornece uma contagem semanal de Tipos de atividade em um período contínuo de 52 semanas. As atividades produzidas semanalmente são um bom indicador de quanto marketing você está fazendo no Marketo Engage. As atividades servem como um proxy para os vários processos do sistema e eventos rastreáveis que ocorrem no Marketo.

Os Tipos de atividade incluem contagens de atividades capturadas quando as pessoas/clientes potenciais interagem com eventos de marketing, bem como atividades baseadas no sistema acionadas por Ações de fluxo. Alguns exemplos de atividades iniciadas por pessoas são quando um recipient abre um email enviado por você ou clica em um link em um email. Um exemplo de uma atividade baseada no sistema acionada por uma Ação de Fluxo é _Enviar para a SFDC_ quando o gatilho é iniciado.

>[!TIP]
>
>Para exibir uma contagem dos tipos de atividade para uma semana específica, passe o mouse sobre a semana desejada e a contagem será exibida.

![](assets/product-usage-dashboards-3.png){width="800" zoomable="yes"}

#### Perguntas frequentes {#faq}

**Quais Tipos de Atividade são contados?**

Ela depende das atividades incluídas no pipeline.

**A atividade de pessoa/cliente potencial conhecida e anônima foi incluída?**

Somente pessoas/clientes em potencial conhecidos.

**Com que frequência os dados são atualizados?**

As contagens de atividades são atualizadas todas as manhãs.

## Detalhamento de atividade {#activity-breakdown}

Aqui obtemos contagens de atividades dos últimos sete dias com base em fatias significativas dos dados. Agrupar atividades pelos tipos de atividades mais comuns observados nos últimos sete dias. Isso pode incluir categorias como _Alterar Valor dos Dados_, _Adicionar à Lista_ ou _Enviar Email_. Isso permite que você veja quais tipos de atividades estão acontecendo com mais frequência no sistema. O uso do Tipo de atividade é um indicador importante para determinar o crescimento ou se são necessárias otimizações para reduzir o uso.

>[!NOTE]
>
>* Todos os detalhamentos abaixo são uma soma acumulada de sete dias e **não** incluem o dia atual. Então pense nisso como &quot;ontem + seis dias antes disso.&quot;
>
>* O painel mostra apenas os 20 principais tipos de atividade, enquanto o restante é classificado em uma categoria chamada &quot;Outros&quot;.

![](assets/product-usage-dashboards-4.png){width="800" zoomable="yes"}

O uso da atividade mostra quanto marketing está sendo realizado e ajuda a visualizar o crescimento em relação ao nível de produto contratado para o. Os painéis também podem ser usados como guia para determinar a otimização que pode/deve ser feita ao reduzir os campos que estão sendo atualizados.

### Por tipo {#by-type}

Agrupar atividades pelos tipos de atividades mais comuns observados nos últimos sete dias. Isso pode incluir categorias como _Alterar Valor dos Dados_, _Adicionar à Lista_ ou _Enviar Email_. Isso permite ver quais tipos de atividades estão acontecendo com mais frequência na sua conta do Marketo Engage.

### Por atributo de valor de dados de alteração {#by-change-data-value-attribute}

_Alterar Valor de Dados_ é o tipo de atividade mais comum. Indica quando uma parte das informações em um registro de pessoa/cliente potencial é atualizada. Aqui, agrupamos pelos campos que são alterados com mais frequência para que você possa determinar quais informações são úteis para suas operações de marketing, se há oportunidades para otimizar o uso da plataforma etc.

### Por campanha {#by-campaign}

Grupo pelo qual as campanhas estão produzindo mais atividades. Isso permite ver se você tem campanhas particularmente &quot;barulhentas&quot; que criam mais atividade do que o necessário. Aprenda rapidamente sobre campanhas que devem ser desativadas ou campanhas que estão fazendo mais trabalho do que o esperado.

### Por Source (EM BREVE) {#by-source}

Agrupe pela origem das atividades (_Sincronização de CRM_, _Ação de fluxo de campanha_, _Upload de API_, _Preenchimento de formulário de landing page_ etc.). Isso ajuda você a entender se a maioria das suas atividades está sendo produzida por ações de marketing, sincronizações de CRM ou pelas próprias pessoas/leads.
