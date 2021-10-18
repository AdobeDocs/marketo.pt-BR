---
unique-page-id: 11383953
description: Configurar conversões offline do Facebook - Documentos do Marketo - Documentação do produto
title: Configurar conversões offline do Facebook
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 5%

---

# Configurar conversões offline do Facebook {#set-up-facebook-offline-conversions}

Ao enviar dados de conversão offline de volta para a Facebook para pessoas criadas com leads, sua equipe de publicidade pode otimizar melhor do que nunca o gasto com seus anúncios. Veja como configurar.

>[!PREREQUISITES]
>
>* Você deve [configurar Anúncios de leads do Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* Você deve ter um modelo aprovado em [Modelador do ciclo de receita](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).


## Configuração do administrador {#admin-configuration}

1. Ir para o Marketo **Administrador**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Ir para **LaunchPoint** e clique duas vezes no serviço Anúncios de leads da Facebook criado anteriormente.

   >[!NOTE]
   >
   >Se você não fez isso, vá em frente e [Configurar anúncios de lead da Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)E então volte aqui.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Se desejar, edite a variável **Nome de exibição** para incluir Conversões offline. Clique em **Próximo**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Verificar **Ativar conversões offline** e clique em **Próximo**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Clique em **Próximo**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Clique em **Salvar**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   Doce! Você já terminou a metade de ativar as Conversões offline do Facebook. Vamos saltar para o Modelador do Ciclo de Receita para mapear os estágios.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Configuração do Modelador do Ciclo de Receita {#revenue-cycle-modeler-configuration}

1. Ir para **Analytics**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Selecione o modelo e clique em **Editar rascunho**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >Atualmente, há 10 eventos do Facebook que você pode mapear Estágios do Ciclo de Receita para:
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


1. Selecione o palco que deseja mapear e, em seguida, selecione o **Conversão do facebook** selecione o Evento do Facebook para o qual deseja mapeá-lo. Repita esta etapa para mapear todos os estágios no RCM para estágios de conversão offline no Facebook.

   ![](assets/1-1.png)

1. Quando terminar de mapear, feche o modelo.

   ![](assets/2.png)

1. Aprove seu modelo e você terminou!

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   Agora, quando os leads de anúncios atingem os estágios mapeados, as conversões são enviadas ao Facebook para relatórios.

   >[!CAUTION]
   >
   >Verifique sua conta do Facebook e garanta que todas as [anúncios são associados](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) para o Conjunto de Eventos de Conversões Offline do Marketo. Caso contrário, a atribuição pode não funcionar.

   >[!NOTE]
   >
   >Os dados de conversão offline são enviados do Marketo para o Facebook várias vezes ao dia.

>[!MORELIKETHIS]
>
>[Noções básicas sobre conversões offline do Facebook](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
