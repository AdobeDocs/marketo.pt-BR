---
unique-page-id: 7504676
description: Noções básicas sobre custos de período - Documentos do Marketo - Documentação do produto
title: Noções básicas sobre custos de período
exl-id: 99f50eaf-28cf-4a8b-8ebd-89a4beef986a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Noções básicas sobre custos de período {#understanding-period-costs}

## Visão geral {#overview}

Os custos do período se referem ao dinheiro que você gastou em um mês específico em um programa.

>[!NOTE]
>
>**Exemplo**
>
>Se você gastar US$ 1.000 para contratar um ilustrador para um eBook que será lançado em julho - o programa eBook teria um custo de US$ 1.000 no período de julho.
>
>Se você gastar US$ 200 por mês no Google AdWords - o programa Google AdWords teria um custo de período de US$ 200 **todo mês**.

>[!NOTE]
>
>[Noções básicas sobre programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[Compreensão da assinatura do programa](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## Como os custos do período são calculados {#how-period-costs-are-calculated}

Imagine um evento, como um webinário, que ocorre em março. Novas pessoas são adquiridas previamente com a publicidade em janeiro e fevereiro. Novos contatos também são adquiridos depois do evento, quando as pessoas baixam o webinário nos meses de abril e maio.

1. Com um único custo de período atribuído a março..

   ![](assets/graph1.png)

   ...contatos adicionados nos meses anteriores e posteriores *only* conte para março.

   ![](assets/graph2.png)

1. Com custos de período atribuídos a janeiro, fevereiro e março..

   ![](assets/graph3.png)

   ...os contatos adicionados somente nos meses seguintes a março contarão até março.

   ![](assets/graph4.png)

1. Com custos de período atribuídos a janeiro e abril...

   ![](assets/graph5.png)

   ...os contatos adicionados nos meses de janeiro a março contarão até janeiro. Contatos adicionados nos meses de abril e maio contarão até abril.

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >Em resumo - meses sem custos de período definidos serão revertidos para o último que foi definido. Se não houver custo de período anterior, os meses serão encaminhados &quot;para a frente&quot; para o próximo que foi definido. Se um custo de período não tiver sido definido para _any_ meses, os relatórios no RCE não estarão disponíveis para o programa.

   >[!MORELIKETHIS]
   >
   >* [Uso de Custos de Período em um Programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [Filtrar um Relatório de Programa por Custo de Período](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)

