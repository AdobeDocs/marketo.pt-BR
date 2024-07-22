---
unique-page-id: 11383945
description: Noções básicas sobre conversões offline do Facebook - Documentação do Marketo - Documentação do produto
title: Noções básicas sobre conversões offline do Facebook
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# Noções básicas sobre conversões offline do Facebook {#understanding-facebook-offline-conversions}

As campanhas de anúncios de clientes potenciais da facebook geram clientes potenciais e os enviam para a Marketo para uso em campanhas de marketing. No entanto, sem visibilidade sobre as conversões offline, o anunciante do Facebook não pode saber quais anúncios são mais eficazes. Aqui está um exemplo.

>[!NOTE]
>
>**Exemplo**
>
>O facebook Lead Ads veicula três anúncios.
>
>* O anúncio 1 gera 20 leads
>* O anúncio 2 gera 30 leads
>* O anúncio 3 gera 50 leads
>
>Com base apenas nesses números, a Ad 3 parece ser a mais eficaz.
>
>No entanto, ao analisar os dados no lado do Marketo, uma história diferente se desenvolve.
>
>* O anúncio 1 gera 10 vendas
>* O anúncio 3 gera 2 vendas
>
>Isso significa que o anúncio 1, apesar de gerar menos leads, teve uma taxa de sucesso de 50%, enquanto o anúncio 3 foi pouco eficaz.
>
>Sem conversões offline, o anunciante provavelmente investiria mais dinheiro no anúncio 3. Com dados de conversão offline, o anunciante terá mais probabilidade de investir no Ad 1.

Você pode [configurar Conversões Offline do Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) para enviar desempenho de anúncio offline para o Facebook.

1. Verifique se a sua [integração com o Facebook LaunchPoint](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) está atualizada.
1. Mapear estágios no seu Modelo de ciclo de receita para estágios de conversão offline no Facebook.
1. Quando um lead da Facebook é gerado a partir de um anúncio de lead da Facebook e atinge um estágio mapeado, a Marketo envia dados de conversão offline para a Facebook várias vezes por dia, por meio de uma API segura e automatizada. Os dados são exibidos no Relatório do Facebook Ads Manager.

>[!MORELIKETHIS]
>
>[Configurar conversões offline do Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
