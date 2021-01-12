---
unique-page-id: 10096583
description: Perguntas frequentes sobre o rastreamento Munchkin da próxima geração - Documentos do Marketing - Documentação do produto
title: Perguntas frequentes sobre o rastreamento Munchkin da próxima geração
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---


# Perguntas frequentes sobre o rastreamento Munchkin da próxima geração {#next-generation-munchkin-tracking-faq}

Estamos empolgados em anunciar que em breve começaremos um lançamento em etapas da nossa tecnologia de rastreamento da Web de próxima geração.

Estas são as coisas mais importantes a saber:

* Estamos removendo o filtro &quot;É Anônimo&quot; de Lista inteligente com nossa versão do primeiro trimestre (já concluída)
* Estamos aumentando o número de eventos da Web (Visite a página da Web, Link clicado na página da Web) que podemos assimilar
* Seu código Munchkin não será alterado, portanto, nenhuma atualização é necessária em seu site

## Quando a minha subscrição de Marketo estará na Munchkin V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Ainda não temos uma data exata, mas verifique aqui para obter atualizações.

## Precisarei fazer alguma alteração no meu rastreamento de Munchkin no meu site? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

Não. O código de rastreamento Munchkin continua o mesmo. Não é necessário fazer alterações no seu site.

>[!NOTE]
>
>Essa alteração não afeta a Personalização da Web (Personalização em tempo real). Ele continua a identificar visitantes da Web anônimos e conhecidos e a personalizar o conteúdo em tempo real para esses visitantes.

## Por que o Marketo removeu o filtro &quot;Is Anonymous&quot; das Listas inteligentes? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Nós mudamos como pessoas anônimas interagem com Campanhas inteligentes. Antes, eles fluíam através de uma campanha inteligente, como pessoas conhecidas. O filtro &quot;É anônimo&quot; foi usado para especificar que somente pessoas conhecidas ou anônimas fluem pela campanha.

Com o Munchkin V2, continuaremos a acompanhar todas as atividades anônimas; no entanto, não é mais possível aplicar filtros a pessoas anônimas. No ponto de conversão (quando a pessoa se torna conhecida em Marketo), todas as atividades que ocorreram quando a pessoa era anônima são anexadas ao registro de atividades da pessoa e, nesse momento, fluem pelas campanhas para as quais se qualificam.

Se você já estiver usando esse filtro em uma Lista inteligente (por exemplo, em uma Campanha inteligente ou em um Relatório), ele não será removido automaticamente da Lista inteligente. Consulte abaixo para obter mais detalhes.

>[!NOTE]
>
>**Acionador**: Visitas à Página da Web, Página da Web é Página de Preços\
>**Fluxo**: Alterar pontuação +10 e momento interessante
>**Web**: Página de Preços Exibida
>
>Com Munchkin V2, se uma pessoa anônima visitar a página de preços, ela não entra na campanha imediatamente. Quando a pessoa anônima se tornar conhecida, nós vamos colocar essa campanha nela. Ela irá:
>
>* Obter uma pontuação de 10
   >
   >
* Ter a atividade da Página da Web definida como a data certa (quando ela realmente visitou)
   >
   >
* Ter um momento interessante registrado para ela (com a data em que ela realmente visitou a página, não quando ela ficou conhecida)
   >
   >
* Ter uma atividade &quot;Nova Pessoa&quot; registrada, como está hoje


## O que acontece com minhas Listas inteligentes que já têm o filtro &quot;É Anônimo&quot;? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Depois da nossa versão de inverno de 16, se você tiver Campanhas inteligentes antigas com uma Lista inteligente que tem o filtro &quot;É anônimo&quot;, uma das duas coisas acontecerão:

1. Se a Lista inteligente tiver o filtro &quot;Is Anonymous = False&quot;, nada acontecerá. Vamos simplesmente ignorá-lo.
1. Se a Lista inteligente tiver o filtro &quot;Is Anonymous = True&quot;, então essa campanha falhará e você receberá uma notificação.

## Estou usando Marketo há algum tempo. Como faço para saber qual de minhas campanhas usa o filtro &quot;É anônimo&quot;? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Antes de fazermos essa alteração, enviamos várias notificações semanais para sua caixa de entrada Notificações com uma lista de Listas inteligentes, Campanhas inteligentes e relatórios que usam o filtro &quot;É anônimo&quot;. Isso pode ajudá-lo a identificar onde você está usando esse filtro no momento.

Revise-os e identifique onde &quot;É Anônimo&quot; está definido como Verdadeiro, já que essas são as campanhas afetadas. Na maioria das vezes, os clientes usam essa configuração para algum tipo de pontuação. Consulte o exemplo acima para entender como essas campanhas funcionarão agora.

## Eu gostaria de documentação mais detalhada. Onde posso encontrá-lo? {#id-like-more-detailed-documentation-where-can-i-find-it}

Confira estes links:

[Visão geral de atualizações de clientes potenciais anônimos](https://nation.marketo.com/docs/DOC-2937)

[Atualizações de clientes potenciais anônimos - Alterações na interface do usuário do marketing](https://nation.marketo.com/docs/DOC-2938)

[Atualizações de clientes potenciais anônimos - Ação necessária do cliente](https://nation.marketo.com/docs/DOC-2939)

[Atualizações de clientes potenciais anônimos - Relatórios do Analytics](https://nation.marketo.com/docs/DOC-2940)

[Upgrades de clientes potenciais anônimos - Programação de lançamento](https://nation.marketo.com/docs/DOC-2961)

[Upgrades De Chumbo Anônimos - Abaixo Da Capa](https://nation.marketo.com/docs/DOC-2962)

[Promoção Anônima de Chumbo para Chumbo Conhecido - Comportamento Munchkin V2](https://nation.marketo.com/docs/DOC-2963)

## Tenho mais perguntas! Como obtenho respostas? {#i-have-more-questions-how-do-i-get-them-answered}

Entre em contato com a [comunidade](https://nation.marketo.com/welcome). Você também pode entrar em contato com o [Suporte ao Marketing](https://nation.marketo.com/t5/Support/ct-p/Support). Eles ficarão felizes em responder suas perguntas.
