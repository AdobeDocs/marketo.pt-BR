---
unique-page-id: 4720796
description: Redirecionamento com dados do Web Personalization - Documentação do Marketo - Documentação do produto
title: Redirecionamento com dados da personalização da web
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 3%

---

# Redirecionamento com dados [!DNL Web Personalization] {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>O Redirecionamento de site agora se enquadra no bloco Web Personalization. Se você comprou apenas o Redirecionamento, verá este bloco e acessará o produto [!DNL Web Personalization] com **somente** recursos de Redirecionamento habilitados. Isso dá acesso às configurações da conta, à página de redirecionamento, aos segmentos e às páginas de rastreamento adicionais.

O remarketing direciona os clientes potenciais que visitaram seu site no passado com publicidade de exibição com base em quem eles são e no que fizeram. O redirecionamento personalizado segmenta públicos-alvo específicos com anúncios relevantes com base no setor, contas nomeadas e dados de pessoas conhecidas.

O Web Personalization atualmente anexa dados às seguintes plataformas de remarketing:

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

[!DNL Web Personalization] envia os seguintes dados através do para as plataformas de remarketing para criar públicos e executar campanhas de anúncios de remarketing:

<table>
 <tbody>
  <tr>
   <th colspan="1">[!DNL Web Personalization] Dados</th>
  </tr>
  <tr>
   <th><p>Setor</p></th>
  </tr>
  <tr>
   <th><p>Grupo (Enterprise, SMB)</p></th>
  </tr>
  <tr>
   <th><p>Categoria (Fortune 500/1000, Global 2000)</p></th>
  </tr>
  <tr>
   <th><p>Lista ABM (listas de contas nomeadas)</p></th>
  </tr>
  <tr>
   <th><p>Público segmentado (com base em segmentos)</p></th>
  </tr>
  <tr>
   <th><p>Campanhas da Web clicadas</p></th>
  </tr>
 </tbody>
</table>

## Configuração de remarketing {#remarketing-configuration}

1. Vá para **[!UICONTROL Redirecionamento]**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >A configuração de redirecionamento é por domínio ou subdomínio. Ative os outros domínios se desejar enviar dados desses domínios para a plataforma de redirecionamento.

1. Ativar Configurações para Google Analytics ou [!DNL Google Universal Analytics] por domínio.

   >[!NOTE]
   >
   >Você precisa ter a Tag de redirecionamento do Google implementada em seu site.
   >
   >Se você já configurou a Integração com o Web Personalization e o Google Analytics, não é necessário editar esta parte, pois é a mesma configuração em Configurações da conta.

   ![](assets/two.png)

1. Ative a configuração para o Facebook. Clique e expanda a opção [!DNL Facebook], Clique em **[!UICONTROL Ligado]** para enviar os respectivos eventos e dados para o Facebook Audience Manager. Clique em **[!UICONTROL Salvar]**.

   >[!NOTE]
   >
   >Você precisa ter o [[!DNL Facebook] Pixel de público-alvo personalizado](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) instalado em seu site para que este recurso funcione.

   ![](assets/three.png)

## Criação de público segmentado {#creating-segmented-audience}

Um público-alvo segmentado permite selecionar um segmento existente como um público-alvo para usar em campanhas de redirecionamento. Por exemplo, selecionando os segmentos Pessoa conhecida.

>[!TIP]
>
>Não há necessidade de criar um Público-alvo segmentado para dados do setor ou outros que já tenham sido enviados na Configuração de domínio. É melhor usar Públicos segmentados para segmentos com base em dados de pessoas conhecidas.

1. Clique em **[!UICONTROL Criar Público Segmentado]**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Insira o Nome do público-alvo, selecione Canais e selecione Segmento na lista de Segmentos existentes.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Clique em **[!UICONTROL Salvar]**.

   Você concluiu a Configuração de Redirecionamento em [!DNL Web Personalization], fez logon nas plataformas de redirecionamento e criou públicos-alvo com base nesses dados e configurou as campanhas de anúncios de redirecionamento.
