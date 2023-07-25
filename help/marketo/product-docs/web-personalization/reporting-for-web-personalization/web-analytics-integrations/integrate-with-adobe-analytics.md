---
unique-page-id: 2949160
description: Integração com o Adobe Analytics - Documentação do Marketo - Documentação do produto
title: Integrar ao Adobe Analytics
exl-id: 6ea35811-6f3d-4dc8-91aa-877d613f8e93
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---

# Integrar ao Adobe Analytics {#integrate-with-adobe-analytics}

## Introdução {#intro}

Analise sua análise da Web de uma perspectiva B2B visualizando dados de campanha de organização, setor e Personalização em tempo real (RTP) da Marketo na sua conta do Adobe Analytics.

Este documento habilita a integração entre a Personalização em tempo real (RTP) da Marketo e o Adobe Adobe Analytics. Os dados da RTP permitirão detectar e analisar tendências em todos os segmentos do setor e organizações que visitam seu site e medir a eficácia de suas campanhas RTP, fornecendo os insights e análises para obter os melhores resultados.

Você pode fazer isso observando métricas como os números de visitantes novos e recorrentes em cada segmento, analisando taxas de clique em campanhas e descobrindo quais setores, segmentos personalizados e campanhas em tempo real geraram os melhores leads de conversão. Aproveite essa capacidade para obter o máximo benefício da sua conta RTP.

## AUDIENCE ANALYTICS RTP {#rtp-audience-analytics}

Com a integração RTP - AA, você tem uma nova dimensão na interface de análise da Web. O RTP melhora automaticamente seus painéis de análise da Web com:

1. Dados da organização e do setor
1. Segmentos personalizados do RTP
1. Listas de contas nomeadas (Account-Based Marketing)

Isso melhora seus dados B2B e permite que você se concentre em visitantes relevantes, otimizando:

1. Canais de saída
1. Conteúdo
1. Redirecionamento

## Relatório de canal {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

O painel de RTP ajuda você a entender o detalhamento de seus visitantes de acordo com os segmentos verticais e RTP. Você pode ver o desempenho do visitante de acordo com o setor e as diferentes campanhas de marketing (pagas, orgânicas, sociais) relacionadas a esse setor. O painel também fornece uma visão geral de alto nível de quais seções do site seus visitantes estão visualizando, de acordo com o tipo de setor.

## Relatório comportamental {#behavioral-report}

Relatórios de comportamento diferentes podem ser criados no Adobe Analytics com base nos dados de organização, setor e segmento RTP. Esses Relatórios de fluxo visualizam o caminho que os visitantes tomam de uma Página ou Evento para a próxima. Este relatório pode ajudar você a descobrir qual conteúdo mantém os visitantes envolvidos com seu site.

## Desempenho de RTP {#rtp-performance}

Exiba impressões e conversões da campanha RTP em Links personalizados na Adobe Analytics.

Este relatório de Link personalizado mostrará impressões e conversões de campanhas no seguinte formato de nomenclatura:

* Segmento de impressão: [Nome do segmento RTP], ICampaign: [Nome da campanha RTP]
* Segmento de conversão: [Nome do segmento RTP], ICampaign: [Nome da campanha RTP]

![](assets/custom-links-report.png)

## Configurar no Adobe Analytics {#set-up-in-adobe-analytics}

A integração usa a API JavaScript que o Adobe Analytics oferece. As variáveis de conversão personalizadas (eVar), eventos personalizados (evento) e variáveis de tráfego são usadas na integração. Todos devem ser ativados no administrador do AA. Você deve definir as variáveis de conversão, os eventos personalizados e as variáveis de tráfego no AA ou não será possível ver os dados no conjunto, mesmo que você os tenha ativado no RTP.

Conclua as etapas a seguir para configurar essas variáveis no AA:

