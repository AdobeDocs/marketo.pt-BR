---
unique-page-id: 4720125
description: Integrar RTP ao Google Universal Analytics - Documentos do Marketing - Documentação do produto
title: Integrar RTP ao Google Universal Analytics
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# Integrar RTP ao Google Universal Analytics {#integrate-rtp-with-google-universal-analytics}

## Introdução {#intro}

Aproveite o Google Universal Analytics (GUA) com os dados firmmográficos e de personalização RTP (Real-Time Personalization, personalização em tempo real) da Marketo para medir e analisar melhor seus esforços de marketing online.

Esta postagem explica como configurar e integrar a plataforma Marcketo Real-Time Personalization (RTP) com contas do Google Universal Analytics (GUA). Os dados RTP podem ser anexados à sua conta GUA, permitindo que você visualização e veja o desempenho de organizações, setores, firmográficos e segmentos RTP que visitam seu site.

**Google Universal Analytics**

O Google Universal Analytics com os dados RTP fornece uma melhor compreensão de como os usuários B2B interagem com seu conteúdo online e ajudam a medir e obter melhores resultados de suas campanhas de personalização. [Leia mais sobre o Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**`For Google Tag Manager Users Only`**
>
>Não é necessário fazer a codificação ou configuração especial. Certifique-se de concluir a seguinte lista de verificação:
>
>* `RTP dimensions are created in Google Universal Analytics`
>* [A tag RTP está instalada corretamente no Google Tag Manager](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* `Google Universal Analytics Integration is enabled in the RTP's Account Settings`
>* [A tag do Google Universal Analytics está configurada corretamente no Google Tag Manager](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [A tag do Google Tag Manager está instalada corretamente no seu site](https://developers.google.com/tag-manager/quickstart)

>



## Configurar Dimension personalizados no GUA {#set-up-custom-dimensions-in-gua}

1. Em Google Analytics,

   1. Ir para **Administrador**
   1. Selecione a **Conta.**
   1. Selecione a **Propriedade.**
   1. Selecione **Definições personalizadas **e Dimension **personalizados.**

      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. Adicione uma nova dimensão personalizada. Clique em **+Novo Dimension personalizado**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. Adicione os seguintes Dimension **personalizados:**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>Nome do Dimension personalizado</strong></p></td> 
   <td><p><strong>Âmbito</strong></p></td> 
   <td><p><strong>Ativo</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Organização</strong></p></td> 
   <td><p>Sessão</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP-Indústria</strong></p></td> 
   <td><p>Sessão</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>CATEGORIA RTP</strong></p></td> 
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
>**Os Nomes** de Dimension personalizados devem ser exatamente como definidos na tabela acima (caso contrário, painéis e relatórios RTP personalizados no GUA não serão exibidos corretamente)

1. Adicione o **Nome. **Selecione o Escopo como **Sessão.** Clique em **Criar.**

   ![](assets/image2014-11-29-11-3a12-3a51.png)

Sua lista Dimension personalizada deve ser parecida com esta.

![](assets/image2014-11-29-11-36-50-version-2.png)

Depois de ativar os Dimension personalizados no GUA, vá para a plataforma RTP para ativar essas dimensões no RTP.

## Ativar a integração GUA na sua conta RTP {#activate-the-gua-integration-in-your-rtp-account}

1. Na plataforma RTP, vá para Configurações da **conta.**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Em Configurações **da** conta, clique em **Domínio.**
1. Em **Analytics, **clique em **Google Universal Analytics**.
1. Ative **** os Dimension personalizados e Eventos relevantes para anexar esses dados do RTP ao Google Universal Analytics.
1. Informe o número **do** Índice da dimensão alinhado com o número do índice no GUA.
1. Clique em **Salvar**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>O Número de índice do Dimension personalizado pode ser encontrado no GUA em Dimension personalizados.
>
>Exemplo: Número de índice RTP-Indústria igual a 1, Número de índice RTP-Organização igual a 2.

## Remover Painéis antigos em Google Analytics {#remove-old-dashboards-in-google-analytics}

1. Em Google Analytics. Vá ao **Relatórios.**
1. Clique em **Painéis.**
1. Selecione um **Painel **(Desempenho RTP B2B ou RTP)
1. Clique em **Excluir Painel**.

![](assets/image2014-11-29-11-3a42-3a55.png)

