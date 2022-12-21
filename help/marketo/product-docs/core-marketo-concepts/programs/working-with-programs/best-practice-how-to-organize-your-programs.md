---
unique-page-id: 6848705
description: Prática recomendada - Como organizar seus programas - Documentos do Marketo - Documentação do produto
title: Prática recomendada - Como organizar seus programas
exl-id: 018a3fbd-b741-4005-9695-56958063d71a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 4%

---

# Prática recomendada: Como organizar seus programas {#best-practice-how-to-organize-your-programs}

Há muitas maneiras de organizar a árvore nas Atividades de marketing, bem como o conteúdo de um único programa. No entanto, algumas maneiras são melhores e ajudarão as pessoas em seu departamento de marketing.

>[!TIP]
>
>Um dia (quando é promovido!) outra pessoa tentará entender seus programas. Uma boa organização os ajudará a produzir rapidamente.

## Pastas {#folders}

Nas Atividades de marketing, você deve usar pastas para organizar seus programas. A estrutura que recomendamos está no seguinte exemplo:

>[!NOTE]
>
>**Exemplo**
>
>* Programas de marketing ativos
   >   * E-mails
   >   * Eventos
      >      * Eventos ao vivo / Roadshows
      >      * Shows de vendas
      >      * Webinars
   >   * Boletins informativos
   >   * Promoção
   >   * Conteúdo da Web
   >   * Formulários da Web
>* Aprendizagem
>* Operacional
   >   * Ciclo de vida
   >   * Pontuação
   >   * Gerenciamento de dados
>* Sales Insight
   >   * Momentos interessantes
   >   * E-mails de vendas
   >   * Campanhas solicitadas de vendas
>* **Arquivar**
   >   * Arquivar eventos
      >      * Arquivo 2012
      >      * Arquivo 2013


Cada um desses mencionados no exemplo é uma pasta. Observe como todos têm um nome exclusivo. Você pode ter nomes duplicados (mais simples) de pastas DENTRO de programas, mas não na raiz da árvore.

>[!TIP]
>
>A pasta &quot;Arquivo&quot; é um tipo especial de pasta criada para remover itens de listas selecionadas, bem como relatórios. Isso ajudará seu sistema a funcionar mais rápido. Saiba mais [mais informações sobre pastas](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md).

Você certamente poderá adicionar mais pastas, como desejar. Lembre-se de que as futuras gerações de profissionais de marketing em sua empresa estarão familiarizadas com suas decisões sobre como nomear/organizar as coisas.

## Nomear esquemas {#naming-schemes}

A nomenclatura é essencial, já que os recursos da Marketo usam uma linguagem comum para se comunicar. Para programas, você deve nomeá-los como exclusivos. **Nenhum programa pode ter o mesmo nome**. A prática recomendada é usar o seguinte formato:

[Abreviação do tipo de programa] [YYYY]-[MM]-[DD opcional] [Breve descrição]

>[!NOTE]
>
>**Exemplo**
>
>Exemplos de nomes de programas:
>
>1. ES 2015-09-21 - Introdução de widget
>1. Newsletter NL 2015-06
>1. WBN 2015-12-01 Tópico Do Webinar Aqui


Os nomes de programas precisam ser exclusivos em sua assinatura, mesmo em [espaços de trabalho](/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md).  Para os ativos locais dentro dos programas, a regra é **manter o nome simples**. Basta nomear um convite como &quot;Convite&quot;, em oposição ao &quot;Convite do Webinar de 2015.&quot; Como eles estão em um programa, o programa pai faz automaticamente parte do nome ao escolhê-lo em outro lugar. Em outras palavras, os ativos locais só precisam ser exclusivos dentro do programa. Você pode ter centenas de ativos chamados de &quot;Convidar&quot;, cada um em um programa diferente, e isso não irá atrapalhar você.

## Tokens {#tokens}

Tokens usam pastas e programas como um veículo para definir variáveis a serem usadas por landing pages, emails e outros ativos.

A organização mencionada acima permite colocar tokens na pasta Evento para que ela fique em cascata em todos os eventos.

>[!NOTE]
>
>**Exemplo**
>
>**Seu endereço corporativo**. Use um token em vez de gravá-lo todas as vezes. Dessa forma, você pode atualizá-lo em um ponto sem precisar criar muitos rascunhos. Em seguida, substitua o token conforme necessário em uma pasta de nível inferior.

## Eventos {#events}

Um evento geralmente tem muitas partes móveis, incluindo: convites, páginas de aterrissagem, formulários, widgets sociais e campanhas inteligentes. A prática recomendada para organizá-los para facilitar o uso é pela fase do Evento. Este é um exemplo de como a árvore de pastas deve procurar um Evento.

![](assets/capture.png)

## Programas de envolvimento {#engagement-programs}

Saiba mais [tudo sobre programas de envolvimento](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/understanding-engagement-programs.md). A melhor maneira de organizar seu programa de envolvimento é com pastas. Crie uma pasta para cada fluxo e coloque os emails ou programas nessa pasta. Inclua uma pasta de arquivamento em cada fluxo quando o conteúdo estiver obsoleto e desejar removê-lo.

## Programas Operacionais {#operational-programs}

Eles são usados para fins de limpeza de dados. Ter pastas para as datas em que os programas foram executados e, em seguida, arquivar as pastas. Ao tornar o programa operacional, você o está omitindo dos relatórios, o que é bom para esse tipo de atividade.

## Aninhamento de programas de email {#nesting-email-programs}

Programas de email foram projetados para serem sua ferramenta de emails estragados. Você pode colocá-los dentro de Eventos ou outros programas para promoções, convites e lembretes. Eles vêm com um painel legal e outros recursos de teste A/B. Além disso, elas são facilmente manipuladas na visualização de programação do programa.

Você também pode criar um programa de email como um programa independente. Programas de email não são permitidos em outros programas de email. Isso seria loucura!

## Clonando {#cloning}

Um dos recursos mais interessantes do Marketo é a capacidade de clonar programas. Isso significa que você pode configurar um &quot;template&quot; de programa que tenha todas as campanhas inteligentes e emails desejados. Configure-o antecipadamente e clone-o para sua próxima iniciativa de marketing.

>[!TIP]
>
>Observe os Modelos de evento no exemplo na parte superior. Coloque seus diferentes tipos de eventos lá para facilitar a clonagem.

Algumas pessoas até mesmo abstraem a maior parte do texto nos emails e landing pages em tokens. Isso permite clonar e editar os tokens. Por fim, acesse a visualização do cronograma do programa e ajuste as datas e termine. Voila!

## Resumo {#summary}

Como podem ver, há muito poder no Marketo. Nós cobrimos as noções básicas aqui, mas considere alguns [serviços adicionais de especialistas da Marketo](https://www.marketo.com/services/) para afinar e se preparar para o sucesso.
