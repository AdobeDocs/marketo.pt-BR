---
unique-page-id: 2360389
description: Disponibilizar um programa sem um custo por período no Explorador de receita e nos Analisadores - Documentos da Marketo - Documentação do produto
title: Disponibilizar um programa sem um custo por período no Explorador e Analisadores de Receita
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Disponibilizar um programa sem um custo por período no Explorador e Analisadores de Receita {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

Período do programa Os custos permitem definir &quot;Quanto dinheiro&quot; e &quot;Quando&quot; para um programa. Isso é exibido no Explorador do Ciclo de Receita e [analisadores](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md).

>[!NOTE]
>
>**Permissões de administrador necessárias**

Alguns programas podem precisar ser incluídos mesmo que não tenham um custo de ponto. Embora você possa inserir 0 para o custo do período, facilitamos a inclusão desses programas.

>[!NOTE]
>
>O Analisador de programas classifica o Sucesso do programa por custo do período. Se não houver custo de período disponível, o sucesso do programa não será exibido, independentemente do comportamento de análise do programa. Se o comportamento de análise for configurado, os dados serão exibidos para métricas de oportunidade (oportunidades de pipeline, receita ganha, etc.).

1. Na seção Admin , clique em **Tags**.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. Expanda os Canais e clique duas vezes no canal de sua escolha.

   >[!NOTE]
   >
   >Todos os programas que usam esse canal, independentemente do custo do período, ficarão disponíveis para exploradores e analisadores de receita. Essa alteração entrará em vigor no dia seguinte.

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. Altere o comportamento do Analytics para Inclusivo e clique em **Salvar**.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>Você notou a opção Operacional? Isso faz o contrário. Exclui estes programas independentemente do custo do período.

Excelente! Agora, qualquer programa que use o canal modificado será incluído no explorador e analisadores de receita sem a necessidade de um custo de período.

>[!MORELIKETHIS]
>
>[Substituir o comportamento do Analytics no nível do programa](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)
