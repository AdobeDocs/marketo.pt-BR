---
unique-page-id: 2949160
description: Integrar à Adobe Analytics - Documentos do Marketing Cloud - Documentação do produto
title: Integrar ao Adobe Analytics
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---


# Integrar ao Adobe Analytics {#integrate-with-adobe-analytics}

## Introdução {#intro}

Analise suas análises da Web de uma perspectiva B2B, visualizando dados de campanha de organização, setor e Marketing Real-Time Personalization (RTP) em sua conta da Adobe Analytics.

Este documento permite a integração entre a RTP (Marketo Real-Time Personalization, personalização em tempo real) e a Adobe Analytics Adobe. Os dados do RTP permitirão que você detecte e analise tendências em todos os segmentos do setor e organizações que visitam seu site e avalie a eficácia das campanhas RTP, fornecendo insights e análises para obter resultados ideais.

Você pode fazer isso observando métricas como o número de visitantes novos e recorrentes em cada segmento, analisando as taxas de cliques no campanha e descobrindo quais setores, segmentos personalizados e campanhas em tempo real geraram as melhores oportunidades de conversão. Aproveite essa capacidade para obter o máximo benefício de sua conta RTP.

## AUDIENCE ANALYTICS RTP {#rtp-audience-analytics}

Com a integração RTP - AA, você tem uma nova dimensão na interface do Web Analytics. O RTP aprimora automaticamente seus painéis de análise da Web com:

1. Dados da organização e do setor
1. Segmentos RTP personalizados
1. Listas de conta nomeadas (Marketing baseado em conta)

Isso aprimora seus dados B2B e permite que você se concentre em visitantes relevantes ao otimizar:

1. Canais de saída
1. Conteúdo
1. Redefinição de metas

## Relatório de canal {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

O painel RTP ajuda você a entender o detalhamento dos visitantes de acordo com segmentos verticais e RTP. Você pode ver o desempenho do seu visitante de acordo com a indústria e diferentes campanhas de marketing (pagas, orgânicas, sociais) relacionadas a essa indústria. O painel também fornece uma visão geral de alto nível das seções do site que seus visitantes estão visualizando de acordo com o tipo do setor.

## Relatório comportamental {#behavioral-report}

Relatórios de comportamento diferentes podem ser criados no Adobe Analytics com base em dados de organização, setor e segmento RTP. Esses Relatórios de fluxo visualizam o caminho que os visitantes levam de uma Página ou Evento para a seguinte. Este relatório pode ajudá-lo a descobrir qual conteúdo mantém os visitantes envolvidos no site.

## Desempenho RTP {#rtp-performance}

Impressões e conversões de campanha RTP de visualização em Links personalizados no Adobe Analytics.

Este relatório de Link personalizado mostrará impressões e conversões de campanhas no seguinte formato de nomeação:

* Impressão ISegment: [Nome do segmento RTP], ICampaign: [Nome da Campanha RTP]
* ISegment de conversão: [Nome do segmento RTP], ICampaign: [Nome da Campanha RTP]

![](assets/custom-links-report.png)

## Configurar no Adobe Analytics {#set-up-in-adobe-analytics}

A integração usa a API JavaScript que a Adobe Analytics oferta. As variáveis de conversão personalizadas (eVar), eventos personalizados (evento) e variáveis de tráfego são usadas na integração. Todos devem ser habilitados de dentro do administrador AA. Você deve definir as variáveis de conversão, os eventos personalizados e as variáveis de tráfego no AAou não poderá ver os dados no conjunto mesmo se você os ativou no RTP.

Complete as etapas a seguir para configurar essas variáveis no AA:

