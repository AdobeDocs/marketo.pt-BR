---
unique-page-id: 4720125
description: Integração do RTP ao Google Universal Analytics - Documentação do Marketo - Documentação do produto
title: Integrar o RTP ao Google Universal Analytics
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 2%

---

# Integrar o RTP ao Google Universal Analytics {#integrate-rtp-with-google-universal-analytics}

## Introdução {#intro}

Aproveite o Google Universal Analytics (GUA) com dados firmográficos e de personalização do Marketo Real-Time Personalization (RTP) para medir e analisar melhor suas iniciativas de marketing online.

Esta publicação explica como configurar e integrar a plataforma Marketo Real-Time Personalization (RTP) às contas do Google Universal Analytics (GUA). Os dados RTP podem ser anexados à sua conta GUA, permitindo que você visualize e veja o desempenho de organizações, setores, firmográficos e segmentos RTP que visitam seu site.

**Análises universais do Google**

O Google Universal Analytics com dados da RTP fornece uma melhor compreensão de como os usuários B2B interagem com seu conteúdo online e ajuda a medir e obter melhores resultados de suas campanhas de personalização. [Leia mais sobre o Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**Somente para usuários do Google Tag Manager**
>
>Nenhuma codificação ou configuração especial precisa ser feita. Certifique-se de concluir a seguinte lista de verificação:
>
>* As dimensões RTP são criadas no Google Universal Analytics
>* [A tag RTP está instalada corretamente no Google Tag Manager](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* A Integração do Google Universal Analytics está habilitada nas Configurações de conta do RTP
>* [A tag do Google Universal Analytics está configurada corretamente no Google Tag Manager](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [A tag do Google Tag Manager está instalada corretamente no site](https://developers.google.com/tag-manager/quickstart)

## Configurar Dimension personalizados no GUA {#set-up-custom-dimensions-in-gua}

1. Em Google Analytics,

   1. Ir para **Admin**
   1. Selecione o **Conta.**
   1. Selecione o **Propriedade.**
   1. Selecionar **Definições Personalizadas** e **Dimension personalizado**.
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Adicione uma nova dimensão personalizada. Clique em **+Novo Dimension personalizado**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Adicione o seguinte **Dimension personalizados:**

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
   <td><p align="center">✓ µ</p></td> 
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
>**Nomes de Dimension personalizados** deve ser exatamente como definido na tabela acima (caso contrário, os painéis e relatórios personalizados de RTP no GUA não serão exibidos corretamente)

1. Adicione o **Nome**. Selecione o Escopo como **Session**. Clique em **Criar**.

   ![](assets/image2014-11-29-11-3a12-3a51.png)

Sua lista de Dimension personalizados deve ficar assim.

![](assets/image2014-11-29-11-36-50-version-2.png)

Depois de ativar os Dimension personalizados no GUA, acesse a plataforma RTP para ativar essas dimensões no RTP.

## Ativar a integração GUA na sua conta RTP {#activate-the-gua-integration-in-your-rtp-account}

1. Na plataforma RTP, acesse **Configurações da conta.**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Em **Configurações da conta**, clique em **Domínio**.
1. Em **Analytics**, clique em **Google Universal Analytics**.
1. Girar **Ligado** Use os Dimension e Eventos personalizados relevantes para anexar esses dados da RTP ao Google Universal Analytics.
1. Insira o **Número do índice** da dimensão alinhada com o número de índice no GUA.
1. Clique em **Salvar**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>O número de índice do Dimension personalizado pode ser encontrado no GUA em Dimension personalizados.
>
>Exemplo: Número do Índice RTP-Setor é igual a 1, Número do Índice RTP-Organização é igual a 2.

## Remover painéis antigos no Google Analytics {#remove-old-dashboards-in-google-analytics}

1. Em Google Analytics. Ir para **Relatórios.**
1. Clique em **Painéis.**
1. Selecione um **Painel** (Desempenho RTP B2B ou RTP)
1. Clique em **Excluir painel**.

![](assets/image2014-11-29-11-3a42-3a55.png)
