---
unique-page-id: 11383953
description: Configurar conversões offline do Facebook - Documentação do Marketo - Documentação do produto
title: Configurar conversões offline do Facebook
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 5%

---

# Configurar conversões offline do Facebook {#set-up-facebook-offline-conversions}

Ao enviar dados de conversão offline de volta para o Facebook para as pessoas criadas com anúncios de cliente potencial, sua equipe de publicidade pode otimizar seus gastos com anúncios melhor do que nunca. Veja como configurar isso.

>[!PREREQUISITES]
>
>* Você deve [Configurar anúncios de cliente potencial do Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* Você deve ter um modelo aprovado no [Modelador de ciclo de receita](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).

## Configuração de administração {#admin-configuration}

1. Ir para o Marketo **Admin**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Ir para **LaunchPoint** e clique duas vezes no serviço Facebook Lead Ads criado anteriormente.

   >[!NOTE]
   >
   >Se ainda não tiver feito isso, vá em frente e [Configurar Anúncios De Cliente Potencial Da Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md), então volte aqui.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Se desejar, edite o **Nome de exibição** para incluir conversões offline. Clique em **Próxima**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Marcar **Habilitar conversões offline** e clique em **Próxima**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Clique em **Próxima**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Clique em **Salvar**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   Doce! Você está na metade da habilitação de Conversões Offline do Facebook. Vamos passar para o Modelador de ciclo de receita para mapear os estágios.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Configuração do Modelador de Ciclo de Receita {#revenue-cycle-modeler-configuration}

1. Ir para **Analytics**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Selecione seu modelo e clique em **Editar rascunho**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >Atualmente, há 10 eventos do Facebook para os quais você pode mapear Estágios do ciclo de receita:
   >
   >* Adiciona às Informações de pagamento
   >* Adiciona ao Carrinho
   >* Adiciona à lista de desejos
   >* Registros concluídos
   >* Check-outs iniciados
   >* Pessoa
   >* Outro
   >* Adquirir
   >* Pesquisas
   >* Exibições de conteúdo

1. Selecione o estágio que deseja mapear e na **Conversão do facebook** selecione o Evento Facebook para o qual deseja mapeá-lo. Repita esta etapa para mapear todos os estágios no seu RCM para estágios de conversão offline no Facebook.

   ![](assets/1-1.png)

1. Quando terminar o mapeamento, feche o modelo.

   ![](assets/2.png)

1. Aprove seu modelo e pronto!

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   Agora, quando os leads de anúncio de lead atingem os estágios mapeados, as conversões são enviadas ao Facebook para relatórios.

   >[!CAUTION]
   >
   >Verifique sua conta da Facebook e certifique-se de que [anúncios estão associados](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) para o Conjunto de eventos de conversões offline do Marketo. Se não estiverem, a atribuição de anúncio pode não funcionar.

   >[!NOTE]
   >
   >Os dados de conversão offline são enviados do Marketo para o Facebook várias vezes diariamente.

>[!MORELIKETHIS]
>
>[Noções básicas sobre conversões offline do Facebook](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
