---
unique-page-id: 12979858
description: Perguntas frequentes sobre o Performance Insights - Documentação do Marketo - Documentação do produto
title: Perguntas frequentes sobre insights de desempenho
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1346'
ht-degree: 0%

---

# Perguntas frequentes sobre insights de desempenho {#performance-insights-faq}

## Qual é a definição de &quot;sucesso&quot; na guia Engajamento? {#what-is-the-definition-of-success-in-the-engagement-tab}

O sucesso é uma medida de interação significativa no Marketo. O objetivo de um programa é criar uma interação significativa com a pessoa ou prospecto. O sucesso é marcado quando uma pessoa atinge o status que atinge essa meta. Ele pode estar participando de um webinário, clicando em um link em um email ou preenchendo um formulário web. O sucesso varia dependendo do canal do programa.

>[!NOTE]
>
>Em um programa de webinário, pode haver vários status, como: Convidado, Registrado e Presente. Convidados ou registrados não são interações significativas porque as pessoas não assistem ao webinário. Participou é considerado sucesso neste caso.

## O MPI funcionará com algum CRM? {#will-mpi-work-with-any-crm}

Sim. Tecnicamente, o MPI não interage diretamente com o CRM para sincronização de dados. O MPI utiliza dados armazenados na Data Warehouse do Marketo Analytics. Como a sincronização do CRM acontece no aplicativo de gerenciamento de clientes potenciais, qualquer CRM compatível com a Marketo e integrado ao aplicativo de gerenciamento de clientes potenciais mostrará os dados corretamente. No entanto, os campos de oportunidade do CRM precisam ser mapeados corretamente para os campos de oportunidade do Marketo.

## Não tenho nenhum outro produto no Marketing Analytics (ARB, RCE, RCA, Program Analysis). O MPI funcionará para mim? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

O MPI é um complemento independente do aplicativo de gerenciamento de clientes potenciais. Ela não requer o uso de nenhum outro produto de análise.

## A RCA também me mostra os dados de desempenho do programa. Há uma diferença entre os dados mostrados em MPI e RCA? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

Nº O MPI origina dados do mesmo data warehouse que o RCA. Portanto, você não verá diferenças de dados entre os dois. A RCA permite criar seus próprios relatórios dinamicamente. O MPI fornece acesso a painéis visuais fáceis de entender.

## Não quero que alguns dos meus programas (por exemplo, Operacionais) sejam exibidos em MPI. Como controlar a visibilidade de programas específicos? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

Você pode controlar a visibilidade de seus programas definindo o comportamento Analytics de seus programas como Operacional. Isso fará com que o programa seja excluído dos cálculos de análise.

>[!NOTE]
>
>Saiba mais sobre como definir o comportamento da análise [aqui](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md).

## Estou executando uma campanha multicanal para um novo lançamento de produto. Como posso visualizar o desempenho dessa campanha em todos os canais diferentes em um único local? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Recomendamos que, para programas que fazem parte de uma campanha desse tipo, você utilize tags de programa. As tags de programa são sincronizadas automaticamente com o MPI e você pode filtrá-las em todos os painéis de MPI para visualizar o desempenho da campanha multicanal.

## Terei acesso às configurações de atribuição se não tiver o RCA? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Você terá acesso às configurações de atribuição se tiver MPI, independentemente de ter RCA ou não.

## Quando faço logon, recebo um alerta em MPI informando que minhas configurações de atribuição estão incorretas. O que há de errado? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

O MPI calcula se todas as oportunidades estão ou não sendo incluídas no Analytics. Caso contrário, você será solicitado a considerar a alteração das configurações de atribuição (Explícito, Implícito, Híbrido) para incluir mais oportunidades.

Você também pode estar perdendo oportunidades devido ao custo do programa que está faltando em seus programas. Revise o comportamento do Analytics de seus programas. Eles podem ser:

1. Padrão - O comportamento padrão é o programa ser incluído SOMENTE no MPI se houver pelo menos um custo do período, mesmo um com zero dólares atribuídos.

1. Inclusivo - Essa opção garantirá que o programa esteja disponível em MPI, independentemente de você ter ou não incluído um custo do período.

1. [Operacional](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs) - Esta opção faz com que o programa não apareça em MPI.

>[!NOTE]
>
>O Custo do Período **tem** para ser configurado para os relatórios de Sucesso e Novos Nomes no painel Envolvimento. Esse painel usa dados de Custo do Período para agregar sucessos e novos nomes. Se o Custo do período não estiver configurado, o painel de engajamento não será relatado corretamente independentemente das configurações de comportamento do Analytics acima.

## Por que estou perdendo algumas oportunidades no MPI? {#why-am-i-missing-some-opportunities-in-mpi}

Dois motivos principais para você perder oportunidades na MPI são:

1. A configuração Atribuição está definida como Explícito, mas as oportunidades não têm Funções de contato atribuídas
1. O custo do período não está incluído em seus programas

