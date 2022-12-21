---
unique-page-id: 2360401
description: Compare a eficácia do canal com o Analisador de programas - Documentos da Marketo - Documentação do produto
title: Compare a eficácia do canal com o analisador de programas
exl-id: bfe635a7-b077-4074-889d-fc2256102cd5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Compare a eficácia do canal com o analisador de programas {#compare-channel-effectiveness-with-the-program-analyzer}

Use o Analisador de programas para comparar os custos do canal, a aquisição de membros, o pipeline, a receita e muito mais, para identificar seus canais mais e menos eficazes.

>[!PREREQUISITES]
>
>[Criar um analisador de programas](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. Clique em **Analytics** em **Meu Marketo**.

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. Selecione seu **Analisador de programas**.

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. Alterar a Exibição para **Por canal**.

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. Use o **Eixo X** menu suspenso para escolher uma métrica para o eixo horizontal. Vamos começar com **Custo do Programa**.

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. Use o menu suspenso Eixo Y para escolher uma métrica para o eixo vertical. Aqui, vamos com **(FT) Pipeline criado**.

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >Muitas das métricas que você pode escolher no analisador de programas estão disponíveis com cálculos de primeiro toque (FT) e multitoque (MT). É importante entender a variável [diferença entre atribuição FT e MT](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Use o **Eixo Y** menu suspenso a escolher **(MT) Pipeline criado**.

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   Nesta exibição de atribuição multitoque, vemos que o canal de webinar tem mais influência no pipeline criado e custa menos do que os canais de Transmissão e Anúncios online .

   Agora vamos adicionar mais duas dimensões!

1. Use o **Tamanho da bolha** para selecionar uma medida adicional, como **Novos nomes**.

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. Observe como o gráfico muda.

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   Vemos que o canal de webinar encolhe, conforme medido por **Novos nomes**. Podemos concluir que, embora tenha muitos membros, é menos eficaz na geração de novos leads do que o canal de feiras comerciais.

1. Por fim, use o menu suspenso Color para adicionar a quarta dimensão. Vamos selecionar **(FT) Ganho de Receita**.

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. Observe as cores mudarem no seu gráfico.

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   A partir das cores, aprendemos que o canal de shows de vendas, a bolha mais verde, influenciou a maior receita ganha, medida pela atribuição de primeiro toque.

1. Agora, se alterarmos a métrica Cor para **(MT) Receita vencedora**, vemos que o canal de Anúncios online, agora o mais verde, influenciou mais receita ao longo do tempo_ do que os canais de Webinar e Exibição de vendas.

   ![](assets/image2014-9-17-18-3a41-3a40.png)

No nosso exemplo, vemos que o canal de Exibição de vendas é o mais caro (mais à direita) e o mais bem-sucedido (mais alto no eixo Y) ao medir o pipeline criado pelo primeiro toque. Agora, considere o pipeline de cada canal criado como medido pela atribuição de multitoque.

>[!TIP]
>
>Os exemplos nessas etapas avaliam a eficácia com base no pipeline criado. Use o menu suspenso Eixo Y para selecionar outras maneiras de medir a eficácia do canal, como Novos nomes, Membros, Custo por Sucesso etc.

>[!MORELIKETHIS]
>
>* [Explore os detalhes do programa e do canal com o Analisador de programas](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Comparar a eficácia do programa com o Analisador de programas](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-program-effectiveness-with-the-program-analyzer.md)

