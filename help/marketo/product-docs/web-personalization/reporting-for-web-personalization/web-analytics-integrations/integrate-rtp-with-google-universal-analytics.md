---
unique-page-id: 4720125
description: Integrar RTP ao Google Universal Analytics - Documentos do Marketo - Documentação do produto
title: Integrar RTP ao Google Universal Analytics
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 2%

---

# Integrar RTP ao Google Universal Analytics {#integrate-rtp-with-google-universal-analytics}

## Introdução {#intro}

Aproveite o Google Universal Analytics (GUA) com os dados firmmográficos e de personalização da Personalização em tempo real (RTP) da Marketo para medir e analisar melhor seus esforços de marketing online.

Esta publicação explica como configurar e integrar a plataforma Marketo Real-Time Personalization (RTP) com as contas do Google Universal Analytics (GUA). Os dados da RTP podem ser anexados a sua conta GUA, permitindo que você visualize e veja o desempenho de organizações, setores, firmográficos e segmentos RTP em visitas ao seu site.

**Análises universais do Google**

O Google Universal Analytics com dados da RTP oferece uma melhor compreensão de como os usuários B2B interagem com seu conteúdo online e ajudam a medir e obter melhores resultados de suas campanhas de personalização. [Leia mais sobre o Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**Somente para usuários do Gerenciador de tags da Google**
>
>Nenhuma codificação ou configuração especial precisa ser feita. Preencha a seguinte lista de verificação:
>
>* As dimensões RTP são criadas no Google Universal Analytics
>* [A tag RTP está instalada corretamente no Google Tag Manager](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* A integração do Google Universal Analytics está habilitada nas Configurações da conta da RTP
>* [A tag do Google Universal Analytics está configurada corretamente no Google Tag Manager](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [A tag do Google Tag Manager está instalada corretamente no seu site](https://developers.google.com/tag-manager/quickstart)


## Configurar Dimension personalizados no GUA {#set-up-custom-dimensions-in-gua}

1. No Google Analytics,

   1. Ir para **Administrador**
   1. Selecione o **Conta.**
   1. Selecione o **Propriedade.**
   1. Selecionar **Definições personalizadas** e **Dimension personalizados**.
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Adicione uma nova dimensão personalizada. Clique em **+Novo Dimension personalizado**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Adicione o seguinte **Dimension personalizado:**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>Nome do Dimension personalizado</strong></p></td> 
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
   <td><p><strong>Grupo RTP</strong></p></td> 
   <td><p>Sessão</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Nomes de Dimension personalizados** deve ser exatamente como definido na tabela acima (caso contrário, os painéis e relatórios RTP personalizados no GUA não serão exibidos corretamente)

1. Adicione o **Nome**. Selecione o Escopo como **Sessão**. Clique em **Criar**.

   ![](assets/image2014-11-29-11-3a12-3a51.png)

Sua lista Dimension personalizada deve ser semelhante a esta.

![](assets/image2014-11-29-11-36-50-version-2.png)

Depois de ativar o Dimension personalizado no GUA, vá para a plataforma RTP para ativar essas dimensões no RTP.

## Ativar a integração do GUA em sua conta RTP {#activate-the-gua-integration-in-your-rtp-account}

1. Na plataforma RTP, acesse **Configurações da conta.**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Em **Configurações da conta**, clique em **Domínio**.
1. Em **Analytics**, clique em **Google Universal Analytics**.
1. Turn **Ligado** as Dimension e eventos personalizados relevantes para anexar esses dados da RTP ao Google Universal Analytics.
1. Insira o **Número do índice** da dimensão alinhada ao número de índice no GUA.
1. Clique em **Salvar**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>O Número do índice do Dimension personalizado pode ser encontrado no GUA em Dimension personalizados.
>
>Exemplo: Número do Índice RTP-Setor igual a 1, Número do Índice RTP-Organização igual a 2.

## Remover Painéis Antigos em Google Analytics {#remove-old-dashboards-in-google-analytics}

1. No Google Analytics. Ir para **Relatório.**
1. Clique em **Painéis.**
1. Selecione um **Painel** (Desempenho RTP B2B ou RTP)
1. Clique em **Excluir painel**.

![](assets/image2014-11-29-11-3a42-3a55.png)
