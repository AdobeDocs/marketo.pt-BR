---
unique-page-id: 10096583
description: Perguntas frequentes sobre rastreamento da próxima geração [!DNL Munchkin] Marketo Docs - Documentação do produto
title: 'Perguntas frequentes sobre o Acompanhamento da Próxima Geração [!DNL Munchkin] '
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
hide: true
hidefromtoc: true
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

# Perguntas frequentes sobre o rastreamento de [!DNL Munchkin] da próxima geração {#next-generation-munchkin-tracking-faq}

Estamos animados em anunciar que em breve iniciaremos uma implantação em fases da nossa tecnologia de rastreamento na web de última geração.

Estas são as informações mais importantes:

* Estamos removendo o filtro &quot;Is Anonymous&quot; da Smart List com nossa versão do primeiro trimestre (já concluído)
* Estamos aumentando o número de eventos da Web (Visitar página da Web, Link clicado na página da Web) que podem ser assimilados
* O código [!DNL Munchkin] não será alterado, portanto, não são necessárias atualizações no site

## Quando minha assinatura do Marketo estará em [!DNL Munchkin] V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Ainda não temos uma data exata, mas verifique se há atualizações aqui.

## Será necessário fazer alguma alteração no rastreamento de [!DNL Munchkin] em meu site? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

Não. O código de rastreamento [!DNL Munchkin] permanece o mesmo. Não é necessário fazer alterações no site.

>[!NOTE]
>
>Essa alteração não afeta o Web Personalization (Real-Time Personalization). Ele continua a identificar visitantes anônimos e conhecidos da Web e personalizar o conteúdo em tempo real para esses visitantes.

## Por que o Marketo removeu o filtro &quot;É anônimo&quot; das Smart Lists? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Alteramos a forma como as pessoas anônimas interagem com Campanhas inteligentes. Antes, eles fluíam através de uma campanha inteligente, assim como pessoas conhecidas. O filtro &quot;Is Anonymous&quot; foi usado para especificar que apenas pessoas conhecidas ou anônimas fluem pela campanha.

Com a versão [!DNL Munchkin] V2, continuaremos a rastrear todas as atividades anônimas; no entanto, você não poderá mais aplicar filtros a pessoas anônimas. No ponto de conversão (quando a pessoa se torna conhecida no Marketo), todas as atividades que ocorreram quando a pessoa era anônima são anexadas ao log de atividades da pessoa e, neste momento, elas fluem pelas campanhas para as quais se qualificam.

Se você já estiver usando esse filtro em uma Smart List (por exemplo, em uma Campanha inteligente ou um Relatório), ele não será removido automaticamente da Smart List. Veja mais detalhes abaixo.

>[!NOTE]
>
>**Acionador**: Página Visitas da Web, Página da Web com Preços
>>**Fluxo**: alterar pontuação +10 e momento interessante
>>**Web**: Página de Preços Visualizada
>
>Com a versão [!DNL Munchkin] V2, se uma pessoa anônima visitar a página de preços, ela não entrará na campanha imediatamente. Quando o anônimo se tornar conhecido, faremos essa campanha com ela. Ela vai:
>
>* Obtenha uma pontuação de 10
>
>* Ter a atividade de página da Web definida para a data correta (quando ela realmente visitou)
>
>* Registre um momento interessante para ela (com a data em que ela visitou a página, não quando se tornou conhecida)
>
>* Ter uma atividade &quot;Nova pessoa&quot; registrada, como está hoje

## O que acontece com minhas Smart Lists que já têm o filtro &quot;É anônimo&quot;? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Depois da nossa versão de inverno de 16, se você tiver campanhas inteligentes antigas com uma lista inteligente que contenha o filtro &quot;É anônimo&quot;, uma das duas coisas acontecerá:

1. Se a Smart List tiver o filtro &quot;Is Anonymous = False&quot;, nada acontecerá. Vamos simplesmente ignorá-lo.
1. Se a Smart List tiver o filtro &quot;Is Anonymous = True&quot;, essa campanha falhará e você receberá uma notificação.

## Eu uso o Marketo há algum tempo. Como sei qual das minhas campanhas usa o filtro &quot;É anônimo&quot;? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Antes de fazermos essa alteração, enviamos várias notificações semanais para sua caixa de entrada Notificações com uma lista de Smart Lists, Campanhas inteligentes e Relatórios que usam o filtro &quot;É anônimo&quot;. Isso pode ajudá-lo a identificar onde você está usando esse filtro no momento.

Revise-as e identifique onde &quot;É anônimo&quot; está definido como Verdadeiro, pois essas são as campanhas afetadas. Na maioria das vezes, os clientes usam essa configuração para algum tipo de pontuação. Consulte o exemplo acima para entender como essas campanhas funcionarão agora.

## Eu gostaria de documentação mais detalhada. Onde posso encontrá-lo? {#id-like-more-detailed-documentation-where-can-i-find-it}

Confira estes links:

[Visão Geral De Atualizações De Cliente Potencial Anônimo](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[Atualizações Anônimas de Cliente Potencial - Alterações na Interface do Usuário do Marketo](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[Atualizações Anônimas De Clientes Potenciais - Ação Do Cliente Necessária](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[Atualizações Anônimas de Clientes Potenciais - Relatórios do Analytics](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[Atualizações de Cliente Potencial Anônimas - Agendamento de Lançamento](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[Atualizações Anônimas De Clientes Potenciais - Por Baixo Da Tela](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[Promoção Anônima de Cliente Potencial para Cliente Potencial Conhecido - [!DNL Munchkin] Comportamento V2](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## Eu tenho mais perguntas! Como posso respondê-los? {#i-have-more-questions-how-do-i-get-them-answered}

Contate a [comunidade](https://nation.marketo.com/){target="_blank"}. Você também pode contatar o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}. Eles ficarão felizes em responder suas perguntas.
