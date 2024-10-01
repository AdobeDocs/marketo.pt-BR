---
description: Painel de métricas de observação de sincronização do Salesforce - Documentação do Marketo - Documentação do produto
title: Painel de métricas de observação de sincronização do Salesforce
hide: true
hidefromtoc: true
feature: Reporting
source-git-commit: 2457f0f51c6365c29a040e908678e81517327de5
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Métricas de backlog de sincronização do Salesforce  {#salesforce-sync-backlog-metrics}

Revise suas taxas de transferência de desempenho de sincronização e sincronize listas de pendências com este painel.

## Throughput de Sincronização e Backlog {#sync-throughput-and-backlog}

1. No Marketo Engage, vá para a área Admin.

   CAPTURA DE TELA

1. Selecione Salesforce.

   CAPTURA DE TELA

As estatísticas refletem a taxa de transferência e o status do backlog para cada tipo de objeto em sincronia nas últimas 24 horas. Os tipos de objeto incluem todos os objetos em sincronização, incluindo: lead, contato, conta, oportunidade, campanha, usuário e objetos personalizados. As estatísticas de taxa de transferência são atualizadas automaticamente a cada 15 minutos, mas você pode atualizar manualmente usando o ícone de atualização. O backlog é obtido a cada hora.

>[!NOTE]
>
>As estatísticas são atualizadas continuamente, não por dia.

CAPTURA DE TELA

<table><thead>
  <tr>
    <th>Campo</th>
    <th>Descrição</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Máximo de registros sincronizados/h</td>
    <td>O número máximo de registros sincronizados por hora (taxa de transferência máxima) observado nas últimas 24 horas para o tipo de objeto. O período de 24 horas é acumulado com o tempo, não com o dia do calendário.</td>
  </tr>
  <tr>
    <td>Mínimo de registros sincronizados/h</td>
    <td>O número mínimo de registros sincronizados por hora (taxa de transferência mínima) observado nas últimas 24 horas para o tipo de objeto. O período de 24 horas é acumulado com o tempo, não com o dia do calendário.</td>
  </tr>
  <tr>
    <td>Média de registros sincronizados/h</td>
    <td>O número médio de registros sincronizados por hora (taxa de transferência mínima) observado nas últimas 24 horas para o tipo de objeto. O período de 24 horas é acumulado com o tempo, não com o dia do calendário. Isso é calculado como o número total de registros sincronizados nas últimas 24 horas.</td>
  </tr>
  <tr>
    <td>Sincronizar backlog</td>
    <td>A lista de pendências de registros com sincronização pendente para o tipo de objeto. É a soma total da sincronização pendente do backlog em ambas as direções (de Salesforce para Marketo Engage e vice-versa). O backlog do Salesforce é obtido usando uma chamada de API para o Salesforce e o backlog do Marketo Engage é calculado usando as estatísticas obtidas do log de dados de alteração. Isso é calculado a cada hora. Os próximos dois campos nesta tabela informam quando o backlog foi calculado pela última vez e a próxima programação para cálculo, respectivamente.</td>
  </tr>
  <tr>
    <td>Backlog estimado (tempo)</td>
    <td>Estimativa do tempo necessário para sincronizar o backlog por tipo de objeto. Calculado como Sincronizar registros de lista de pendências/Média de registros sincronizados por hora.</td>
  </tr>
  <tr>
    <td>Última busca de lista de pendências</td>
    <td>A hora do último cálculo de backlog.</td>
  </tr>
  <tr>
    <td>Próxima busca da lista de pendências</td>
    <td>A hora do próximo cálculo de backlog.</td>
  </tr>
  <tr>
    <td>Status do Backlog</td>
    <td>Isso mostra se o acúmulo aumentou nas últimas 6 horas. É inferido como "Crescente" se o backlog atual for maior que o backlog registrado 6 horas atrás. Caso contrário, será mostrado como 'Normal'. O objetivo é mostrar se a taxa de transferência de sincronização está alcançando o backlog.</td>
  </tr>
</tbody></table>

## Tendência do Backlog {#backlog-trend}

A tendência do acúmulo reflete as alterações nos acúmulos registrados nos últimos cinco dias. O backlog é mostrado em um intervalo de 4 horas distribuído por 5 dias. Portanto, o gráfico mostrará 6 intervalos por dia vezes 5 dias, o que equivale a 30 intervalos.

O backlog é observado em um intervalo de tempo específico de 4 horas no eixo x. Esse valor é para todos os objetos em sincronia. Esse é o total do backlog no Salesforce e no Marketo Engage aguardando para sincronização.

CAPTURA DE TELA
