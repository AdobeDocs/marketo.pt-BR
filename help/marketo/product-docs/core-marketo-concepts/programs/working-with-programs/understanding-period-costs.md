---
unique-page-id: 7504676
description: Entendendo os custos do período - Documentos do marketing - Documentação do produto
title: Noções básicas sobre os custos do período
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# Noções básicas sobre os custos do período {#understanding-period-costs}

## Visão geral {#overview}

Os custos do período se referem ao dinheiro que você gasta em um mês específico em um programa.

>[!NOTE]
>
>**Exemplo**
>
>Se você gastar US$ 1.000 para contratar um ilustrador para um eBook que será lançado em julho - o programa do eBook terá um custo de US$ 1.000 em julho.
>
>Se você gastar $200 por mês no Google Adwords - o programa Google Adwords terá um custo de período de $200 **a cada mês**.

>[!NOTE]
>
>[Como entender Programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[Compreensão da associação ao Programa](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## Como os custos do período são calculados {#how-period-costs-are-calculated}

Imagine um evento, como um webinar, que ocorre em março. Novas pessoas são adquiridas antecipadamente com publicidade em janeiro e fevereiro. Novos contatos também são adquiridos após o evento, quando as pessoas baixam o webinar nos meses de abril e maio.

1. Com um custo de período único atribuído a março..

   ![](assets/graph1.png)

   ...os contatos adicionados nos meses anteriores e posteriores serão contados *somente* até março.

   ![](assets/graph2.png)

1. Com os custos do período atribuídos a janeiro, fevereiro e março...

   ![](assets/graph3.png)

   ...os contatos adicionados apenas nos meses seguintes a março contarão para março.

   ![](assets/graph4.png)

1. Com os custos do período atribuídos a Janeiro e abril...

   ![](assets/graph5.png)

   ...os contatos adicionados nos meses de Janeiro a março contam para Janeiro. Os contatos adicionados nos meses de abril e maio contarão até abril.

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >Resumindo, os meses sem um período definido serão revertidos para trás até ao último que foi definido. Se não houver custo do período anterior, os meses serão encaminhados &quot;para a frente&quot; para o próximo que tiver sido definido. Se um custo de período não tiver sido definido para _qualquer_ meses, o relatórios em RCE não estará disponível para o programa.

   >[!MORELIKETHIS]
   >
   >* [Uso dos custos do período em um Programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [Filtrar um Relatório de Programa por Custo de Período](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)

