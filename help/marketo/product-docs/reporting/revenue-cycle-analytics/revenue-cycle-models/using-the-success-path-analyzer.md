---
unique-page-id: 3571886
description: Uso do Analisador de caminho de sucesso - Documentação do Marketo - Documentação do produto
title: Uso do Analisador de caminho de sucesso
exl-id: f816b7ac-a158-46bd-9d00-09ef4cc8b381
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Uso do Analisador de caminho de sucesso {#using-the-success-path-analyzer}

Use um Analisador de Caminho de Sucesso para explorar os detalhes específicos que refletem o fluxo (quantidade) e a velocidade (velocidade, em termos de dias) das pessoas pelos estágios do seu [Modelo de Ciclo de Receita](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).

>[!PREREQUISITES]
>
>[Criar um Analisador de Caminho de Êxito](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/create-a-success-path-analyzer.md)

1. Vá para **Analytics** e selecione seu **Analisador de caminho de sucesso**.

   ![](assets/image2015-6-12-17-3a23-3a53.png)

   O gráfico à direita reflete os dados no botão selecionado à esquerda. Por padrão, esse é Saldo.

1. Clique em **Em Fluxo** para gerar um gráfico com o número de pessoas que entraram no estágio durante o período selecionado.

   ![](assets/image2015-6-12-17-3a30-3a52.png)

   * Clique em Fluxo de saída para criar um gráfico com o número de pessoas que saíram do estágio.
   * Clique em Conv % para criar um gráfico da taxa de conversão desta fase para a próxima.
   * Clique em Tempo Médio para ver quanto tempo as pessoas passaram nesse estágio antes de passar para o próximo estágio.

1. Clique em **Ações de Gráfico** > Comparar Período para comparar os dados a um período diferente de igual duração.

   ![](assets/image2015-6-12-17-3a39-3a15.png)

1. Selecione a data **De** para o período de comparação.

   ![](assets/image2015-6-12-17-3a43-3a49.png)

   A data **Para** é automaticamente definida para corresponder à duração do seu período original.

1. Clique em **Comparar**.

   ![](assets/image2015-6-12-17-3a44-3a8.png)

1. O gráfico é atualizado com dados sobrepostos para o período de comparação, em verde.

   ![](assets/image2015-6-12-17-3a46-3a16.png)

1. Para alterar a escala de tempo do gráfico, clique em um dos botões **Gráfico por**: diário (padrão), semanal e mensal

   ![](assets/image2015-6-12-17-3a46-3a55.png)

1. Para estágios com SLAs (Contratos de Nível de Serviço), clique em **Gráfico de Ações** > **Mostrar SLA Devido** para mostrar todas as pessoas que perderam um destino de SLA no período especificado.

   ![](assets/image2015-6-12-17-3a49-3a23.png)

1. O gráfico é atualizado para refletir quantos SLAs estavam vencidos em cada nó, em laranja.

   ![](assets/image2015-6-12-17-3a50-3a16.png)

   As pessoas mostradas em laranja podem *ou não* ainda estar no estágio de SLA.

1. Clique em **Ações de Gráfico** > **Mostrar SLA em Atraso** para mostrar todas as pessoas com destinos de SLA expirados que ainda estão no estágio de SLA no final do período especificado.

   ![](assets/image2015-6-12-17-3a51-3a39.png)

1. O gráfico é atualizado para refletir quantos SLAs estavam vencidos em cada nó, em laranja.

   ![](assets/image2015-6-12-17-3a52-3a17.png)

1. Para ler os detalhes específicos de um ponto de dados em um nó específico (data), passe o mouse sobre a bolha.

   ![](assets/image2015-6-12-17-3a52-3a49.png)

1. Para imprimir o gráfico, clique em **Ações de Gráfico** > **Imprimir Gráfico**.

   ![](assets/image2015-6-12-17-3a53-3a34.png)

O analisador está aqui para ajudá-lo a entender o movimento pelo seu modelo. À medida que você se torna mais avançado, isso se tornará realmente importante para criar estratégias de esforços de marketing.
