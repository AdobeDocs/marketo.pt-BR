---
description: Métricas de backlog de sincronização do Salesforce - Documentação do Marketo - Documentação do produto
title: Métricas de backlog de sincronização do Salesforce
hide: true
hidefromtoc: true
feature: Reporting
source-git-commit: 1cc876285f8d7ac7a21a763dd65da34341341a0e
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# Métricas de backlog de sincronização do Salesforce  {#salesforce-sync-backlog-metrics}

A lista de pendências de sincronização representa os registros com sincronização pendente de Salesforce para Marketo Engage e vice-versa. Garantir que o backlog permaneça sob controle resultará em sincronizações tranquilas e oportunas.

>[!NOTE]
>
>A lista de pendências abrange os números de pós-atualizações de sincronização pendentes em ambos os lados, e não aqueles que são realizados pelas etapas de fluxo de sincronização, como as etapas de fluxo [Sincronizar Pessoa com o SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} ou [Sincronizar Pessoa com o Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"}.

## Como acessar o {#how-to-access}

1. No Marketo Engage, vá para a área **Admin**.

   CAPTURA DE TELA

1. Selecione **Salesforce**.

   CAPTURA DE TELA

## Sincronizar Tendência de Backlog {#sync-backlog-trend}

A tendência do acúmulo reflete as alterações nos acúmulos registrados nos últimos cinco dias. O backlog é mostrado em um intervalo de 4 horas distribuído por 5 dias. Portanto, o gráfico mostrará 6 intervalos por dia vezes 5 dias, o que equivale a 30 intervalos.

O backlog é observado em um intervalo de tempo específico de 4 horas no eixo x. Esse valor é para todos os objetos em sincronia. Esse é o total do backlog no Salesforce e no Marketo Engage aguardando para sincronização.

CAPTURA DE TELA

## Throughput de Sincronização e Backlog {#sync-throughput-and-backlog}

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
    <td>Estimativa do tempo necessário para sincronizar o backlog por tipo de objeto. Calculado como 'Sincronizar lista de pendências/média de registros sincronizados por hora.'</td>
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

## O que causa pendências de sincronização {#what-causes-sync-backlogs}

Se a atualização for feita no lado do Marketo Engage ou no lado do CRM, ela acionará o registro para ser ressincronizado para atualizar as informações no outro lado por meio do ciclo regular de sincronização do Marketo Engage para o CRM. Sempre que uma atualização é feita em um registro no Salesforce, ela gera um carimbo de data e hora de modificação do sistema, conhecido como &quot;SysModStamp&quot;. Isso coloca uma alteração na fila para sincronização.

Quando uma grande quantidade de atualizações é feita (como a partir de uma alteração de valor de campo), muitos registros são alterados, causando novos SysModStamps. Um grande número de atualizações de registros de pessoas precisa ser ressincronizado entre o Marketo Engage e o CRM, às vezes criando uma lista de pendências temporária.

## Práticas recomendadas para gerenciar registros pendentes de sincronização {#best-practices}

**Campos sincronizados**: verifique se os campos sincronizados são apenas aqueles que precisam ser sincronizados. As alterações nos campos aumentam o backlog de sincronização e os campos de prioridade mais baixa podem estar parando ou atrasando campos mais importantes em sincronização. Entre em contato com o [Suporte para Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} para remover campos em sincronização.

**Campos sensíveis**: alguns campos têm tendência a atualizações frequentes (por exemplo, campos de moeda que estão sujeitos a alterações de moeda). Verifique se eles precisam ser sincronizados ou se os campos precisam ser criados de forma diferente.

**Objetos personalizados**: revise periodicamente objetos personalizados em sincronia e remova todos os que não precisem mais ser sincronizados.

**Atividades**: verifique se há atividades em sincronização que possam ser removidas da sincronização.

**Agendar atualizações em massa durante horas não críticas**: revise seus padrões de sincronização de dados para identificar períodos não críticos. Veja se as atualizações em massa podem ser agendadas durante esses períodos não críticos.

Se você estiver seguindo todas as práticas recomendadas acima e ainda estiver com listas de pendências significativas, contate o [Suporte de Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
