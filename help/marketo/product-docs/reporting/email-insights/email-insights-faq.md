---
unique-page-id: 10100257
description: Perguntas frequentes sobre Insights de email - Documentação do Marketo - Documentação do produto
title: Perguntas frequentes sobre o Email Insights
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Perguntas frequentes sobre o Email Insights {#email-insights-faq}

## Há diferenças entre as métricas de proporção do Email Insights e outros relatórios de email do Marketo? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Sim. Os Insights de email correlacionam as métricas de envolvimento com as métricas de entrega correspondentes para o mesmo email enviado ao calcular as taxas de métrica de envolvimento (Taxa de abertura, Taxa de clique para abertura, Taxa de cancelamento de inscrição). Por exemplo, no Email Insights, ao observar um gráfico de série temporal na semana passada com detalhamentos diários de Clique para taxa de abertura, agora mostramos a verdadeira proporção correlacionada de eventos de abertura/clique/cancelamento de inscrição com base nas métricas de entrega correspondentes. Isso contrasta com o comportamento no Revenue Explorer, que simplesmente resume tudo. O Email Insights apresenta uma exibição mais precisa das taxas de engajamento.

## Por que os Insights de email são compatíveis apenas com 10 Dimension personalizados? {#why-does-email-insights-only-support-custom-dimensions}

Para muitos casos de uso, estender as dimensões padrão do sistema com 10 dimensões personalizadas adicionais será mais do que adequado e inclui dimensões personalizadas com base em Segmentações ou Tags de programa. No futuro, pretendemos permitir que os clientes aumentem o número de Dimension personalizados permitidos.

## Por que não posso reutilizar os slots de Dimension personalizados depois que forem atribuídos? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Depois que um determinado slot de Dimension personalizado é alocado, o remapeamento faz com que os dados anteriores produzam um erro quando combinados com um novo significado. Por esse motivo, os slots de Dimension personalizados não podem ser reutilizados. Esse comportamento é consistente com o de outras ferramentas de análise de métrica, como Google Analytics.

## O Email Insights é compatível com os emails do Marketo Sales Insight? {#does-email-insights-support-marketo-sales-insight-emails}

Sim. Todos os emails enviados pelo Marketo Sales Insights estão incluídos em Email Insights.

## O Email Insights é compatível com emails operacionais? {#does-email-insights-support-operational-emails}

Sim. Por padrão, os Emails operacionais ficam ocultos na exibição e na consulta. No entanto, você pode alterar essa configuração no painel Configurações pessoais.

## Os Insights de email capturam etapas recorrentes de fluxo de email programadas ou executadas novamente no Smart Campaign? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Sim e Não. Com o lançamento inicial do Email Insights, todos os eventos de email são capturados e acessíveis para qualquer campanha inteligente recorrente programada ou executada novamente. Mas você não será capaz de diferenciar as diferentes execuções dessa Campanha inteligente. Estamos adicionando suporte em nossa próxima versão para capturar as informações de execução do Smart Campaign para eventos de abertura, clique e cancelamento de inscrição para fazer a diferenciação.

## Por que muitas métricas mostram zero quando eu filtro por Tipo de dispositivo ou Sistema operacional do dispositivo? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Com exceção de Clique para taxa de abertura, Aberturas, Cliques e Cancelamentos de assinatura, todas as outras métricas compatíveis são eventos de entrega ou taxas derivadas de eventos de entrega. Como o Tipo de dispositivo e o SO do dispositivo se aplicam apenas às métricas de Envolvimento, simplesmente não temos as informações para exibir. Por exemplo, é uma consulta indefinida solicitar a Taxa de entrega quando filtrada por Tipo de dispositivo = móvel, já que o Marketo não teria recebido métricas de Envolvimento para os eventos subjacentes Entrega e Envio. Estamos explorando maneiras de aplicar o Tipo de dispositivo e o SO do dispositivo a partir das métricas de envolvimento para proporções compostas pelas métricas de Envolvimento e Entrega.

## O que o Email Insights faz quando determinados clientes de email bloqueiam imagens? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Um problema comum do setor é que um número cada vez maior de clientes de email está desativando imagens por padrão. O carregamento de imagens é a base para o registro de aberturas. É perfeitamente possível que um usuário receba um email com imagens bloqueadas, mas com o texto e os links totalmente legíveis. Se um usuário tiver essa experiência e clicar em um link nesse email, você acabará com um cenário de um evento Click, mas nenhum evento Open correspondente para esse email. O Marketo Email Insights gerará automaticamente todos os eventos que estavam ausentes. A lógica é idêntica à forma como o Marketo faz isso para o Relatório de desempenho de email, bem como para a área de Análise de email no Revenue Explorer.
