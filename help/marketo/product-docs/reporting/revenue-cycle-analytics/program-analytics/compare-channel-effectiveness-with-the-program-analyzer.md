---
unique-page-id: 2360401
description: Compare a eficácia do canal com o Analisador de programa - Documentação do Marketo - Documentação do produto
title: Comparar a eficácia do canal com o analisador de programa
exl-id: bfe635a7-b077-4074-889d-fc2256102cd5
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 1%

---

# Compare a eficácia do canal com o [!UICONTROL Analisador de programas] {#compare-channel-effectiveness-with-the-program-analyzer}

Use o [!UICONTROL Analisador de Programas] para comparar os custos de canal, aquisição de membros, pipeline, receita e muito mais, para identificar seus canais mais e menos eficazes.

>[!PREREQUISITES]
>
>[Criar um [!UICONTROL Analisador de Programas]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. Clique no **[!UICONTROL Analytics]** em **Minha Marketo**.

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. Selecione o Analisador de programa.

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. Altere a exibição para **[!UICONTROL Por canal]**.

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. Use o menu suspenso **[!UICONTROL Eixo X]** para escolher uma métrica para o eixo horizontal. Vamos começar com **[!UICONTROL Custo do programa]**.

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. Use o menu suspenso **[!UICONTROL Eixo Y]** para escolher uma métrica para o eixo vertical. Aqui, vamos com o pipeline **[!UICONTROL (FT) criado]**.

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >Muitas das métricas que você pode escolher no analisador de programa estão disponíveis com cálculos de primeiro toque (FT) e multitoque (MT). É importante entender a [diferença entre a atribuição FT e MT](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Use o menu suspenso **[!UICONTROL Eixo Y]** para escolher o Pipeline **[!UICONTROL (MT) Criado]**.

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   Nesta visualização de atribuição multitoque, vemos que o canal de webinário tem mais influência no pipeline criado e custa menos do que os canais de Tradeshow e Advertising online.

   Agora vamos adicionar mais duas dimensões!

1. Use o menu suspenso **[!UICONTROL Tamanho da Bolha]** para selecionar uma medida adicional, como **[!UICONTROL Novos Nomes]**.

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. Veja como o gráfico muda.

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   Vemos que o canal do Webinar fica reduzido, conforme medido por **[!UICONTROL Novos Nomes]**. Podemos concluir que, embora tenha muitos membros, é menos eficaz na geração de novos leads do que o canal Tradeshow.

1. Por fim, use o menu suspenso Cor para adicionar a quarta dimensão. Vamos selecionar **[!UICONTROL (FT) Receita conquistada]**.

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. Veja as cores mudarem no seu gráfico.

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   Com base nas cores, descobrimos que o canal Tradeshow, a bolha mais verde, influenciou a maior receita obtida, medida pela atribuição de primeiro contato.

1. Agora, se alterarmos a métrica de Cor para **[!UICONTROL (MT) Receita Ganha]**, veremos que o canal do Online Advertising, agora o mais ecológico, influenciou mais receita _ao longo do tempo_ do que os canais de Webinar e Tradeshow.

   ![](assets/image2014-9-17-18-3a41-3a40.png)

Em nosso exemplo, vemos que o canal de Tradeshow é o mais caro (mais à direita) e o mais bem-sucedido (mais alto no eixo Y) ao medir o pipeline criado pelo primeiro contato. Agora, vamos considerar o pipeline de cada canal criado como medido pela atribuição multitoque.

>[!TIP]
>
>Os exemplos dessas etapas medem a eficácia com base no pipeline criado. Use o menu suspenso [!UICONTROL Eixo Y] para selecionar outras maneiras de medir a eficácia do canal, como [!UICONTROL Novos Nomes], [!UICONTROL Membros], [!UICONTROL Custo por Sucesso] etc.

>[!MORELIKETHIS]
>
>* [Explore detalhes do programa e do canal com o [!UICONTROL Analisador de programas]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Comparar a eficácia do programa com o [!UICONTROL Analisador de programas]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-program-effectiveness-with-the-program-analyzer.md)