1. Ir para **Ferramentas administrativas** na sua conta do AA.
1. Selecione o **Report Suite** para ser usado com a integração.
1. Em **Editar configurações**, vá para **Conversão** e selecione **[Variáveis de conversão](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**.\
   Selecione o [Variável de conversão](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) número (recomendamos):

   1. Evar nº 20 para conversões personalizadas do setor
   1. Evar nº 21 para conversões personalizadas de organização

   >[!NOTE]
   >
   >Se esses # forem usados, selecione outro número disponível. Alinhe esse número com o número do slot nas Configurações da conta RTP.

   1. Alterar status para _Ativado_.

      1. Alterar nome para **Setor** e **Organização**. (É assim que ele será exibido no Conjunto de relatórios.)

      1. Alterar campo Expirar após para **Visita**.

1. Em **Editar configurações** ir para **Conversão** e selecione **[Eventos bem-sucedidos](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**.

   1. Selecione o número do Evento bem-sucedido personalizado (recomendamos):

      1. event20 para Campanhas RTP
      1. event21 para segmentos RTP

      >[!NOTE]
      >
      >Se esses # forem usados, selecione outro número disponível. Alinhe esse número com o número do slot nas Configurações da conta RTP.

      1. Altere os nomes dos dois eventos para **Campanhas RTP** e **Segmentos RTP**. Esse é o nome que aparecerá no Conjunto de relatórios.

   1. Selecione o campo Type a ser **Contador (sem sub-relações)**

1. Em **Editar configurações** ir para **[Tráfego](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable)** e selecione **[Variáveis de tráfego](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**.

   1. Selecione o número de propriedade da variável de tráfego (recomendamos):

      1. Propriedade nº 20 - Nome: Organização do Segmento RTP
      1. Propriedade nº 21 - Nome: RTP Segment Industry
      1. Propriedade nº 25 - Nome: Organização de Campanha
      1. Propriedade nº 26 - Nome: RTP Campaign Industry

      >[!NOTE]
      >
      >Se esses # forem usados, selecione outro número disponível. Alinhe esse número com o número do slot nas Configurações da conta RTP)

      1. Altere os 4 nomes de propriedade. Esse é o nome que aparecerá no Conjunto de relatórios.

   1. Selecione o campo Enabled para **Ativado**.

   1. Selecione o campo Relatórios de caminho para **Ativado**.

## Configurar na Personalização em tempo real (RTP) do Marketo {#set-up-in-marketo-real-time-personalization-rtp}

1. Na plataforma RTP, acesse **Configurações da conta**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Em **Configurações da conta**, clique em **Domínio**.
1. Em **Analytics, clique em** **Adobe Analytics**.
1. Girar **Ligado** as variáveis Conversão, Personalizado e Tráfego são alternada.
1. Atribuir as variáveis de conversão, evento e tráfego **números de slot** para corresponder aos números de slot criados no AA
1. Clique em **Salvar**.

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>Nossas configurações de slot recomendadas são
>
>**Variáveis de conversão**
>
>* Conversões personalizadas do setor - Slot 20
>* Conversões Personalizadas da Organização - Slot 21
>
>**Eventos personalizados**
>
>* Evento personalizado de campanha - Slot 20
>* Evento personalizado de segmento - Slot 21
>
>**Variáveis de tráfego**
>
>* Variável de tráfego da organização do segmento - Slot 20
>* Variável de tráfego do setor de segmento - Slot 21
>* Variável de tráfego da organização de campanha - Slot 22
>* Variável de tráfego do setor de campanha - Slot 23
>
>**Verifique se esses números de slot estão alinhados com os números de variáveis e eventos criados no AA.**

## Relatórios {#reports}

Crie relatórios aprimorados do SiteAdobe Analytics de acordo com os nomes da organização, os setores e os segmentos RTP e os dados de campanhas em tempo real.

Exemplos de relatórios e painéis personalizados no AA incluem:

* Desempenho por setor ou segmento definido (listas nomeadas baseadas em conta)
* Detalhamento do setor por desempenho de KPI
* Páginas exibidas por organização
* Desempenho do canal de marketing de acordo com Organização, Indústria, Segmentos

**-Exemplos de relatórios-**

**Relatório dos Principais Setores**

![](assets/top-industries-report.png)

**Relatório das organizações**

![](assets/image2014-11-29-12-3a29-3a42.png)

**Criação do painel de RTP**

Criar um [novo painel](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html), chamado **Painel RTP**. Esse painel ajudará a entender o detalhamento dos visitantes de acordo com os segmentos verticais e RTP.

1. Clique em **Painel,** click **Adicionar painel**.

1. Atribuir um nome ao painel **Painel RTP**.

1. Selecione o **tamanho do painel** 3 x 2, 2 x 2.

1. Crie o [reportlet](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) e adicionar [conteúdo para o painel](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard).

Adicionando o Reportlet de setores ao painel

1. Ir para **Conversões personalizadas**, clique em **Setor**.

1. Configurar gráfico para **Gráfico de Pizza**.

1. Clique em **Painel**, adicionar **Reportlet**.

1. Atribuir um nome ao relatório **Principais setores**.

1. Colocar no painel **Painel RTP**.

1. Criar **Novo**.

Adicionar o reportlet de segmentos ao painel

1. Ir para **Métricas do site**. Clique em **Eventos personalizados**, **Segmentos**.

1. Configurar gráfico para **Barra vertical**.

1. Clique em **Painel**, adicionar **Reportlet**.

1. Atribuir um nome ao relatório **Principais segmentos**.

1. Colocar no painel **Painel RTP**.

1. Criar **Novo**.

Seus reportlets serão exibidos no painel.

## Exibir impressões e cliques (conversões) no Adobe Analytics {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. Clique em **Links personalizados**.

   ![](assets/sitecatalyst1-1.png)

1. Procure por Impressões para visualizar os nomes de Segmento e Campanha que representam o número de impressões da campanha.\
   ![](assets/sitecatalyst1.png)

1. Procure por Conversão para visualizar os nomes de Segmento e Campanha que representam o número de cliques da campanha.

   ![](assets/sitecatalyst2.png)
