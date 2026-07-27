---
description: Saiba como as políticas de retenção de dados de 25 meses e 90 dias do Marketo afetam os relatórios do Analytics, com um detalhamento por relatório e dicas para reter dados por mais tempo.
title: Retenção de dados
feature: Reporting
source-git-commit: 8eb9fd285e5dd055603579fbb5e7a4c4eb681172
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 5%

---

# Política de retenção de dados de atividades do Marketo - Impacto nos relatórios

O Marketo mantém os dados da atividade de marketing continuamente. Os dados de Atividade e Associação de campanha são armazenados por um período contínuo de 25 meses após a data da atividade, e os dados de atividades de alto volume são retidos por um período contínuo de 90 dias após a data da atividade por padrão, que pode ser ajustado por usuário. Além desses períodos de retenção, os dados não estarão mais disponíveis por meio da interface do usuário do Marketo.

## Relatórios do Marketo Analytics

Como os dados da atividade são retidos por até 25 meses, alguns relatórios do Marketo Analytics são afetados por essa política, enquanto outros não. Os relatórios que coletam dados de logs de atividades de pessoas só mostrarão dados de até 25 meses. Os relatórios que não fazem referência à atividade da pessoa não são afetados.

No entanto, até mesmo os relatórios que não fazem referência à atividade de pessoa por padrão podem ser afetados se os filtros forem adicionados à lista inteligente do relatório. Os filtros que fazem referência aos atributos da pessoa (informações nos campos no registro da pessoa) não causam qualquer alteração no relatório. Os filtros que procuram atividades que a pessoa realizou só podem acessar atividades dentro da janela de retenção, portanto, se a atividade tiver ocorrido há mais tempo do que isso, os resultados do relatório serão alterados.

A tabela abaixo resume como cada relatório se comporta, incluindo cenários de filtro comuns.

## Referência do relatório

