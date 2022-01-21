---
unique-page-id: 2950396
description: Prioridade, urgência, pontuação relativa e melhores propostas - Documentos do Marketo - Documentação do produto
title: Prioridade, urgência, pontuação relativa e melhores propostas
exl-id: 391aae00-e4f5-4fb1-8728-f5224276dfc2
source-git-commit: 15263f9c23c958499aaa2e4e6491b4962c617358
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 1%

---

# Prioridade, urgência, pontuação relativa e melhores propostas {#priority-urgency-relative-score-and-best-bets}

O Marketo Sales Insight escolhe seus melhores leads e contatos com base em sua prioridade. A prioridade de um cliente potencial ou contato tem dois componentes: urgência e pontuação relativa.

![](assets/priority-urgency-relative-score-and-best-bets-1.png)

Elas são derivadas da pontuação do lead — uma medida do interesse da pessoa em seus produtos. Quanto maior a pontuação, mais provavelmente responderão positivamente a uma chamada da sua equipe de vendas.

>[!NOTE]
>
>Você precisa de várias campanhas de pontuação para obter o valor total de prioridade, urgência e pontuação relativa.  Com muito poucas ou nenhuma campanha de pontuação, esses campos não serão úteis.

## Urgência {#urgency}

As chamas representam urgência — quanto a pontuação de liderança desta pessoa mudou recentemente. A alta urgência (mais chamas) significa que a pontuação deste chumbo tem aumentado muito ultimamente; é um bom sinal de que esse cliente potencial está interessado em sua oferta. Você deveria acompanhar esta pessoa rapidamente!

Por exemplo, um cliente potencial que solicitou uma demonstração e visitou várias páginas da Web provavelmente terá uma urgência muito alta. Um cliente potencial que não visitou sua página da Web ou abriu seus emails terá baixa urgência. Use a urgência para priorizar quem precisa ser contatado em seguida.

![](assets/priority-urgency-relative-score-and-best-bets-2.png)

## Pontuação relativa {#relative-score}

As estrelas representam uma pontuação relativa - uma medida de como a pontuação de liderança dessa pessoa se compara à de todos os outros. Uma pontuação relativa alta significa que essa pessoa provavelmente está mais interessada e informada sobre sua oferta em comparação com pessoas com pontuações relativas mais baixas.

Se dois leads tiverem a mesma urgência, você pode usar uma pontuação relativa para saber qual deles merece uma chamada telefônica primeiro. O com pontuação relativa mais alta pode reagir de forma mais favorável à sua oferta em vez da menor.

## Melhores opções {#best-bets}

Suas Melhores Apostas são seus leads e contatos com a maior urgência e pontuação relativa. Somente os leads que você tem são visíveis nessa lista e a lista é atualizada à medida que as pontuações do lead mudam.

>[!NOTE]
>
>Se suas melhores apostas não corresponderem aos melhores clientes potenciais e contatos de sua propriedade, fale com alguém de sua empresa que tenha acesso ao Marketo sobre como atualizar seu [Regras de pontuação](/help/marketo/getting-started/quick-wins/simple-scoring.md).

### Como a urgência e a pontuação relativa são calculadas

Para calcular o número de estrelas e chamas, seus leads e contatos são classificados primeiro por pontuação ou alteração de pontuação (para Pontuação relativa e Urgência, respectivamente). Depois dividem-se em camadas — a camada superior recebe a maioria das estrelas ou chamas, a próxima recebe menos, e assim por diante.

Conforme as pontuações mudam, urgência, prioridade e valores de pontuação relativos são recalculados imediatamente. Os níveis de urgência e pontuação relativa são calculados automaticamente todas as noites nos servidores da Marketo.

>[!NOTE]
>
>A contagem de Urgência relativa (chamas) e Pontuação relativa (estrelas) são inteiros no Marketo. Os valores possíveis para cada são de 0 a 3.
