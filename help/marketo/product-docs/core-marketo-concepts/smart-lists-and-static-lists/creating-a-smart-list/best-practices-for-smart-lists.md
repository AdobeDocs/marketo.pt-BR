---
unique-page-id: 7512524
description: Práticas recomendadas para Smart Lists - Documentação do Marketo - Documentação do produto
title: Práticas recomendadas para listas inteligentes
exl-id: 466de198-1012-4ac3-906c-d41943fe5bc0
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 1%

---

# Práticas recomendadas para listas inteligentes {#best-practices-for-smart-lists}

As Smart Lists são a ferramenta de consulta mais avançada no universo de marketing. Eles encontram as pessoas que você procura com rapidez e facilidade mágicas.

Para facilitar o trabalho e otimizar o desempenho, criamos uma lista de práticas recomendadas. Aproveite!

>[!NOTE]
>
>**Cada usuário do Marketo Engage é diferente.** Quanto maior o banco de dados, mais processamento acontece. Quanto mais atividades você armazenar, mais tempo levará para pesquisá-las.
>
>Se estiver com lentidão, experimente as dicas abaixo. Se o problema persistir, contate o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. **Limitar histórico -** Os filtros de histórico (também conhecidos como filtros de atividade) estão entre as operações que consomem mais recursos e mais tempo. Se precisar usá-los, tente limitar o intervalo de datas para o mais curto possível, o que reduziria o conjunto de dados pesquisável. Além disso, os intervalos de datas não substituirão os períodos de retenção. Exemplo: se a atividade que você está consultando tiver um período de retenção de 90 dias e você escolher &quot;últimos 100 dias&quot;, somente os resultados dos últimos 90 dias serão retornados. Os períodos de retenção de atividade [podem ser encontrados aqui](https://nation.marketo.com/t5/knowledgebase/marketo-activities-data-retention-policy/ta-p/251480){target="_blank"}.
1. **Limitar Smart Lists aninhadas -** Ao criar uma nova Smart List, limite a quantidade de filtros &quot;Membro da Smart List&quot; usados. Isso é chamado de aninhamento de Smart Lists, e cada Smart List referenciada aumentará o tempo de processamento. Em vez disso, faça referência a listas estáticas ou utilize a [segmentação](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md){target="_blank"}.
1. **Use operadores positivos sobre negativos -** Embora os filtros &quot;não&quot; estejam disponíveis, eles precisam pesquisar todo o conjunto de dados na sua instância, o que pode ser extremamente demorado. Os filtros positivos &quot;is&quot; são capazes de aproveitar algoritmos de pesquisa mais eficazes.
1. **Evite &quot;contém&quot; -** Se você tiver apenas dados parciais, os qualificadores &quot;começa com&quot; produzirão resultados muito mais rápidos que &quot;contém&quot;. &quot;Is&quot; será executado ainda mais rápido. Evite usar &quot;contains&quot; com vários valores; os dois juntos podem retardar ainda mais uma campanha.
1. **Usar Amostra Aleatória por si só -** A Amostra Aleatória é um filtro especial. Use-o sozinho para colocar seu pessoal em listas pré-fabricadas. Em seguida, use &quot;Membro da lista&quot; para tornar sua lista inteligente super rápida. A Amostra aleatória **NÃO** funcionará com Smart Lists aninhadas. O filtro de Amostra aleatória não funcionará se for a Smart List que está sendo referenciada para o filtro &quot;Membro da Smart List&quot;.
1. **Seja eficiente com filtros de inatividade -** Filtros como &quot;Formulário não preenchido&quot; podem ser muito úteis, mas exigem muito mais poder de processamento.
1. **Seja eficiente ao colar em vários valores -** A seleção múltipla foi projetada para colar em dezenas ou possivelmente centenas de valores. Coloque muitas, no entanto, e vai desacelerar muito.
1. **Seja econômico ao adicionar restrições -** Estes são os pequenos detalhes de uma regra e valores relacionados. Quanto mais restrições você adicionar, mais lento será o tempo de processamento.
1. **Simplifique suas campanhas -** mais de 100 regras independentes (nós vimos isso!) obviamente levarão algum tempo para serem processadas. Mantenha-o simples e você perceberá os ganhos de velocidade - além disso, será mais fácil para você entender.
1. **Inclua o símbolo @ antes do nome de domínio ao usar o filtro de Endereço de Email** **-**. Isso faz com que ele use uma consulta mais rápida. Exemplo: em vez de usar _email contém &#39;somedomain.com&#39;_, use _email contém &#39;@somedomain.com_.&#39; Se você estiver usando vários endereços de email com &quot;contém&quot;, TODOS eles deverão começar com &quot;@&quot;.

>[!TIP]
>
>O Marketo Engage pode ser usado de várias maneiras e determinadas técnicas são melhores para você e para sua empresa. Entre em contato com o representante de vendas da Adobe Professional Services se desejar obter ajuda para aproveitar ao máximo seu investimento.
