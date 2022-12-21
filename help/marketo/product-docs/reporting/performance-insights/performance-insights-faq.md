---
unique-page-id: 12979858
description: Perguntas frequentes sobre o Performance Insights - Documentos do Marketo - Documentação do produto
title: Perguntas frequentes sobre o Performance Insights
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1357'
ht-degree: 0%

---

# Perguntas frequentes sobre o Performance Insights {#performance-insights-faq}

## Qual é a definição de &quot;sucesso&quot; na guia Envolvimento? {#what-is-the-definition-of-success-in-the-engagement-tab}

O sucesso é uma medida de interação significativa no Marketo. A finalidade de um programa é criar uma interação significativa com a pessoa ou prospecto. O sucesso é marcado quando uma pessoa atinge o status que atinge esse objetivo. Ele pode estar participando de um webinário, clicando em um link em um email ou preenchendo um formulário da Web. O sucesso varia dependendo do canal do programa.

>[!NOTE]
>
>Em um programa de webinar, pode haver vários status, como: Convidado, registrado e assistido. Convidado ou registrado não são interações significativas porque as pessoas não assistem ao webinário. Nesse caso, a participação é considerada um sucesso.

## O MPI funcionará com qualquer CRM? {#will-mpi-work-with-any-crm}

Sim. Tecnicamente, a MPI não interage diretamente com o CRM para sincronização de dados. A MPI utiliza dados armazenados na Data Warehouse do Marketo Analytics. Como a sincronização do CRM acontece no aplicativo de Gerenciamento de clientes potenciais, qualquer CRM suportado pela Marketo integrado ao aplicativo de Gerenciamento de clientes potenciais mostrará os dados corretamente. No entanto, os campos de oportunidade do CRM precisam ser mapeados corretamente para os campos de oportunidade do Marketo.

## Não tenho nenhum outro produto do Marketing Analytics (ARB, RCE, RCA, Análise do Programa). O MPI funcionará para mim? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

O MPI é um complemento independente do aplicativo de Gerenciamento de clientes potenciais. Não requer o uso de nenhum outro produto de análise.

## A RCA também mostra os dados de desempenho do programa. Existe uma diferença entre os dados mostrados em MPI e RCA? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

Nº Os dados de origens MPI do mesmo data warehouse que o RCA. Portanto, você não verá diferenças de dados entre os dois. O RCA permite criar seus próprios relatórios em tempo real. O MPI fornece acesso a painéis visuais fáceis de entender.

## Não quero que alguns dos meus programas (por exemplo, operacionais) apareçam em MPI. Como controlar a visibilidade de programas específicos? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

Você pode controlar a visibilidade de seus programas definindo o comportamento do Analytics de seus programas como Operacional. Isso fará com que o programa seja excluído dos cálculos do Analytics.

>[!NOTE]
>
>Saiba mais sobre como configurar o comportamento do Analytics [here](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md).

## Estou executando uma campanha multicanal para um novo lançamento de produto. Como posso visualizar o desempenho desta campanha em todos os canais diferentes em um único lugar? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Recomendamos que, para programas que fazem parte dessa campanha, você utilize tags de programa. As tags de programa são sincronizadas automaticamente com MPI e você pode filtrá-las em todos os painéis MPI para visualizar o desempenho da campanha de vários canais.

## Terei acesso às configurações de atribuição se não tiver RCA? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Você obtém acesso às configurações de atribuição se tiver MPI, independentemente de ter RCA ou não.

## Recebo um alerta no MPI quando faço logon informando que as configurações de atribuição estão incorretas. O que há de errado? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

O MPI calcula se todas as suas oportunidades estão ou não sendo incluídas no Analytics. Caso contrário, você será solicitado a considerar a alteração das configurações de atribuição (explícito, implícito, híbrido) para incluir mais oportunidades.

Você também pode estar perdendo oportunidades devido ao custo do programa ausente em seus programas. Revise o comportamento do Analytics de seus programas. Eles podem ser:

1. Padrão - O comportamento padrão é que o programa seria incluído no MPI SOMENTE se houvesse pelo menos um custo de período, mesmo um com dólares zero atribuídos.

1. Inclusivo - Essa opção garantirá que o programa esteja disponível no MPI, independentemente de você ter ou não incluído um custo do período.

1. [Operacional](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs) - Essa opção faz com que o programa não apareça no MPI.

>[!NOTE]
>
>Custo do Período **has** a ser configurado para relatórios de Sucesso e Novos Nomes no painel Envolvimento. Esse painel utiliza os dados de Custo do Período para agregar sucessos e novos nomes. Se o Custo do Período não estiver configurado, o painel de envolvimento não será relatado corretamente, independentemente das configurações de comportamento do Analytics acima.

## Por que estou perdendo algumas oportunidades no MPI? {#why-am-i-missing-some-opportunities-in-mpi}

Dois motivos principais pelas quais podem estar faltando oportunidades no MPI são:

1. A configuração de atribuição é definida como Explícito, mas as oportunidades não têm Funções de Contato atribuídas
1. O custo do período não está incluído em seus programas

