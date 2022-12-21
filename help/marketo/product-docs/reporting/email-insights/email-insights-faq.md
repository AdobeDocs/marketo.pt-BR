---
unique-page-id: 10100257
description: Perguntas frequentes sobre insights de email - Documentos do Marketo - Documentação do produto
title: Perguntas frequentes sobre insights de email
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Perguntas frequentes sobre insights de email {#email-insights-faq}

## Existem diferenças entre as métricas de proporção com o Email Insights e outros relatórios de email do Marketo? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Sim. Os Insights de email correlacionam as métricas de envolvimento com suas métricas de delivery correspondentes para o mesmo email enviado ao calcular as taxas de métrica de envolvimento (Taxa de abertura, Taxa de clique para abrir, Taxa de cancelamento de inscrição). Por exemplo, no Email Insights, ao analisar um gráfico de séries de tempo na semana passada com detalhamentos diários da Taxa de clique para abrir, agora mostramos a verdadeira proporção correlacionada de eventos de abertura/clique/cancelamento de inscrição com base nas métricas de delivery correspondentes. Isso contrasta com o comportamento no Explorador de receita, que simplesmente resume tudo. O Email Insights apresenta uma exibição mais precisa das taxas de engajamento.

## Por que o Email Insights suporta apenas 10 Dimension personalizados? {#why-does-email-insights-only-support-custom-dimensions}

Para muitos casos de uso, a extensão das dimensões padrão do sistema com 10 dimensões personalizadas adicionais será mais do que adequada e inclui dimensões personalizadas com base em Segmentações ou Tags de programa. No futuro, pretendemos permitir que os clientes aumentem o número de Dimension personalizados permitidos.

## Por que não posso reutilizar slots de Dimension personalizados depois de atribuídos? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Depois que um determinado slot de Dimension personalizado é alocado, remapear o slot faz com que os dados anteriores gerem um erro ao serem combinados com um novo significado. Por causa disso, os slots de Dimension personalizado não podem ser reutilizados. Esse comportamento é consistente ao de outras ferramentas de análise de métrica, como o Google Analytics.

## Os Email Insights são compatíveis com os emails do Marketo Sales Insight? {#does-email-insights-support-marketo-sales-insight-emails}

Sim. Todos os emails enviados via Marketo Sales Insights são incluídos em Email Insights.

## Os Insights de email são compatíveis com emails operacionais? {#does-email-insights-support-operational-emails}

Sim. Por padrão, os emails Operacionais são ocultos da exibição e da consulta. No entanto, você pode alterar essa configuração no painel Configurações pessoais .

## O Email Insights captura etapas recorrentes de fluxo de email programadas ou reexecutadas do Smart Campaign? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Sim e Não. Com a versão inicial do Email Insights, todos os eventos de email são capturados e acessíveis para qualquer campanha inteligente recorrente agendada ou executada novamente. Mas você não será capaz de diferenciar entre diferentes execuções dessa Campanha Inteligente. Estamos adicionando suporte em nossa próxima versão para capturar as informações de execução da Campanha inteligente para eventos Abertos, Clicados e Cancelar assinatura para diferenciar.

## Por que muitas métricas mostram zero quando eu filtro por Tipo de dispositivo ou SO de dispositivo? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Com exceção de Click-to-Open-Rate, Opens, Clicks e Unsubscribes, todas as outras métricas compatíveis são eventos de delivery ou taxas derivadas de eventos de delivery. Como o Tipo de dispositivo e o SO do dispositivo se aplicam apenas às métricas de Envolvimento, simplesmente não temos as informações para exibir. Por exemplo, é uma consulta indefinida solicitar a Taxa de entrega quando filtrada pelo Tipo de dispositivo = móvel, já que o Marketo não teria recebido métricas de Envolvimento para os eventos subjacentes de Entrega e Enviado. Estamos explorando maneiras de aplicar o Tipo de dispositivo e o SO do dispositivo a partir de métricas de Envolvimento para taxas compostas por métricas de Envolvimento e Delivery.

## O que o Email Insights faz quando determinados clientes de email bloqueiam imagens? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Um problema comum do setor é que um número crescente de clientes de email está desativando imagens por padrão. O carregamento de imagens é a base de como as Aberturas são registradas. É totalmente possível que um usuário receba um email com imagens bloqueadas, mas com o texto e os links totalmente legíveis. Se um usuário experimentou isso e clicou em um link nesse email, você acabaria com um cenário de um evento Click , mas nenhum evento Open correspondente para esse email. O Marketo Email Insights gerará automaticamente todos os eventos que estiverem faltando. A lógica é idêntica à forma como o Marketo faz isso no relatório de Desempenho de email, bem como na área Análise de email no Explorador de receita.