O MPI calcula se todas as oportunidades estão ou não sendo incluídas no Analytics. Caso contrário, você será solicitado a considerar a alteração das configurações de atribuição (Explícito, Implícito, Híbrido) para incluir mais oportunidades.

Você também pode estar perdendo oportunidades devido ao custo do programa que está faltando em seus programas. O alerta será exibido, mas não indica a você quais programas estão com custos faltando. Revise a configuração de seu programa para incluir custos, para garantir que todos os seus programas e oportunidades estejam incluídos no MPI.

## Por que não vejo campos personalizados, tipo de oportunidade e filtros ABM no painel Envolvimento? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

Campos Personalizados, Tipo de Oportunidade e Filtros ABM são atributos relacionados a uma oportunidade. O painel Engajamento permite medir o engajamento e a aquisição de clientes potenciais, estejam ou não associados a uma oportunidade. Como o painel Envolvimento não leva a oportunidade em consideração, os Campos personalizados, o Tipo de oportunidade e os Filtros ABM não se aplicam.

## Quero usar um campo personalizado de Oportunidade do Salesforce para relatórios de receita em vez do campo padrão de Valor de Oportunidade do Salesforce. O MPI me permitirá fazer isso? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Sim. O [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) pode remapear o campo Valor da Oportunidade da Marketo para um campo personalizado de Oportunidade da Salesforce, desde que o tipo de campo seja moeda. Como o MPI aponta para o campo de valor de oportunidade da Marketo, o MPI pode usar os dados do campo personalizado remapeado do Salesforce.

>[!NOTE]
>
>Após o remapeamento, o MPI mostrará os dados a partir de agora. O valor do histórico não será alterado.

## Se eu não usar as oportunidades, ainda posso usar o MPI? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

A MPI foi projetada para permitir medir o desempenho do programa desde a parte superior do funil até o impacto na receita. Se você não usar as oportunidades, ainda será capaz de:

* Visualize o desempenho de seus programas de criação para o envolvimento do público-alvo.
* Exibir o desempenho de seus programas de aquisição de clientes potenciais.
* Visualize o desempenho de campanhas multicanal por meio de tags de programa.
* Consulte Tendências de envolvimento do público-alvo nos últimos 12 meses.
* Salvar e exportar dados de desempenho no PowerPoint.

## Posso medir o sucesso das estratégias baseadas em conta no MPI? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Sim. O MPI integra-se ao [Marketo TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) para transferir listas de contas ABM para o MPI de forma contínua. Você pode usar o filtro Lista de Contas do ABM para escolher a lista do ABM desejada para filtrar os dados.

## A atribuição fica disponível instantaneamente quando eu compro MPI? {#is-attribution-instantly-available-when-i-purchase-mpi}

Os recursos de atribuição do Marketo estão disponíveis para nossos clientes ao comprarem MPI. No entanto, é necessária uma [configuração adequada](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) para garantir que as oportunidades e os dados do programa fluam corretamente para o MPI.

## O que devo fazer para configurar a atribuição? {#what-do-i-have-to-do-to-set-up-attribution}

1. Configuração de oportunidade

   1. Verifique se as oportunidades estão sincronizadas com seu CRM
   1. Se as configurações de Atribuição estiverem definidas como Explícito, verifique se as funções de contato nas oportunidades estão preenchidas
   1. Recomendamos alterar a configuração de Atribuição para Híbrido
   1. Configuração de programa

      1. Incluir o custo do programa em seus programas
      1. Revise o comportamento da análise para indicar se um programa deve ser incluído na análise
      1. Defina os critérios de sucesso para cada canal que você tiver
      1. Vincular pessoa aos programas

         1. Verifique se o Programa de aquisição e a Data de aquisição foram definidos para cada pessoa no banco de dados para que a Atribuição de primeiro contato funcione.
         1. Verifique se os programas estão definindo estados de sucesso para as pessoas no banco de dados

>[!TIP]
>
>Todas as etapas de instalação necessárias estão detalhadas em [este artigo](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md).

## Qual é a diferença entre o MPI e o Program Analyzer? {#whats-the-difference-between-mpi-and-the-program-analyzer}

O Analisador de programas permite comparar seus programas em até quatro medidas. O MPI permite analisar a contribuição do canal e do programa para uma métrica escolhida, como Sucesso, Novas oportunidades criadas etc. Também permite visualizar a tendência do canal de 12 meses com base em uma métrica específica escolhida.

## Qual é a diferença entre o MPI e o Report Builder avançado? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

O Report Builder avançado (às vezes chamado de RCE) foi projetado para relatórios de autoatendimento (ou ad hoc), normalmente feitos por Operações de marketing. A MPI foi projetada para fornecer aos líderes de marketing e profissionais de marketing acesso com um clique à análise de desempenho. A configuração mínima é necessária.

## O que aconteceu com a opção &quot;Ano anterior&quot; no filtro de datas da Contribuição? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Removemos temporariamente a seleção &quot;Ano anterior&quot;. Você ainda tem a opção de exibir os dados de desempenho do ano inteiro usando a seleção de Intervalo de datas personalizado.