1. Vá para **Ferramentas administrativas** na sua conta AA.
1. Selecione o **Conjunto de relatórios** a ser usado com a integração.
1. Em **Editar configurações,** vá para **Conversão** e selecione ** [Variáveis de conversão](http://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**.\
   Selecione o número [Variável de conversão](http://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) (recomendamos):

   1. 

      1. Evar nº 20 para conversões personalizadas do setor
      1. Evar nº 21 para conversões personalizadas da organização

         >[!NOTE]
         >
         >Se esses números forem tomados, selecione outro número disponível. Alinhe esse número com o número do slot nas Configurações da conta RTP.

      1. Alterar status para* ativado*

         1. Altere o Nome para **Setor** e **Organização**. (É assim que será exibido no Conjunto de relatórios.)

         1. Altere o campo Expirar após para **Visita.**

1. Em **Editar configurações **vá para** Conversão **e selecione ** [Eventos bem-sucedidos](http://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**.

1. Selecione o número do Evento Eventos de sucesso personalizados (recomendamos):

   1. evento20 para Campanhas RTP
   1. evento21 para segmentos RTP

      >[!NOTE]
      >
      >Se esses números forem tomados, selecione outro número disponível. Alinhe esse número com o número do slot nas Configurações da conta RTP.

   1. Altere os nomes dos dois eventos para **Campanhas RTP** e **Segmentos RTP**. Esse é o nome que será exibido no Conjunto de relatórios.

1. Selecione o campo Tipo* *para ser **Contador (sem sub-relações)**

1. Em **Editar configurações** vá para ** [Tráfego](http://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable) **e selecione ** [Variáveis de tráfego](http://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**.

   1. Selecione a propriedade da variável de tráfego # (recomendamos):

      1. Propriedade # 20 - Nome: Organização do segmento RTP
      1. Propriedade # 21 - Nome: Setor do segmento RTP
      1. Propriedade # 25 - Nome: Organização de campanhas
      1. Propriedade # 26 - Nome: Indústria de Campanha RTP

         >[!NOTE]
         >
         >Se esses números forem tomados, selecione outro número disponível. Alinhe esse número com o número do slot nas Configurações da conta RTP)

      1. Altere os nomes das propriedades 4. Esse é o nome que será exibido no Conjunto de relatórios.
   1. Selecionar campo Ativado para **Ativado**
   1. Selecione o campo Relatórios de caminho para **Ativado**


## Configurar no Marcador para personalização em tempo real (RTP) {#set-up-in-marketo-real-time-personalization-rtp}

1. Na plataforma RTP, vá para **Configurações da conta**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Em **Configurações da conta**, clique em **Domínio**.
1. Em **Analytics, clique em** **Adobe Analytics**.
1. Ative **On **as variáveis Conversão, Personalizado e Tráfego alternam.
1. Atribua as Variáveis de conversão, Evento e tráfego **números de slot** para corresponder aos números de slot criados em AA
1. Clique em **SALVAR**.

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>Nossas configurações de slot recomendadas são
>
>**Variáveis de conversão**
>
>* Conversões personalizadas do setor - Slot 20
>* Conversões personalizadas da organização - Slot 21

>
>
**Eventos personalizados**
>
>* Evento personalizado de campanha - Slot 20
>* Evento personalizado do segmento - Slot 21

>
>
**Variáveis de tráfego**
>
>* Variável de tráfego da organização do segmento - Slot 20
>* Variável de tráfego do setor de segmentos - Slot 21
>* Variável de tráfego da organização da campanha - Slot 22
>* Variável de tráfego da indústria de campanhas - Slot 23

>
>
**Certifique-se de que esses números de slot estejam alinhados com os números de variáveis e eventos criados em AA.**

## Relatórios {#reports}

Crie relatórios aprimorados do SiteAdobe Analytics de acordo com nomes de organizações, setores e segmentos RTP e dados de campanhas em tempo real.

Exemplos de relatórios e painéis personalizados em AA incluem:

* Desempenho por setor ou segmento definido (listas nomeadas baseadas em conta)
* Detalhamento do setor por desempenho de KPI
* Páginas visualizadas por organização
* Desempenho do canal de marketing de acordo com Organização, Setor, Segmentos

**Exemplos de relatórios**

**Relatório dos principais setores**

** ![](assets/top-industries-report.png)

**

**Relatório de organizações**

![](assets/image2014-11-29-12-3a29-3a42.png)

**Criação do Painel RTP**

Crie um [novo painel](http://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html), chamado **Painel RTP**. Esse painel ajudará a entender o detalhamento dos visitantes de acordo com segmentos verticais e RTP.

1. Clique em **Painel,** clique em** Adicionar Painel**

1. Nomeie o Painel **Painel RTP**
1. Selecione **tamanho do painel** 3 x 2, 2 x 2
1. Crie o [reportlet](http://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) e adicione [conteúdo ao painel](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard)

Adicionando o reportlet Setores ao Painel

1. Vá para **Conversões personalizadas**, clique em **Setor**

1. Configurar gráfico para **Gráfico de pizza**
1. Clique em **Painel**, adicione **Reportlet**

1. Nomeie o relatório **Principais setores**
1. Local no Painel **Painel RTP**
1. Crie **Novo**.

Adicionar o reportlet Segmentos ao Painel

1. Ir para **Métricas do site, **Clique em **Eventos personalizados, segmentos**

1. Configurar gráfico para **barra vertical**
1. Clique em **Painel**, adicione **Reportlet**

1. Nomeie o relatório **Principais segmentos**
1. Local no Painel **Painel RTP**
1. Criar **Novo.**

Seus reportlets serão exibidos no painel.

## Impressões e cliques de visualização (conversões) no Adobe Analytics {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. Clique em Links personalizados.

   ![](assets/sitecatalyst1-1.png)

1. Procure por impressões para nomes de segmentos de visualização e Campanhas que representem o número de impressões da campanha.\
   ![](assets/sitecatalyst1.png)

1. Procure Conversão para Segmentos de visualização e nomes de Campanha que representam o número de cliques para a campanha.

   ![](assets/sitecatalyst2.png)

