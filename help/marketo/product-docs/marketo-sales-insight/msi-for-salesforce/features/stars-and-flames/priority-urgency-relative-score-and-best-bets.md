---
unique-page-id: 2950396
description: Prioridade, Urgência, Pontuação relativa e Melhores Opções - Documentação do Marketo - Documentação do produto
title: Prioridade, urgência, pontuação relativa e melhores opções
exl-id: 391aae00-e4f5-4fb1-8728-f5224276dfc2
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 2%

---

# Prioridade, Urgência, Pontuação Relativa e [!DNL Best Bets] {#priority-urgency-relative-score-and-best-bets}

O [!DNL Marketo Sales Insight] escolhe seus melhores clientes em potencial e contatos com base em suas prioridades. A prioridade de um cliente potencial ou contato tem dois componentes: urgência e pontuação relativa.

![](assets/priority-urgency-relative-score-and-best-bets-1.png)

Eles são derivados da pontuação de lead — uma medida do interesse da pessoa em seu(s) produto(s). Quanto maior a pontuação, mais provável eles responderão positivamente a uma chamada da equipe de vendas.

>[!NOTE]
>
>Você precisa de várias campanhas de pontuação para obter o valor completo de prioridade, urgência e pontuação relativa.  Com poucas ou nenhuma campanha de pontuação, esses campos não serão úteis.

## Urgência {#urgency}

As chamas representam urgência — o quanto o lead score dessa pessoa mudou recentemente. Uma alta urgência (mais chamas) significa que a pontuação deste lead aumentou muito ultimamente; é um bom sinal que este lead esteja interessado em sua oferta. Você deve entrar em contato com esta pessoa rapidamente!

Por exemplo, um lead que solicitou uma demonstração e visitou várias páginas da Web provavelmente terá uma urgência muito alta. Um lead que não visitou sua página da Web ou abriu seus emails terá uma urgência baixa. Use a urgência para priorizar quem precisa ser contatado em seguida.

![](assets/priority-urgency-relative-score-and-best-bets-2.png)

## Pontuação relativa {#relative-score}

As estrelas representam pontuação relativa — uma medida de como a pontuação de leads dessa pessoa se compara à de outras pessoas. Uma pontuação relativa alta significa que essa pessoa provavelmente está mais interessada e informada sobre sua oferta em comparação às pessoas com pontuações relativas mais baixas.

Se dois leads tiverem a mesma urgência, você poderá usar a pontuação relativa para saber qual deles merece uma chamada telefônica primeiro. Aquele com a pontuação relativa mais alta pode reagir mais favoravelmente à sua oferta em relação ao menor.

## [!DNL Best Bets] {#best-bets}

Seus [!DNL Best Bets] são seus clientes em potencial e contatos com a maior urgência e pontuação relativa. Somente os clientes em potencial que você possui estão visíveis nessa lista, e ela é atualizada conforme as pontuações dos clientes em potencial mudam.

>[!NOTE]
>
>Se suas melhores opções não corresponderem aos seus clientes em potencial e contatos, fale com alguém da sua empresa que tenha acesso à Marketo sobre a atualização das suas [Regras de Pontuação](/help/marketo/getting-started/quick-wins/simple-scoring.md).

### Como a urgência e a pontuação relativa são calculadas

Para calcular o número de estrelas e chamas, seus leads e contatos são classificados primeiro por pontuação ou alteração de pontuação (para Pontuação relativa e Urgência, respectivamente). Então eles são divididos em camadas — a camada de cima recebe mais estrelas ou chamas, a próxima recebe menos, e assim por diante.

À medida que as pontuações mudam, os valores de urgência, prioridade e pontuação relativa são recalculados imediatamente. Os níveis de urgência e pontuação relativa são calculados automaticamente todas as noites nos servidores da Marketo.

>[!NOTE]
>
>A Urgência relativa (chamas) e a Pontuação relativa (estrelas) são números inteiros no Marketo. Os valores possíveis para cada são 0-3.
