---
unique-page-id: 2360354
description: Adicionar o código de rastreamento do Munchkin ao seu site - Documentos do Marketo - Documentação do produto
title: Adicionar o código de rastreamento do Munchkin ao seu site
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Adicionar o código de rastreamento do Munchkin ao seu site {#add-munchkin-tracking-code-to-your-website}

O código de rastreamento personalizado JavaScript do Marketo, chamado Munchkin, rastreia todos os indivíduos que visitam seu site para que você possa reagir às visitas com campanhas de marketing automatizadas. Até mesmo visitantes anônimos são rastreados junto com seus endereços IP e outras informações. **Sem esse código de rastreamento, você não poderá rastrear visitas ou outras atividades no seu site**!

>[!PREREQUISITES]
>
>Certifique-se de ter acesso a um desenvolvedor JavaScript experiente. O Suporte técnico da Marketo não está configurado para ajudar na solução de problemas do JavaScript personalizado.

## Adicionar código de rastreamento ao seu site {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Os clientes do Adobe Experience Cloud também podem usar a integração do Marketo no Adobe Launch para incluir o script do Munchkin em suas páginas da Web. Obtenha o aplicativo [aqui](https://www.adobeexchange.com/experiencecloud.details.101054.html).

1. Vá para **Admin** e clique em **Munchkin** na árvore à esquerda.

   ![](assets/image2015-8-25-16-3a21-3a14.png)

   Selecione Assíncrono para Tipo de código de rastreamento.

   ![](assets/image2015-8-25-16-3a24-3a33.png)

   >[!NOTE]
   >
   >Em quase todos os casos, você deve usar o código assíncrono. [Saiba mais.](#types-of-munchkin-tracking-codes)

   Clique em e copie o código de rastreamento do Javascript a ser colocado no seu site.

   ![](assets/image2015-8-25-16-3a26-3a12.png)

   >[!CAUTION]
   >
   >Não use o código mostrado nesta captura de tela - você deve usar o código exclusivo que aparece em sua conta!

   >[!TIP]
   >
   >Coloque o código de rastreamento nas páginas da Web que deseja rastrear. Isso pode ser em todas as páginas para sites menores ou somente páginas-chave em sites que tenham muitas páginas da Web geradas dinamicamente, fóruns de usuários, e assim por diante.

   Para obter melhores resultados, use o código do Munchkin assíncrono e coloque-o dentro dos elementos `<head>` de suas páginas. Se você estiver usando o código simples (não recomendado), isso é antes da tag `</body>` .
   ![](assets/image2015-8-25-16-3a5-3a20.png)

>[!TIP]
>
>Para sites que visualizam um alto volume de tráfego (ou seja, centenas de milhares de visitas por mês), recomendamos que você opte por não rastrear pessoas anônimas. [Saiba mais](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/).

## Adicionar código de rastreamento ao usar vários espaços de trabalho {#add-tracking-code-when-using-multiple-workspaces}

Se estiver usando Espaços de trabalho na sua conta do Marketo, provavelmente também terá presenças da Web separadas que correspondem aos seus espaços de trabalho. Nesse caso, você pode usar o Javascript de rastreamento do Munchkin para atribuir suas pessoas anônimas ao espaço de trabalho e partição corretos.

1. Vá para **Admin** e clique em **Munchkin** na árvore à esquerda.

![](assets/image2015-8-25-16-3a28-3a41.png)

1. Selecione o espaço de trabalho apropriado para as páginas da Web que você deseja rastrear.

   ![](assets/image2015-8-25-16-3a30-3a32.png)

>[!NOTE]
>
>Se você não usar o código do espaço de trabalho especial Munchkin, as pessoas serão atribuídas à partição padrão que foi criada quando sua conta foi configurada. Ela é chamada de &quot;Padrão&quot; inicialmente, mas você pode ter alterado isso em sua conta do Marketo.

1. Selecione **Assíncrono** para Tipo de código de rastreamento.

   ![](assets/image2015-8-25-16-3a32-3a42.png)

1. Clique em e copie o código de rastreamento do JavaScript para colocar em seu site.

   ![](assets/image2015-8-25-16-3a34-3a7.png)

   >[!CAUTION]
   >
   >Não use o código mostrado nesta captura de tela - você deve usar o código exclusivo que aparece em sua conta!

1. Coloque o código de rastreamento em suas páginas da Web no elemento `<head>` . Novas pessoas que visitarem esta página serão atribuídas a esta partição.

   ![](assets/image2015-8-25-16-3a5-3a20.png)

>[!CAUTION]
>
>Você só pode usar um script de rastreamento Munchkin para uma única partição e espaço de trabalho em uma página. Não inclua scripts de rastreamento para várias partições/espaços de trabalho no site.

>[!NOTE]
>
>As landing pages criadas no Marketo contêm automaticamente o código de rastreamento, de modo que não é necessário colocar esse código nelas.

## Tipos de códigos de rastreamento do Munchkin {#types-of-munchkin-tracking-codes}

Há três tipos de códigos de rastreamento do Munchkin que você pode escolher. Cada um afeta o tempo de carregamento da página da Web de forma diferente.

1. **Simples**: O tem menos linhas de código, mas não otimiza para o tempo de carregamento da página da Web. Este código carrega a biblioteca jQuery cada vez que uma página da Web é carregada.
1. **Assíncrono**: reduz o tempo de carregamento da página da Web.
1. **jQuery** assíncrona: reduz o tempo de carregamento da página da Web e também melhora o desempenho do sistema. Esse código pressupõe que você já tenha um jQuery e não verifica para carregá-lo.

## Teste se o código do Munchkin está funcionando {#test-if-your-munchkin-code-is-working}

Para verificar se o código do Munchkin está funcionando depois de adicioná-lo:

1. Visite sua página da Web.

1. Vá para **Analytics**.

   ![](assets/mainnav-analytics-hand.png)

1. Clique em **Atividade da página da Web**.

   ![](assets/webanalytics.png)

1. Clique na guia **Setup**, clique duas vezes em **Activity Source** e altere para **Anonymous Visitors (incluindo ISPs)**.

   ![](assets/analytics-activity-source.png)

   ![](assets/activitysource.png)

1. Clique na guia **Relatório**. Se não vir nenhum dado, espere alguns minutos e clique no ícone de atualização na parte inferior.
