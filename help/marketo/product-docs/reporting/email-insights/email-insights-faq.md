---
unique-page-id: 10100257
description: Perguntas frequentes sobre e-mail Insights - Documentos do Marketing - Documentação do produto
title: Perguntas frequentes sobre insights de email
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---


# Perguntas frequentes do Email Insights {#email-insights-faq}

## Existem diferenças entre as métricas de proporção com o Email Insights e outros relatórios de Email do Marketing? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Sim. Insights de email correlacionam métricas de envolvimento com suas métricas de delivery correspondentes para o mesmo email enviado ao calcular as taxas de métricas de envolvimento (Taxa de abertura, Taxa de clique para abrir, Taxa de cancelamento de inscrição). Por exemplo, no Email Insights, ao observar um gráfico de séries de tempo na semana passada com detalhamentos diários de Click-to-Open-Rate, agora mostramos a verdadeira proporção correlacionada de eventos abertos/clicados/cancelados com base nas métricas de delivery correspondentes. Isso contrasta com o comportamento no Explorador de Receita, que resume tudo. O Email Insights apresenta uma visualização mais precisa das taxas de envolvimento.

## Por que o Email Insights suporta apenas 10 Dimension personalizados? {#why-does-email-insights-only-support-custom-dimensions}

Para muitos casos de uso, estender as dimensões padrão do sistema com 10 dimensões personalizadas adicionais será mais do que adequado e inclui dimensões personalizadas com base em Segmentações ou Tags de Programa. No futuro, pretendemos permitir que os clientes aumentem o número de Dimension personalizados permitidos.

## Por que não posso reutilizar slots de Dimension personalizados depois de atribuídos? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Depois que um determinado slot de Dimension personalizado é alocado, remapear faz com que os dados anteriores gerem um erro quando misturados com um novo significado. Por causa disso, os slots de Dimension personalizados podem não ser reutilizados. Esse comportamento é consistente com o de outras ferramentas de análise de métricas, como Google Analytics.

## O Email Insights suporta e-mails do Marketing to Sales Insight? {#does-email-insights-support-marketo-sales-insight-emails}

Sim. Todos os emails enviados via Marketing to Sales Insights estão incluídos no Email Insights.

## O Email Insights suporta e-mails operacionais? {#does-email-insights-support-operational-emails}

Sim. Por padrão, os emails Operacionais ficam ocultos da visualização e da consulta. No entanto, você pode alterar essa configuração no painel Configurações pessoais.

## O Email Insights captura etapas recorrentes de fluxo de email programado ou de nova execução da Campanha inteligente? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Sim e Não. Com a versão inicial do Email Insights, todos os eventos de email são capturados e acessíveis para qualquer Campanha inteligente recorrente programada ou executada novamente. Mas você não será capaz de diferenciar entre diferentes execuções dessa Campanha inteligente. Estamos adicionando suporte na próxima versão para capturar as informações de execução da Campanha inteligente para eventos abertos, clicados e cancelados para diferenciar.

## Por que muitas métricas mostram zero quando eu filtro por Tipo de dispositivo ou SO de dispositivo? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Com exceção de Click-to-Open-Rate, Open, Clicks e Unsubscribes, todas as outras métricas suportadas são eventos de delivery ou taxas derivadas de eventos de delivery. Como o Tipo de dispositivo e o SO do dispositivo se aplicam somente às métricas de Envolvimento, simplesmente não temos as informações a serem exibidas. Por exemplo, é um query indefinido para solicitar a Taxa de Delivery quando filtrada pelo Tipo de dispositivo = móvel, já que o Marketo não teria recebido nenhuma métrica de Envolvimento para os eventos subjacentes Delivery e Enviado. Estamos explorando maneiras de aplicar o Tipo de dispositivo e o SO do dispositivo a partir das métricas de Envolvimento para proporções que incluem as métricas de Envolvimento e Delivery.

## O que o Email Insights faz quando determinados clientes de email bloqueiam imagens? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Um problema comum do setor é que um número cada vez maior de clientes de e-mail estão desativando as imagens por padrão. O carregamento de imagens é a base para o registro de Aberturas. É totalmente possível que um usuário receba um email com imagens bloqueadas, mas com o texto e os links totalmente legíveis. Se um usuário experimentou isso e clicou em um link nesse email, você acabaria com um cenário de um evento Click, mas nenhum evento Open correspondente para esse email. Os insights de email do Marketo gerarão automaticamente todos os eventos que estiverem faltando. A lógica é idêntica a como o Marketo faz isso para o relatório Desempenho do email, bem como a área Análise do email no Gerenciador de receitas.
