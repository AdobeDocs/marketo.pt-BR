---
unique-page-id: 2951114
description: Notas de versão - junho de 2012 - Documentação da Marketo - Documentação do produto
title: Notas de versão - junho de 2012
exl-id: c22eda86-da7a-4c76-9cea-1ce23ff0f3e8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---

# Notas de versão: Junho de 2012 {#release-notes-june}

## Aprimoramentos de gerenciamento de clientes potenciais da Marketo {#marketo-lead-management-enhancements}

### Renomear {#rename}

É possível renomear as Smart Lists, as listas estáticas e as campanhas. Se você estiver usando esses ativos em filtros, acionadores ou fluxos, o nome também será atualizado automaticamente lá. Sempre foi possível renomear emails, formulários e pastas.

E, como bônus, melhoramos a inserção e a exibição de texto de descrição para ativos.

![](assets/image2014-9-23-10-3a23-3a10.png)

## Importar mapeamento de campos {#import-field-mapping}

Facilitamos muito a importação de uma lista para o Marketo! Durante o processo de importação, é possível mapear o nome do campo Marketo para o nome do cabeçalho da coluna no arquivo de importação. Além disso, em Admin, é possível configurar nomes de alias mapeados para o nome do campo no Marketo, garantindo que os usuários selecionem o campo correto sempre.

À medida que você continua importando e mapeando campos, a Marketo lembrará e exibirá os mapeamentos durante a importação para facilitar o uso. E para tornar a vida ainda mais fácil, você pode clicar no cabeçalho Valor de exemplo para ver os diferentes valores que seriam preenchidos no campo . Isso ajuda a garantir que você mapeie o campo correto todas as vezes!

![](assets/image2014-9-23-10-3a23-3a27.png)

## Página de resumo das Listas inteligentes e Listas estáticas {#summary-page-for-smart-lists-and-static-lists}

Você já se perguntou onde suas listas estão sendo usadas? Ou quem criou a lista ou a modificou pela última vez? A nova página de resumo disponível em Smart Lists e listas estáticas fornecerá esses detalhes importantes.

![](assets/image2014-9-23-10-3a23-3a40.png)

Nas páginas existentes de resumo do Programa e da Campanha, adicionamos as informações Data/Usuário Criado e Data/Usuário da Última Modificação também!

![](assets/image2014-9-23-10-3a23-3a54.png)

## Usado por para Ativos {#used-by-for-assets}

Adicionamos uma nova guia às Páginas de resumo do ativo, chamada Usado por!

![](assets/image2014-9-23-10-3a24-3a5.png)

Exemplo: Usado por para listas estáticas

## Linhas de grade da página de aterrissagem {#landing-page-gridlines}

A adição das linhas de grade da página de aterrissagem facilita muito o alinhamento de texto, gráficos e formulários na página de aterrissagem. Ative e desative para qualquer landing page e ajuste a largura entre as linhas!

![](assets/image2014-9-23-10-3a24-3a19.png)

![](assets/image2014-9-23-10-3a24-3a33.png)

## Clientes Potenciais Bloqueados de Correções {#leads-blocked-from-mailings}

Ao agendar uma campanha, você pode clicar no link para ver a lista de leads que são bloqueados em sua mala direta.

![](assets/image2014-9-23-10-3a24-3a51.png)

## Etapa de espera - Token de lead e Meu token {#wait-step-lead-token-and-my-token}

Na versão de maio, adicionamos opções avançadas à etapa Fluxo de espera . Com essas alterações, você pode especificar um dia útil, data e hora. Nesta versão, adicionamos a capacidade de usar um token na etapa de espera. Por exemplo, você pode usar `{{lead.Birthday}}` para enviar um email no Aniversário ou usar `{{my.Event Date}}` para enviar um lembrete de webinar final.

![](assets/image2014-9-23-10-3a25-3a57.png)

## Exibir como miniaturas no Design Studio {#view-as-thumbnails-in-design-studio}

Alterne sua exibição de uma lista de imagens para uma exibição em miniatura!

![](assets/image2014-9-23-10-3a26-3a13.png)

Observação: A partir desta versão, a classificação anterior nas grades da lista inteligente não se aplicará à próxima lista inteligente que você exibir. Por exemplo, se você classificar uma lista inteligente por Nome da empresa, não classificaremos automaticamente a próxima lista inteligente exibida por esse mesmo campo.

Lembrete: A atualização do Relatório de desempenho de email está em andamento!

## Aprimoramentos do Marketo Revenue Cycle Analytics {#marketo-revenue-cycle-analytics-enhancements}

### Novas métricas na análise de oportunidade do programa {#new-metrics-in-program-opportunity-analysis}

Agora você pode obter insights sobre o número médio de toques de marketing antes que as oportunidades sejam criadas ou fechadas, bem como o valor médio de um toque de marketing.

![](assets/image2014-9-23-10-3a26-3a30.png)

![](assets/image2014-9-23-10-3a26-3a41.png)

## Exibição de vários gráficos {#displaying-multi-charts}

O recurso de vários gráficos permite exibir vários gráficos em um único relatório do Revenue Cycle Explorer. Por exemplo, você pode usar esse recurso quando quiser exibir os mesmos dados em meses diferentes. Esse recurso também evita que você tenha que criar filtros e relatórios separados.

![](assets/image2014-9-23-10-3a27-3a41.png)

## Tipo de Gráfico de Grade de Calor {#heat-grid-chart-type}

As grades de calor permitem a capacidade de visualizar dados para que você possa identificar padrões de desempenho do Marketing. Esse tipo de visualização codificará os resultados em cores, de modo que você visualize análises comerciais complexas em uma visualização fácil de entender.

![](assets/image2014-9-23-10-3a28-3a21.png)

## Tipo de Gráfico de Dispersão {#scatter-chart-type}

Os gráficos de dispersão ajudam a visualizar dados em várias dimensões em um gráfico. Esse tipo de visualização representará uma bolha em um gráfico com base nos atributos usados. Em seguida, é possível usar uma medida para codificar a bolha com cores e/ou usar uma medida para especificar o tamanho da bolha.

![](assets/image2014-9-23-10-3a29-3a7.png)
