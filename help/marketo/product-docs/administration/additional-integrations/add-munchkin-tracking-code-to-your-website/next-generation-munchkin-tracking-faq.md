---
unique-page-id: 10096583
description: Perguntas frequentes sobre o rastreamento do Munchkin de próxima geração - Documentos do Marketo - Documentação do produto
title: Perguntas frequentes sobre o rastreamento do Munchkin de próxima geração
exl-id: 283189ac-c817-479a-b896-91233980608c
source-git-commit: 6ad418c8f4056b9a2fb31b0ac995692f0c618795
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# Perguntas frequentes sobre o rastreamento do Munchkin de próxima geração {#next-generation-munchkin-tracking-faq}

Estamos animados em anunciar que em breve começaremos um lançamento em fases de nossa tecnologia de rastreamento Web de próxima geração.

Estas são as coisas mais importantes a saber:

* Estamos removendo o filtro Smart List &quot;Is Anonymous&quot; com nossa versão do primeiro trimestre (já concluída)
* Estamos aumentando o número de eventos da Web (Visite a página da Web, Link clicado na página da Web) que podemos assimilar
* Seu código do Munchkin não será alterado, portanto, nenhuma atualização em seu site é necessária

## Quando minha assinatura do Marketo será no Munchkin V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Ainda não temos uma data exata, mas confira aqui para obter atualizações.

## Precisarei fazer alguma alteração no rastreamento do Munchkin no meu site? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

Nº O código de rastreamento do Munchkin permanece o mesmo. Não é necessário fazer alterações no seu site.

>[!NOTE]
>
>Essa alteração não afeta o Web Personalization (Real-Time Personalization). Ela continua identificando visitantes da Web anônimos e conhecidos e personalizando o conteúdo em tempo real para esses visitantes.

## Por que o Marketo removeu o filtro &quot;É anônimo&quot; das Smart Lists? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Alteramos a forma como pessoas anônimas interagem com Campanhas Inteligentes. Antes, eles fluíam através de uma campanha inteligente, como pessoas conhecidas. O filtro &quot;Is Anonymous&quot; foi usado para especificar que apenas pessoas conhecidas ou anônimas fluem pela campanha.

Com o Munchkin V2, continuaremos a acompanhar todas as atividades anônimas; no entanto, não é mais possível aplicar filtros a pessoas anônimas. No ponto de conversão (quando a pessoa se torna conhecida no Marketo), todas as atividades que ocorreram quando a pessoa era anônima são anexadas ao registro de atividades da pessoa e, nesse momento, fluem pelas campanhas para as quais se qualificaram.

Se você já estiver usando esse filtro em uma Smart List (por exemplo, em uma Campanha inteligente ou um Relatório), ele não será removido automaticamente da Smart List. Consulte abaixo para obter mais detalhes.

>[!NOTE]
>
>**Acionador**: Visitas Página da Web, Página da Web é Página de Preços\
>**Fluxo**: Alterar pontuação +10 e momento interessante
>**Web**: Página Preços Visualizados
>
>Com o Munchkin V2, se uma pessoa anônima visitar a página de preços, ela não entrará na campanha imediatamente. Quando a pessoa anônima se tornar conhecida, nós realizaremos esta campanha nela. Ela irá:
>
>* Obter uma pontuação de 10
>
>* Ter a atividade Página da Web definida como a data certa (quando ela realmente visitou)
>
>* Tenha um momento interessante registrado para ela (com a data em que ela realmente visitou a página, não quando ela ficou conhecida)
>
>* Tenha uma atividade &quot;Nova pessoa&quot; registrada, como está hoje


## O que acontece com minhas Smart Lists que já têm o filtro &quot;Is Anonymous&quot;? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Depois da nossa versão de inverno de 16, se você tem campanhas inteligentes antigas com uma Smart List que tem o filtro &quot;Is Anonymous&quot; nela, uma das duas coisas acontecerão:

1. Se a Smart List tiver o filtro &quot;Is Anonymous = False&quot;, nada acontecerá. Nós vamos simplesmente ignorá-lo.
1. Se a Smart List tiver o filtro &quot;Is Anonymous = True&quot;, essa campanha falhará e você receberá uma notificação.

## Eu uso o Marketo há algum tempo. Como sei qual das minhas campanhas usa o filtro &quot;É anônimo&quot;? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Antes de fazer essa alteração, enviamos várias notificações semanais para sua caixa de entrada de Notificações com uma lista de Smart Lists, Campanhas inteligentes e Relatórios que usam o filtro &quot;É anônimo&quot;. Isso pode ajudar a identificar onde você está usando esse filtro no momento.

Revise-as e identifique onde você tem &quot;Anônimo&quot; definido como Verdadeiro, pois essas são as campanhas afetadas. Na maioria das vezes, os clientes usam essa configuração para algum tipo de pontuação. Consulte o exemplo acima para entender como essas campanhas funcionarão agora.

## Gostaria de documentação mais detalhada. Onde posso encontrá-lo? {#id-like-more-detailed-documentation-where-can-i-find-it}

Confira estes links:

[Visão geral de atualizações de clientes potenciais anônimos](https://nation.marketo.com/docs/DOC-2937)

[Atualizações de clientes potenciais anônimos - Alterações na interface do usuário do Marketo](https://nation.marketo.com/docs/DOC-2938)

[Upgrades de clientes potenciais anônimos - Ação necessária do cliente](https://nation.marketo.com/docs/DOC-2939)

[Upgrades de clientes potenciais anônimos - Relatórios do Analytics](https://nation.marketo.com/docs/DOC-2940)

[Atualizações de lead anônimas - Programação de lançamento](https://nation.marketo.com/docs/DOC-2961)

[Upgrades De Lead Anônimos - Sob O Cabeça](https://nation.marketo.com/docs/DOC-2962)

[Promoção principal anônima ao cliente potencial conhecido - Comportamento do Munchkin V2](https://nation.marketo.com/docs/DOC-2963)

## Tenho mais perguntas! Como obtenho respostas? {#i-have-more-questions-how-do-i-get-them-answered}

Entre em contato com o [comunidade](https://nation.marketo.com/). Também é possível entrar em contato [Suporte Marketo](https://nation.marketo.com/t5/Support/ct-p/Support). Eles ficarão felizes em responder suas perguntas.