O MPI calcula se todas as suas oportunidades estão ou não sendo incluídas no Analytics. Caso contrário, você será solicitado a considerar a alteração das configurações de atribuição (explícito, implícito, híbrido) para incluir mais oportunidades.

Você também pode estar perdendo oportunidades devido ao custo do programa ausente em seus programas. O alerta aparecerá, mas não aponta para quais programas estão faltando custos. Revise a configuração do seu programa para incluir custos, para garantir que todos os seus programas e oportunidades estejam incluídos no MPI.

## Por que não vejo Campos personalizados, Tipo de oportunidade e filtros ABM no painel Envolvimento? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

Campos personalizados, Tipo de oportunidade e Filtros ABM são todos atributos relacionados a uma oportunidade. O painel Envolvimento permite medir seu engajamento e aquisição de cliente potencial, estejam ou não associados a uma oportunidade. Como o painel Envolvimento não aproveita a oportunidade, os Campos personalizados, o Tipo de oportunidade e os Filtros de ABM não se aplicam.

## Desejo usar um campo Oportunidade do Salesforce personalizado para o relatório de receita em vez do campo Quantia de Oportunidade do Salesforce. O MPI permitirá que eu faça isso? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Sim. [Suporte Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) O é capaz de remapear o campo Quantia da Oportunidade da Marketo para um campo da Oportunidade do Salesforce personalizado, desde que o tipo de campo seja moeda. Como o MPI aponta para o campo Valor da oportunidade do Marketo , o MPI pode usar os dados do campo Salesforce personalizado remapeado.

>[!NOTE]
>
>Após o remapeamento, o MPI mostrará os dados a partir de agora. O valor histórico não será alterado.

## Se eu não usar oportunidades, ainda posso usar MPI? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

O MPI foi projetado para permitir medir o desempenho do programa desde o topo do funil até o impacto na receita. Se você não usar oportunidades, ainda poderá:

* Veja o desempenho de seus programas de criação para o envolvimento do público-alvo.
* Veja o desempenho dos seus programas de aquisição de clientes potenciais.
* Visualize o desempenho de campanhas multicanal por meio de tags de programa.
* Veja as tendências de engajamento do público-alvo nos últimos 12 meses.
* Salve e exporte dados de desempenho no PowerPoint.

## Posso medir o sucesso das estratégias baseadas em conta no MPI? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Sim. MPI integra-se com [Marketo TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) para inserir listas de contas ABM no MPI sem interrupções. Você pode usar o filtro Lista de contas ABM para escolher a lista ABM desejada para filtrar dados.

## A atribuição está instantaneamente disponível ao comprar MPI? {#is-attribution-instantly-available-when-i-purchase-mpi}

Os recursos de Atribuição da Marketo estão disponíveis para nossos clientes quando eles compram MPI. No entanto, [configuração correta](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) é necessário para garantir que as oportunidades e os dados do programa fluam corretamente para o MPI.

## O que devo fazer para configurar a atribuição? {#what-do-i-have-to-do-to-set-up-attribution}

1. Configuração da oportunidade

   1. Garanta que as oportunidades sejam sincronizadas com seu CRM
   1. Se suas Configurações de atribuição forem definidas como Explicito, verifique se as funções de contato nas oportunidades são preenchidas
   1. Recomendamos alterar a configuração Atribuição para Híbrido
   1. Configuração de programa

      1. Inclua o custo do programa em seus programas
      1. Revise o comportamento do analytics para indicar se um programa deve ser incluído no analytics
      1. Definir os critérios de sucesso para cada canal
      1. Vincular pessoa aos programas

         1. Verifique se o Programa de aquisição e a Data de aquisição foram definidos para cada pessoa no banco de dados para que a Atribuição de primeiro contato funcione.
         1. Verifique se os programas estão definindo estados de sucesso para pessoas no banco de dados

>[!TIP]
>
>Todas as etapas de configuração necessárias estão detalhadas em [este artigo](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md).

## Qual é a diferença entre MPI e o Analisador de programas? {#whats-the-difference-between-mpi-and-the-program-analyzer}

O Program Analyzer permite comparar seus programas com até quatro medidas. A MPI permite analisar a contribuição do canal e do programa para uma métrica escolhida, como Sucesso, Novas oportunidades criadas etc. Também permite visualizar a tendência do canal de 12 meses com base em uma métrica específica escolhida.

## Qual é a diferença entre MPI e o Report Builder Avançado? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

O Advanced Report Builder (às vezes chamado de RCE) foi projetado para relatórios de autoatendimento (ou ad hoc), normalmente feitos por operações de marketing. O MPI foi projetado para fornecer aos líderes de marketing e profissionais de marketing acesso com um clique à análise de desempenho. É necessária uma configuração mínima.

## O que aconteceu com a opção &quot;Ano anterior&quot; no filtro de datas da Contribuição? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Removemos temporariamente a seleção do &quot;Ano anterior&quot;. Você ainda tem a opção de exibir os dados de desempenho do ano inteiro usando a seleção Intervalo de datas personalizado .
