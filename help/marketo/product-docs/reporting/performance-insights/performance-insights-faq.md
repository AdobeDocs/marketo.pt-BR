---
unique-page-id: 12979858
description: Perguntas frequentes sobre Performance Insights - Documentos do Marketing - Documentação do produto
title: Perguntas frequentes sobre Performance Insights
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '1404'
ht-degree: 0%

---


# Perguntas frequentes sobre o Performance Insights {#performance-insights-faq}

## Qual é a definição de &quot;sucesso&quot; na guia Envolvimento? {#what-is-the-definition-of-success-in-the-engagement-tab}

O sucesso é uma medida de interação significativa em Marketo. O objetivo de um programa é criar uma interação significativa com a pessoa ou o prospecto. O sucesso é marcado quando uma pessoa atinge o status que atinge esse objetivo. Ele pode estar participando de um webinar, clicando em um link em um email ou preenchendo um formulário da Web. O sucesso varia dependendo do canal do programa.

>[!NOTE]
>
>**Exemplo**
>
>Em um programa de webinar, pode haver vários status, como: Convidado, Registrado e Participado. Convidados ou registrados não são interações significativas porque as pessoas não assistem ao webinar. A participação é considerada um sucesso neste caso.

## A MPI funcionará com algum CRM? {#will-mpi-work-with-any-crm}

Sim. Tecnicamente, o MPI não interage diretamente com o CRM para sincronização de dados. A MPI utiliza dados armazenados na Data Warehouse do Marketing Analytics. Como a sincronização do CRM ocorre no aplicativo de Gerenciamento de clientes potenciais, qualquer CRM compatível com o Marketing Cloud integrado ao aplicativo de Gerenciamento de clientes potenciais mostrará os dados corretamente. No entanto, os campos de oportunidade do CRM precisam ser mapeados corretamente para os campos de oportunidade do Marketing.

## Não tenho outros produtos do Marketing Analytics (ARB, RCE, RCA, Análise de Programas). O MPI vai funcionar para mim? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

O MPI é um complemento independente do aplicativo de gerenciamento de clientes potenciais. Não requer o uso de outros produtos de análise.

## A RCA também me mostra os dados de desempenho do programa. Existe uma diferença entre os dados mostrados em MPI e RCA? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

Não. Os dados de fontes MPI do mesmo data warehouse que o RCA. Portanto, você não verá nenhuma diferença de dados entre os dois. O RCA permite que você crie seus próprios relatórios dinamicamente. O MPI fornece acesso a painéis visuais fáceis de entender.

## Não quero que alguns dos meus programas (por exemplo, operacionais) apareçam no MPI. Como faço para controlar a visibilidade de programas específicos? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

É possível controlar a visibilidade dos programas definindo o comportamento do Analytics dos programas como Operacional. Isso fará com que o programa seja excluído dos cálculos do Analytics.

