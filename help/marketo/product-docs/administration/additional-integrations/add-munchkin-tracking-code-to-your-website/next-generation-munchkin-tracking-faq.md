---
unique-page-id: 10096583
description: Perguntas frequentes sobre a implantação do rastreamento de  [!DNL Munchkin]  de próxima geração e a alteração do filtro É anônimo.
title: 'Perguntas frequentes sobre o Acompanhamento da Próxima Geração [!DNL Munchkin] '
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
hide: true
source-git-commit: 689773f0d6f87b65d5299ecc11f3de11f7e66775
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Perguntas frequentes sobre o rastreamento de [!DNL Munchkin] da próxima geração {#next-generation-munchkin-tracking-faq}

A Marketo está lançando a tecnologia de rastreamento Web da próxima geração em fases.

Estas são as informações mais importantes:

* O filtro &quot;Is Anonymous&quot; da Smart List foi removido
* O número de eventos da Web (Visitar página da Web, Link clicado na página da Web) que o Marketo pode assimilar está aumentando
* O código [!DNL Munchkin] não será alterado, portanto, não são necessárias atualizações no site

## Quando minha assinatura do Marketo estará em [!DNL Munchkin] V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Uma data exata ainda não está disponível. Verifique se há atualizações nesta página.

## Será necessário fazer alguma alteração no rastreamento de [!DNL Munchkin] em meu site? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

Não. O código de rastreamento [!DNL Munchkin] permanece o mesmo. Não é necessário fazer alterações no site.

>[!NOTE]
>
>Essa alteração não afeta o Web Personalization (Real-Time Personalization). Ele continua a identificar visitantes anônimos e conhecidos da Web e personalizar o conteúdo em tempo real para esses visitantes.

## Por que o Marketo removeu o filtro &quot;É anônimo&quot; das Smart Lists? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

O Marketo mudou a forma como as pessoas anônimas interagem com Campanhas inteligentes. Antes, eles fluíam através de uma campanha inteligente, assim como pessoas conhecidas. O filtro &quot;Is Anonymous&quot; foi usado para especificar que apenas pessoas conhecidas ou anônimas fluem pela campanha.

Com o [!DNL Munchkin] V2, a Marketo continuará a rastrear todas as atividades anônimas; no entanto, você não poderá mais aplicar filtros a pessoas anônimas. No ponto de conversão (quando a pessoa se torna conhecida no Marketo), todas as atividades que ocorreram quando a pessoa era anônima são anexadas ao log de atividades da pessoa e, neste momento, elas fluem pelas campanhas para as quais se qualificam.

Se você já estiver usando esse filtro em uma Smart List (por exemplo, em uma Campanha inteligente ou um Relatório), ele não será removido automaticamente da Smart List. Veja mais detalhes abaixo.

>[!NOTE]
>
>**Acionador**: Página Visitas da Web, Página da Web com Preços >**Fluxo**: alterar pontuação +10 e momento interessante >**Web**: Página de Preços Visualizada
>
>Com a versão [!DNL Munchkin] V2, se uma pessoa anônima visitar a página de preços, ela não entrará na campanha imediatamente. No momento em que a pessoa anônima se torna conhecida, o Marketo realiza essa campanha nela. Eles irão:
>
>* Obtenha uma pontuação de 10
>
>* Ter a atividade de página da Web definida para a data correta (quando eles realmente visitaram)
>
>* Registre um momento interessante para eles (com a data em que realmente visitaram a página, não quando se tornaram conhecidos)
>
>* Ter uma atividade &quot;Nova pessoa&quot; registrada, como está hoje

## O que acontece com minhas Smart Lists que já têm o filtro &quot;É anônimo&quot;? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Depois da versão de inverno de 16, se você tiver campanhas inteligentes antigas com uma lista inteligente que contenha o filtro &quot;É anônimo&quot;, uma das duas coisas acontecerá:

1. Se a Smart List tiver o filtro &quot;Is Anonymous = False&quot;, nada acontecerá. Ele é ignorado.
1. Se a Smart List tiver o filtro &quot;Is Anonymous = True&quot;, essa campanha falhará e uma notificação será enviada.

## Eu uso o Marketo há algum tempo. Como sei qual das minhas campanhas usa o filtro &quot;É anônimo&quot;? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Antes dessa alteração, o Marketo enviava várias notificações semanais para sua caixa de entrada de Notificações com uma lista de Smart Lists, Campanhas inteligentes e Relatórios que usam o filtro &quot;É anônimo&quot;. Isso pode ajudá-lo a identificar onde você está usando esse filtro no momento.

Revise-as e identifique onde &quot;É anônimo&quot; está definido como Verdadeiro, pois essas são as campanhas afetadas. Na maioria das vezes, essa configuração é usada para algum tipo de pontuação. Consulte o exemplo acima para entender como essas campanhas funcionarão agora.

## Eu gostaria de obter uma documentação mais detalhada. Onde posso encontrá-lo? {#id-like-more-detailed-documentation-where-can-i-find-it}

Confira estes links:

[Visão geral de atualizações de clientes potenciais anônimos](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[Atualizações de clientes potenciais anônimos - Alterações na interface do usuário do Marketo](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[Atualizações de clientes potenciais anônimos - Ação do cliente necessária](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[Atualizações de clientes potenciais anônimos - Relatórios do Analytics](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[Atualizações de clientes potenciais anônimos - Programação de lançamento](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[Atualizações de leads anônimos - Por baixo dos panos](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[Promoção de lead anônimo para lead conhecido -  [!DNL Munchkin] V2 Comportamento](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## Eu tenho mais perguntas! Como posso respondê-los? {#i-have-more-questions-how-do-i-get-them-answered}

Visite a [Comunidade do Marketo](https://experienceleaguecommunities.adobe.com/?profile.language=pt){target="_blank"}. Você também pode entrar em contato com o Suporte da Marketo. Eles ficam felizes em responder às suas perguntas.
