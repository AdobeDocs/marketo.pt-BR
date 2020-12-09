---
unique-page-id: 2360389
description: Tornar um Programa sem um custo por período disponível no Gerenciador de receitas e nos Analisadores - Documentos de marketing - Documentação do produto
title: Tornar um Programa sem um custo por período disponível no Gerenciador de receita e nos Analisadores
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---


# Tornar um Programa sem um custo por período disponível no Gerenciador de receita e nos Analisadores {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

Os Custos do período do programa permitem que você defina &quot;Quanto dinheiro&quot; e &quot;Quando&quot; para um programa. Isso aparece no explorador [e](http://docs.marketo.com/display/docs/revenue+cycle+analytics) analisadores [do ciclo de](../../../../product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md)receita.

>[!NOTE]
>
>**Permissões de administrador necessárias**

Alguns programas podem precisar ser incluídos mesmo se não tiverem um custo de período. Embora você possa digitar 0 para o custo do período, tornamos mais fácil incluir esses programas.

>[!NOTE]
>
>O Analisador de Programas classifica o Programa bem-sucedido por custo do período. Se não houver custo de período disponível, o Sucesso do Programa não será exibido, independentemente do comportamento de análise do programa. Se o comportamento do Analytics for configurado, os dados serão exibidos para as métricas de oportunidade (oportunidades de pipeline, receita ganha, etc.).

1. Na seção Admin, clique em Tags.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. Expanda seus Canais e duplos e clique no canal de sua escolha.

   >[!NOTE]
   >
   >**Lembrete**
   >
   >Todos os programas que usam esse canal, independentemente do custo do período, estarão disponíveis para os analisadores e exploradores de receita. Esta alteração entrará em vigor no dia seguinte.

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. Altere o comportamento do Analytics para Inclusivo e clique em Salvar.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>Você notou a opção Operacional? Isso faz o oposto. Exclui esses programas independentemente do custo do período.

Bom trabalho! Agora, qualquer programa que usa o canal modificado será incluído no explorador de receita e nos analisadores sem a necessidade de um custo por período.

>[!MORELIKETHIS]
>
>* [Substituir o comportamento do Analytics no nível do Programa](override-analytics-behavior-at-the-program-level.md)

>