| Tipo de relatório | Filtrar cenário | Afetado pela política de retenção? |
|---|---|---|
| **Relatórios do Gerenciador de Ciclo de Receita** | Nenhum filtro disponível | Não: os usuários do Revenue Cycle Explorer e do Advanced Analytics são totalmente isentos desses limites de retenção. Os dados de RCE são enviados durante a noite para um servidor de banco de dados separado que gerencia os relatórios de RCE. Como são alojados separadamente, e não em registros de atividades pessoais, esses relatórios não são afetados por essa política. O Gerenciador de ciclo de receita não extrai dados do banco de dados de pessoas diretamente, portanto, os filtros não estão disponíveis. |
| **Relatório de Desempenho de Pessoas** | Nenhum filtro de lista inteligente | Não |
| | Filtros em atributos de pessoa (Ex: Nome) | Não |
| | Filtros em atividades de pessoas nos últimos 25 meses | Não |
| | Filtros em atividades de pessoas sem restrição de data | Sim |
| **Pessoas por Status** | Nenhum filtro de lista inteligente | Não |
| | Filtros em atributos de pessoa (Ex: Nome) | Não |
| | Filtros em atividades de pessoas nos últimos 25 meses | Não |
| | Filtros em atividades de pessoas sem restrição de data | Sim |
| **Pessoas por estágio de receita** | Nenhum filtro de lista inteligente | Não |
| | Filtros em atributos de pessoa (Ex: Nome) | Não |
| | Filtros em atividades de pessoas nos últimos 25 meses | Não |
| | Filtros em atividades de pessoas sem restrição de data | Sim |
| **Analisador de Caminho de Sucesso** | Não inclui Smart Lists | N/A |
| **Relatório de Influência Social** | Nenhum filtro de lista inteligente | Sim |
| | Filtros em atributos de pessoa (Ex: Nome) | Sim |
| | Filtros em atividades de pessoas nos últimos 25 meses | Sim |
| | Filtros em atividades de pessoas sem restrição de data | Sim |
| **Analisador de Influência da Oportunidade** | Não inclui Smart Lists | Não |
| **Desempenho do email** | Nenhum filtro de lista inteligente | Não |
| | Filtros em atributos de pessoa (Ex: Nome) | Não |
| | Filtros em atividades de pessoas nos últimos 25 meses | Não |
| | Filtros em atividades de pessoas sem restrição de data | Sim |
| **Desempenho do Link de Email** | Nenhum filtro de lista inteligente | Não |
| | Filtros em atributos de pessoa (Ex: Nome) | Não |
| | Filtros em atividades de pessoas nos últimos 25 meses | Não |
| | Filtros em atividades de pessoas sem restrição de data | Sim |
| **Email Insights** | Não usa Smart Lists | Não |
| **Desempenho de email do Sales Insight** | Nenhum filtro de lista inteligente | Não |
| | Filtros em atributos de pessoa (Ex: Nome) | Não |
| | Filtros em atividades de pessoas nos últimos 25 meses | Não |
| | Filtros em atividades de pessoas sem restrição de data | Sim |
| **Desempenho da página de aterrissagem** | Nenhum filtro de lista inteligente | Não: os dados de Desempenho da página de aterrissagem são retidos indefinidamente e não estão sujeitos à política de retenção. |
| | Filtros em atributos de pessoa (Ex: Nome) | Não |
| | Filtros em atividades de pessoas nos últimos 25 meses | Não |
| | Filtros em atividades de pessoas sem restrição de data | Não |
| **Atividade da página da Web** | Nenhum filtro de lista inteligente | Sim: sujeito ao período de retenção padrão de 90 dias (ajustável por usuário) |
| | Filtros em atributos de pessoa (Ex: Nome) | Sim |
| | Filtros em atividades de pessoas nos últimos 25 meses | Sim |
| | Filtros em atividades de pessoas sem restrição de data | Sim |
| **Atividade da empresa na Web** | Nenhum filtro de lista inteligente | Sim |
| | Filtros em atributos de pessoa (Ex: Nome) | Sim |
| | Filtros em atividades de pessoas nos últimos 25 meses | Sim |
| | Filtros em atividades de pessoas sem restrição de data | Sim |
| **Desempenho do Programa** | Nenhum filtro de lista inteligente | Não |
| | Filtros em atributos de pessoa (Ex: Nome) | Não |
| | Filtros em atividades de pessoas nos últimos 25 meses | Não |
| | Filtros em atividades de pessoas sem restrição de data | Sim |
| **Desempenho do Fluxo de Engajamento** | Nenhum filtro de lista inteligente | Não |
| | Filtros em atributos de pessoa (Ex: Nome) | Não |
| | Filtros em atividades de pessoas nos últimos 25 meses | Não |
| | Filtros em atividades de pessoas sem restrição de data | Sim |
| **Analisador de programas** | Não usa Smart Lists | Não |
| **Atividade de campanha** | Nenhum filtro de lista inteligente | Não |
| | Filtros em atributos de pessoa (Ex: Nome) | Não |
| | Filtros em atividades de pessoas nos últimos 25 meses | Não |
| | Filtros em atividades de pessoas sem restrição de data | Sim |
| **Desempenho do Email da Campanha** | Nenhum filtro de lista inteligente | Sim |
| | Filtros em atributos de pessoa (Ex: Nome) | Sim |
| | Filtros em atividades de pessoas nos últimos 25 meses | Sim |
| | Filtros em atividades de pessoas sem restrição de data | Sim |

## Soluções alternativas para relatórios

Muitos usuários podem considerar os dados de atividade anteriores à janela de retenção obsoletos. No entanto, você pode ter um caso de uso em que essas informações são necessárias. Veja a seguir maneiras de reter esses dados além do período de retenção padrão.

## Exportar os dados

A Marketo oferece a [API REST de extração em massa](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/bulk-extract/bulk-extract), que permite exportar atividades de pessoas e hospedá-las localmente. Depois que os dados forem extraídos por meio da API, você poderá armazená-los e classificá-los da maneira que precisar para o caso de uso.

>[!TIP]
>
>Exporte seus dados pessoais de acordo com uma programação regular, não apenas uma vez. As atividades de pessoa são retidas em um ciclo contínuo de 25 meses. Defina um lembrete para exportar novamente _antes_ do final desse período de 25 meses.

## Usar campos personalizados

Os valores do campo Pessoa não são afetados pela Política de retenção de dados. Você pode usar as Campanhas inteligentes para preencher campos personalizados com valores com base nas atividades realizadas por seu pessoal. Isso permite que você filtre as pessoas por esses atributos de pessoa (não sujeitos à política de retenção) em vez das próprias atividades (que estão sujeitas à política de retenção).

Um benefício adicional dessa abordagem é que a pesquisa por atributos de pessoa é mais rápida do que a pesquisa por meio de logs de atividades de pessoa.
