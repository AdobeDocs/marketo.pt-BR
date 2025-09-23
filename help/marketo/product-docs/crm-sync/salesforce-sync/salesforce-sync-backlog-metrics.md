---
description: Métricas de backlog de sincronização do Salesforce - Documentação do Marketo - Documentação do produto
title: Métricas de lista de pendências de sincronização do Salesforce
feature: Reporting
exl-id: 6b58eb50-ff0d-4774-a232-3ae929948e2a
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# Métricas de lista de pendências de sincronização do Salesforce  {#salesforce-sync-backlog-metrics}

O backlog de sincronização é o nome usado para a sincronização pendente de registros. Conta para registros com sincronização pendente do Salesforce para o Marketo Engage e vice-versa. Garantir que o backlog permaneça sob controle levará a sincronizações suaves e temporais. O backlog cobre os números pendentes de atualizações de publicação de sincronização em ambos os lados, e não aqueles que são realizados pelas etapas de fluxo de sincronização, como o lead de sincronização para as etapas de fluxo do SFDC.

## Como acessar o {#how-to-access}

1. No Marketo Engage, vá para a área **Administrador**.

   ![](assets/salesforce-sync-backlog-metrics-1.png)

1. Selecione **Salesforce**.

   ![](assets/salesforce-sync-backlog-metrics-2.png)

## Sincronizar Tendência de Backlog {#sync-backlog-trend}

A tendência do acúmulo reflete as alterações nos acúmulos registrados nos últimos cinco dias. O backlog é mostrado em um intervalo de 4 horas distribuído por 5 dias. Portanto, o gráfico mostrará 6 intervalos por dia vezes 5 dias, o que equivale a 30 intervalos.

O backlog é observado em um intervalo de tempo específico de 4 horas no eixo x. Esse valor é para todos os objetos em sincronia. Esse é o total do backlog no Salesforce e no Marketo Engage aguardando sincronização.

![](assets/salesforce-sync-backlog-metrics-3.png)

## Throughput de Sincronização e Backlog {#sync-throughput-and-backlog}

As estatísticas refletem a taxa de transferência e o status do backlog para cada tipo de objeto em sincronia nas últimas 24 horas. Os tipos de objeto incluem todos os objetos em sincronização, incluindo: lead, contato, conta, oportunidade, campanha, usuário e objetos personalizados. As estatísticas de taxa de transferência são atualizadas automaticamente a cada 15 minutos, mas você pode atualizar manualmente usando o ícone de atualização. O backlog é obtido a cada hora.

>[!NOTE]
>
>As estatísticas são atualizadas continuamente, não por dia.

![](assets/salesforce-sync-backlog-metrics-4.png)

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
    <td>A lista de pendências de registros com sincronização pendente para o tipo de objeto. É o total da soma da sincronização pendente do backlog em ambas as direções (do Salesforce para o Marketo Engage e vice-versa). O backlog do Salesforce é obtido usando uma chamada de API para o Salesforce e o backlog do Marketo Engage é calculado usando as estatísticas obtidas do log de dados de alteração. Isso é calculado a cada hora. Os próximos dois campos nesta tabela informam quando o backlog foi calculado pela última vez e a próxima programação para cálculo, respectivamente.</td>
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

Se a atualização for feita no Marketo Engage ou no CRM, ela acionará o registro para ser ressincronizado para atualizar as informações na outra extremidade por meio do ciclo de sincronização normal do Marketo Engage para o CRM. Sempre que uma atualização é feita em um registro no Salesforce, ela gera um carimbo de data e hora de modificação do sistema, conhecido como &quot;SysModStamp&quot;. Isso coloca uma alteração na fila para sincronização.

Quando uma grande quantidade de atualizações é feita (como a partir de uma alteração de valor de campo), muitos registros são alterados, causando novos SysModStamps. Um grande número de atualizações de registros de pessoas precisa ser ressincronizado entre o Marketo Engage e o CRM, às vezes criando um backlog momentâneo.

## Práticas recomendadas para gerenciar registros pendentes de sincronização {#best-practices}

**Campos visíveis para o Usuário de Sincronização**: verifique se os campos visíveis para sincronização são apenas aqueles que precisam ser sincronizados e têm valor para esforços de marketing. Qualquer atualização em um registro no Salesforce que atualize o carimbo de data e hora da última modificação enfileirará um registro no backlog de sincronização, e a sincronização de campos desnecessários poderá retardar campos mais importantes em sincronização. Se os campos desnecessários estiverem ocultos do usuário de sincronização, as atualizações nesses campos resultarão em um salto muito mais rápido do que uma atualização. Trabalhe com seu administrador do Salesforce para analisar as práticas recomendadas [aqui](https://nation.marketo.com/t5/marketo-whisperer-blogs/best-practices-for-determining-which-fields-to-sync-with-marketo/ba-p/247449){target="_blank"} e atualizar quais campos estarão visíveis para o Usuário de Sincronização do Marketo.

**Ocultar ou filtrar registros desnecessários**: se um registro não for comercializável, poderá estar desperdiçando recursos de sincronização. Se o usuário de sincronização não conseguir vê-la, então não desperdiçará recursos tentando sincronizá-la. O [Suporte do Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support#_blank){target="_blank"} pode ajudar a configurar um filtro de sincronização para impedir que os registros sejam sincronizados com base em critérios adicionais. Mais informações sobre como configurar um Filtro de Sincronização Personalizado [podem ser encontradas aqui](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"}. É altamente recomendável usar campos de índice no Salesforce (entre em contato com a salesforce para obter mais informações).

**Agendar atualizações em massa durante horas não críticas**: revise seus padrões de sincronização de dados para identificar períodos não críticos. Verifique se as atualizações em massa podem ser agendadas nesses períodos não críticos, se possível.

**Campos Atualizados com Frequência**: alguns campos estão sujeitos a atualizações frequentes. Por exemplo, campos de moeda que estão sujeitos a alterações de moeda. Verifique se eles precisam ser sincronizados ou se os campos devem ser criados de forma diferente. Se você tiver outros campos que são atualizados com frequência e não são necessários, oculte-os do usuário de sincronização. Certifique-se de discutir com suas integrações de administrador do SFDC que podem estar atualizando campos.

**Objetos personalizados**: revise periodicamente [objetos personalizados](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync){target="_blank"} habilitados para sincronizar e desabilitar aqueles que não precisam mais ser sincronizados.

**Atividades**: [Verifique se alguma atividade](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync){target="_blank"} habilitou a sincronização que possa ser removida da sincronização.  Essas atividades só são sincronizadas uma vez por dia por lead.

**Revisar erros de sincronização**: a manipulação de exceções pode retardar a sincronização. A revisão das notificações do usuário e a resolução de erros podem melhorar a integridade da sincronização.

**Contate o Suporte**: se você estiver seguindo todas as práticas recomendadas acima e ainda estiver com listas de pendências significativas, contate o [Suporte da Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support#_blank){target="_blank"}.
