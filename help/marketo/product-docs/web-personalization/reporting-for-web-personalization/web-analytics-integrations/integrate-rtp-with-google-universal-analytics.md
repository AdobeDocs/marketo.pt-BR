---
unique-page-id: 4720125
description: Integração do RTP ao Google Universal Analytics - Documentação do Marketo - Documentação do produto
title: Integrar o RTP ao Google Universal Analytics
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 3%

---

# Integrar RTP com [!DNL Google Universal Analytics] {#integrate-rtp-with-google-universal-analytics}

## Introdução {#intro}

Aproveite o [!DNL Google Universal Analytics] (GUA) com os dados firmográficos e de personalização (RTP) do [!DNL Marketo Real-Time Personalization] para medir e analisar melhor suas iniciativas de marketing online.

Esta publicação explica como configurar e integrar a plataforma [!DNL Marketo Real-Time Personalization] (RTP) com contas [!DNL Google Universal Analytics] (GUA). Os dados RTP podem ser anexados à sua conta GUA, permitindo que você visualize e veja o desempenho de organizações, setores, firmográficos e segmentos RTP que visitam seu site.

**[!DNL Google Universal Analytics]**

O [!DNL Google Universal Analytics] com dados da RTP fornece uma melhor compreensão de como os usuários B2B interagem com seu conteúdo online e ajuda a medir e obter melhores resultados de suas campanhas de personalização. [Leia mais sobre [!DNL Google Universal Analytics]](https://support.google.com/analytics/answer/2790010/?hl=en&authuser=1).

>[!NOTE]
>
>**Somente Para Usuários Do Google Tag Manager**
>
>Nenhuma codificação ou configuração especial precisa ser feita. Certifique-se de concluir a seguinte lista de verificação:
>
>* Dimensões RTP são criadas em [!DNL Google Universal Analytics]
>* [A marca RTP está instalada corretamente no Gerenciador de Marcas do Google](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* A integração [!DNL Google Universal Analytics] está habilitada nas Configurações de Conta do RTP
>* A [[!DNL Google Universal Analytics] tag está configurada corretamente no Gerenciador de Tags da Google](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [A marca do Google Tag Manager está instalada corretamente em seu site](https://developers.google.com/tag-manager/quickstart)

## Configurar dimensões personalizadas no GUA {#set-up-custom-dimensions-in-gua}

1. No Google Analytics,

   1. Ir para **[!UICONTROL Administrador]**
   1. Selecione a **[!UICONTROL Conta].**
   1. Selecione a **[!UICONTROL Propriedade].**
   1. Selecione **[!UICONTROL Definições personalizadas]** e **[!UICONTROL Dimensões personalizadas]**.

      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Adicione uma nova dimensão personalizada. Clique em **[!UICONTROL +Nova Dimension Personalizada]**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Adicionar as seguintes **[!UICONTROL Dimensões Personalizadas]:**

<table>
 <tbody>
  <tr>
   <td><p><strong>Nome Dimension personalizado</strong></p></td>
   <td><p><strong>Escopo</strong></p></td>
   <td><p><strong>Ativo</strong></p></td>
  </tr>
  <tr>
   <td><p><strong>RTP-Organização</strong></p></td>
   <td><p>Sessão</p></td>
   <td><p align="center">✓</p></td>
  </tr>
  <tr>
   <td><p><strong>RTP-Setor</strong></p></td>
   <td><p>Sessão</p></td>
   <td><p align="center">✓</p></td>
  </tr>
  <tr>
   <td><p><strong>RTP-Categoria</strong></p></td>
   <td><p>Sessão</p></td>
   <td><p align="center">✓</p></td>
  </tr>
  <tr>
   <td><p><strong>RTP-Group</strong></p></td>
   <td><p>Sessão</p></td>
   <td><p align="center">✓</p></td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>**Nomes personalizados de Dimension** devem ser exatamente como definidos na tabela acima (caso contrário, os painéis e relatórios personalizados de RTP no GUA não serão exibidos corretamente)

1. Adicione o **[!UICONTROL Nome]**. Selecione o Escopo como **[!UICONTROL Sessão]**. Clique em **[!UICONTROL Criar]**.

   ![](assets/image2014-11-29-11-3a12-3a51.png)

Sua lista Dimension personalizado deve ficar assim.

![](assets/image2014-11-29-11-36-50-version-2.png)

Depois de ativar as Dimensões personalizadas no GUA, acesse a plataforma RTP para ativar essas dimensões no RTP.

## Ativar a integração GUA na sua conta RTP {#activate-the-gua-integration-in-your-rtp-account}

1. Na plataforma RTP, vá para **[!UICONTROL Configurações da Conta].**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Em **[!UICONTROL Configurações de conta]**, clique em **[!UICONTROL Domínio]**.
1. Em **[!UICONTROL Analytics]**, clique em **[!UICONTROL Google Universal Analytics]**.
1. Ative **[!UICONTROL o]** as Dimensões e Eventos Personalizados relevantes para anexar esses dados do RTP a [!DNL Google Universal Analytics].
1. Insira o **[!UICONTROL Número do índice]** da dimensão alinhada com o número do índice em GUA.
1. Clique em **[!UICONTROL Salvar]**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>O número de índice do Dimension personalizado pode ser encontrado no GUA em Dimensões personalizadas.
>
>Exemplo: Número do Índice RTP-Setor é igual a 1, Número do Índice RTP-Organização é igual a 2.

## Remover painéis antigos no Google Analytics {#remove-old-dashboards-in-google-analytics}

1. No Google Analytics. Ir para **[!UICONTROL Relatórios].**
1. Clique em **[!UICONTROL Painéis].**
1. Selecione um **[!UICONTROL Painel]** (RTP B2B ou Desempenho RTP)
1. Clique em **[!UICONTROL Excluir Painel]**.

![](assets/image2014-11-29-11-3a42-3a55.png)
