---
unique-page-id: 2360389
description: Disponibilizar um programa sem um custo de período no Gerenciador e analisadores de receita - Documentação do Marketo - Documentação do produto
title: Disponibilizar um programa sem um custo de período no Gerenciador e nos Analisadores de receita
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Disponibilizar um programa sem um custo de período no Gerenciador e nos Analisadores de receita {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

Custos do período de programa permitem definir &quot;Quanto dinheiro&quot; e &quot;Quando&quot; para um programa. Isso é exibido no Gerenciador de Ciclo de Receita e em [analisadores](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md).

>[!NOTE]
>
>**Permissões de administrador necessárias**

Alguns programas podem precisar ser incluídos mesmo se não tiverem um custo de período. Embora você possa inserir 0 para o custo do período, facilitamos a inclusão desses programas.

>[!NOTE]
>
>O Analisador de programas classifica o Sucesso do programa por custo do período. Se não houver custo do período disponível, o Êxito do programa não será exibido, independentemente do comportamento analítico do programa. Se o comportamento de análise for configurado, os dados serão exibidos para as métricas de oportunidade (oportunidades de pipeline, receita ganha etc.).

1. Na seção [!UICONTROL Admin], clique em **[!UICONTROL Marcas]**.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. Expanda os Canais e clique duas vezes no canal de sua escolha.

   >[!NOTE]
   >
   >Todos os programas que usam esse canal, independentemente do custo do período, ficarão disponíveis para o explorador de receita e os analisadores. Essa alteração entrará em vigor no dia seguinte.

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. Altere o [!UICONTROL Comportamento do Analytics] para **Inclusivo** e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>Você notou a opção Operacional? Isso faz o oposto. Ele exclui esses programas independentemente do custo do período.

Excelente! Agora, qualquer programa que use o canal modificado será incluído no explorador de receita e nos analisadores sem a necessidade de um custo de período.

>[!MORELIKETHIS]
>
>[Substituir comportamento do Analytics no nível do programa](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)