>[!NOTE]
>
>Saiba mais sobre como configurar o comportamento de análise [aqui](http://docs.marketo.com/display/public/DOCS/Edit+Analytics+Behavior+Settings).

## Estou executando uma campanha de vários canais para um novo lançamento de produto. Como posso visualização o desempenho desta campanha em todos os diferentes canais em um único lugar? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Recomendamos que, para programas de tal campanha, você utilize tags de programa. As tags de programa são sincronizadas automaticamente com MPI e você pode filtrá-las em todos os painéis MPI para visualização do desempenho da campanha de vários canais.

## Eu terei acesso às configurações de atribuição se não tiver RCA? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Você terá acesso às configurações de atribuição se tiver MPI, independentemente de ter RCA ou não.

## Recebo um alerta no MPI quando faço logon informando que minhas configurações de atribuição estão incorretas. O que há de errado? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

A MPI calcula se todas as suas oportunidades estão sendo incluídas na análise. Caso contrário, você será solicitado a considerar a alteração das configurações de atribuição (Explícita, implícita, híbrida) para incluir mais oportunidades.

Você também pode estar perdendo oportunidades devido ao custo do Programa ausente em seus programas. Analise o comportamento dos programas do Analytics. Eles podem ser:

1. Padrão - O comportamento padrão é o programa que seria incluído APENAS no MPI se houvesse pelo menos um custo do período, mesmo um com zero dólares atribuídos.
1. Inclusivo - Essa opção garantirá que o programa esteja disponível em MPI, independentemente de você ter incluído ou não um custo do período.
1. [Operacional](http://docs.marketo.com/display/DOCS/Best+Practice%3A+How+to+Organize+your+Programs#BestPractice:HowtoOrganizeyourPrograms-OperationalPrograms)  - Essa opção resulta na não exibição do programa no MPI.

>[!NOTE]
>
>O Custo do Período **tem** para ser configurado para relatórios Bem-sucedido e Novos Nomes no painel Envolvimento. Este painel utiliza dados de Custo do Período para obter agregações bem-sucedidas e novos nomes. Se o Custo do período não estiver configurado, o painel de envolvimento não informará corretamente independentemente das configurações de comportamento do Analytics acima.

## Por que estou perdendo algumas oportunidades no MPI? {#why-am-i-missing-some-opportunities-in-mpi}

Duas razões principais pelas quais você pode estar perdendo oportunidades no MPI são:

1. A configuração de atribuição está definida como Explícita, mas as oportunidades não têm Funções de contato atribuídas
1. O custo do período não está incluído em seus programas

A MPI calcula se todas as suas oportunidades estão sendo incluídas na análise. Caso contrário, você será solicitado a considerar a alteração das configurações de atribuição (Explícita, implícita, híbrida) para incluir mais oportunidades.

Você também pode estar perdendo oportunidades devido ao custo do Programa ausente em seus programas. O alerta aparecerá, mas não indica a você quais programas não têm custos. Revise a configuração do programa para incluir custos, a fim de garantir que todos os programas e oportunidades sejam incluídos na MPI.

## Por que não vejo campos personalizados, tipo de oportunidade e filtros ABM no painel de envolvimento? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

Campos personalizados, Tipo de oportunidade e Filtros ABM são todos atributos relacionados a uma oportunidade. O painel Envolvimento permite medir seu envolvimento e aquisição de lead, independentemente de estarem ou não associados a uma oportunidade. Como o painel de Envolvimento não leva em consideração a oportunidade, os campos personalizados, o tipo de oportunidade e os Filtros ABM não se aplicam.

## Desejo usar um campo Oportunidade do Salesforce personalizado para relatórios de receita em vez do campo Quantia de Oportunidade do Salesforce. O MPI me permitirá fazer isso? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Sim. [O ](http://docs.marketo.com/cdn-cgi/l/email-protection#b5c6c0c5c5dac7c1f5d8d4c7ded0c1da9bd6dad8) suporte de marketing pode remapear o campo Quantia de Oportunidade do Marketo para um campo de Oportunidade do Salesforce personalizado, desde que o tipo de campo seja moeda. Como o MPI aponta para o campo de valor da Oportunidade de marketing, o MPI pode usar os dados do campo remapeado personalizado do Salesforce.

>[!NOTE]
>
>Após o remapeamento, o MPI mostrará os dados em andamento. O valor histórico não será alterado.

## Se eu não usar oportunidades, ainda posso usar MPI? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

A MPI foi projetada para permitir que você avalie o desempenho do programa da parte superior do funil para o impacto na receita. Se você não usar oportunidades, ainda poderá:

* Desempenho de visualização dos programas de criação para participação na audiência.
* Desempenho visualização dos programas de aquisição de lead.
* Desempenho da visualização de campanhas de vários canais por meio de tags de programa.
* Veja as tendências de envolvimento da audiência nos últimos 12 meses.
* Salve e exporte dados de desempenho no PowerPoint.

## Posso medir o sucesso de estratégias baseadas em conta no MPI? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Sim. O MPI integra-se com [Marketing ABM](http://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) para inserir listas de conta ABM no MPI sem problemas. Você pode usar o filtro Lista de conta do ABM para escolher a lista do ABM desejada para filtrar os dados.

## A atribuição está disponível instantaneamente quando eu compro MPI? {#is-attribution-instantly-available-when-i-purchase-mpi}

Os recursos de Atribuição de marketing estão disponíveis para nossos clientes quando eles compram MPI. No entanto, [é necessária a configuração adequada](http://docs.marketo.com/x/mRPG) para garantir que as oportunidades e os dados do programa fluam corretamente para o MPI.

## O que devo fazer para configurar a atribuição? {#what-do-i-have-to-do-to-set-up-attribution}

1. Configuração da oportunidade

   1. Verifique se as oportunidades são sincronizadas com seu CRM
   1. Se suas configurações de Atribuição estiverem definidas como Explícita, verifique se as funções de contato nas oportunidades foram preenchidas
   1. Recomendamos alterar a configuração de Atribuição para Híbrido
   1. Configuração do programa

      1. Inclua o custo do programa em seus programas
      1. Revise o comportamento do Analytics para indicar se um programa deve ser incluído no Analytics
      1. Defina os critérios de sucesso para cada canal que você tiver
      1. Vincular pessoa aos Programas

         1. Verifique se o Programa de aquisição e a Data de aquisição foram definidos para cada pessoa no banco de dados para que a Atribuição de primeiro contato funcione.
         1. Certifique-se de que seus programas estejam configurando estados de sucesso para pessoas em seu banco de dados

>[!TIP]
>
>Todas as etapas de configuração necessárias estão detalhadas em [este artigo](http://docs.marketo.com/x/mRPG).

## Qual é a diferença entre a MPI e o Analisador de Programas? {#whats-the-difference-between-mpi-and-the-program-analyzer}

O Analisador de Programas permite que você compare seus programas em até quatro medidas. A MPI permite analisar a contribuição do canal e do programa para uma métrica escolhida, como Sucesso, Novas oportunidades criadas etc. Também permite que você visualização a tendência dos canais de 12 meses com base em uma métrica específica que você escolheu.

## Qual é a diferença entre o MPI e o Report Builder avançado? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

O Report Builder avançado (às vezes chamado de RCE) é projetado para relatórios de autoatendimento (ou ad hoc), normalmente feito pelas Operações de marketing. A MPI foi projetada para fornecer aos líderes de marketing e profissionais de marketing acesso com um clique à análise de desempenho. É necessária uma configuração mínima.

## O que aconteceu com a opção &quot;Ano anterior&quot; no filtro de datas do Contribution? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Removemos temporariamente a seleção &quot;Ano Anterior&quot;. Você ainda tem a opção de exibir os dados de desempenho do ano inteiro usando a seleção Intervalo de datas personalizado.
