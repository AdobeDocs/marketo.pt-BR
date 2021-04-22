---
unique-page-id: 7512524
description: Práticas recomendadas para Smart Lists - Documentos do Marketo - Documentação do produto
title: Práticas recomendadas para Smart Lists
exl-id: 466de198-1012-4ac3-906c-d41943fe5bc0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# Práticas recomendadas para Smart Lists {#best-practices-for-smart-lists}

As listas inteligentes são a ferramenta de query mais eficiente no universo de marketing. Eles encontram as pessoas que você está procurando com velocidade mágica e facilidade.

Para facilitar o trabalho e otimizar o desempenho, criamos uma lista de boas práticas. Aproveite!

>[!NOTE]
>
>**Cada cliente é diferente.** Quanto maior o banco de dados, mais processamento acontece. Quanto mais atividades você tiver armazenado, mais tempo levará para pesquisá-las.
>
>Se estiver passando por uma lentidão, tente as dicas abaixo. Se o problema persistir, entre em contato com o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. **Histórico de limite -** Os filtros de histórico (também conhecidos como filtros de atividade) estão entre as operações mais demoradas e com uso intenso de recursos. Se precisar usá-los, tente limitar o intervalo de datas para o mais curto possível, o que reduziria o conjunto de dados pesquisável.
1. **Limitar listas inteligentes aninhadas -** Ao criar uma nova lista inteligente, limite a quantidade de filtros &quot;Membro da Smart List&quot; usados. Isso é chamado de aninhamento de listas inteligentes, e cada lista inteligente referenciada aumentará o tempo de processamento. Em vez disso, faça referência a listas estáticas ou utilize [segmentation](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).
1. **Use operadores positivos em vez de negativos -** Embora os filtros &quot;não&quot; estejam disponíveis, eles precisam pesquisar todo o conjunto de dados na sua instância, o que pode ser extremamente demorado. Filtros positivos &quot;is&quot; podem aproveitar algoritmos de pesquisa mais eficazes.
1. **Evite &quot;contém&quot; -** se você tiver apenas dados parciais, os qualificadores &quot;inicia com&quot; produzirão resultados muito mais rápidos do que &quot;contém&quot;. &quot;Is&quot; será executado ainda mais rápido. Evite usar &quot;contains&quot; com vários valores; os dois juntos podem atrasar uma campanha ainda mais.
1. **Usar a Amostra aleatória sozinha -** Amostra aleatória é um filtro especial. Use-o por si só para colocar seu povo em listas pré-fabricadas. Em seguida, use &quot;Membro da lista&quot; para tornar sua lista inteligente super rápida. A Amostra Aleatória **NOT** funcionará com Smart Lists aninhadas. O filtro Amostra aleatória não funcionará se for a Smart List que está sendo referenciada para o filtro &quot;Membro da Smart List&quot;.
1. **Seja confiável com filtros de inatividade -** Filtros como &quot;Formulário não preenchido&quot; podem ser realmente úteis, mas exigem muito mais poder de processamento.
1. **Tenha orgulho de colar em vários valores - a seleção múltipla**  foi projetada para colar em dezenas ou possivelmente centenas de valores. No entanto, coloque demasiadas coisas e irá abrandar.
1. **Tenha orgulho ao adicionar restrições -** Esses são os detalhes minúsculos de uma regra e valores relacionados. Quanto mais restrições você adicionar, mais lento será o tempo de processamento.
1. **Simplifique suas campanhas - mais de** 100 regras independentes (já vimos!) obviamente que levarão algum tempo para processar. Mantenha-o simples e você notará os ganhos de velocidade - além disso, será mais fácil para você entender.
1. **Inclua o símbolo @ antes do nome de domínio ao usar o filtro Endereço de email** **-** Isso faz com que ele use uma consulta mais rápida. Exemplo: Em vez de usar _email contém &#39;somedomain.com&#39;_, use _email contém &#39;@somedomain.com_&#39;. Se estiver usando vários endereços de email com &quot;contém&quot;, TODOS eles devem começar com &quot;@.&quot;

>[!TIP]
>
>O Marketo pode ser usado de muitas formas e determinadas técnicas são melhores para você e para sua empresa. Considere [os serviços profissionais da Marketo](https://pages2.marketo.com/72-hour-survival-guide.html) para fazer seu investimento brilhar.
