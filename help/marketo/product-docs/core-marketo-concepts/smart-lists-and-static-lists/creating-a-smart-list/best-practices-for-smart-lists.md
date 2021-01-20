---
unique-page-id: 7512524
description: Práticas recomendadas para Listas inteligentes - Documentos de marketing - Documentação do produto
title: Práticas recomendadas para Listas inteligentes
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---


# Práticas recomendadas para Listas inteligentes {#best-practices-for-smart-lists}

As listas inteligentes são a ferramenta de query mais poderosa do universo de marketing. Eles encontram as pessoas que você está procurando com velocidade mágica e facilidade.

Para facilitar o trabalho e otimizar o desempenho, criamos uma lista de boas práticas. Aproveite!

>[!NOTE]
>
>**Cada cliente é diferente.** Quanto maior o banco de dados, mais processamento acontece. Quanto mais atividades você armazena, mais tempo leva para pesquisar por elas.
>
>Se você estiver experimentando lentidão, tente as dicas abaixo. Se o problema persistir, entre em contato com o [Suporte de marketing](https://nation.marketo.com/t5/Support/ct-p/Support).

1. **Histórico limite - filtros** do histórico (também conhecido como Filtros de atividade) estão entre as operações mais demoradas, que consomem muitos recursos. Se você precisar usá-los, tente limitar o intervalo de datas ao mínimo possível, o que reduziria o conjunto de dados pesquisáveis.
1. **Limitar listas inteligentes aninhadas -** Ao criar uma nova lista inteligente, limite a quantidade de filtros &quot;Membro da Lista inteligente&quot; usados. Isso é chamado de aninhamento de listas inteligentes, e cada lista inteligente referenciada aumentará o tempo de processamento. Em vez disso, faça referência a listas estáticas ou utilize [segmentação](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).
1. **Use operadores positivos em vez de negativos -** Embora os filtros &quot;não&quot; estejam disponíveis, eles precisam pesquisar todo o conjunto de dados em sua instância, o que pode ser extremamente demorado. Filtros positivos &quot;is&quot; são capazes de aproveitar algoritmos de pesquisa mais eficazes.
1. **Evite &quot;contém&quot; -** se você tiver apenas dados parciais, os qualificadores &quot;start com&quot; produzirão resultados muito mais rápidos do que &quot;contém&quot;. &quot;Is&quot; funcionará ainda mais rápido. Evite usar &quot;contém&quot; com vários valores; os dois juntos podem retardar uma campanha ainda mais.
1. **Use Amostra aleatória sozinha - Amostra** aleatória é um filtro especial. Use-o sozinho para colocar seu povo em listas pré-fabricadas. Depois, use &quot;Membro da Lista&quot; para tornar sua lista inteligente super rápida. A Amostra aleatória **NOT** funcionará com Listas inteligentes aninhadas. O filtro Amostra aleatória não funcionará se for a Lista inteligente que está sendo referenciada para o filtro &quot;Membro da Lista inteligente&quot;.
1. **Seja próspero com filtros de inatividade -** Filtros como &quot;Formulário não preenchido&quot; podem ser realmente úteis, mas exigem muito mais poder de processamento.
1. **Seja próspero ao colar em vários valores - a** seleção múltipla foi projetada para colar em dezenas ou possivelmente centenas de valores. No entanto, coloque demasiadas coisas e vai abrandar.
1. **Seja próspero ao adicionar restrições -** Esses são os detalhes minúsculos de uma regra e valores relacionados. Quanto mais restrições você adicionar, mais lento será o tempo de processamento.
1. **Simplifique suas regras independentes campanha -** 100+ (já vimos!) obviamente vamos levar algum tempo para processar. Mantenha-o simples e você notará os ganhos de velocidade - além disso, será mais fácil para você entender.
1. **Inclua o símbolo @ antes do nome do domínio ao usar o filtro** **Endereço de email -** Isso faz com que ele use um query mais rápido. Exemplo: Em vez de usar _email contém &#39;somedomain.com&#39;_, use _email contém &#39;@somedomain.com_.&#39; Se você estiver usando vários endereços de email com &quot;contém&quot;, TODOS devem start com &quot;@&quot;.

>[!TIP]
>
>O Marketo pode ser usado de várias maneiras e certas técnicas são melhores para você e para sua empresa. Considere [Serviços profissionais de marketing](https://pages2.marketo.com/72-hour-survival-guide.html) para tornar seu investimento brilhante.
