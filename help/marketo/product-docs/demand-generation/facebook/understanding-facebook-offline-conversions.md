---
unique-page-id: 11383945
description: Noções básicas sobre conversões offline do Facebook - Documentos do Marketo - Documentação do produto
title: Noções básicas sobre conversões offline do Facebook
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Noções básicas sobre conversões offline do Facebook {#understanding-facebook-offline-conversions}

As campanhas do facebook Lead Ads geram leads e os enviam para a Marketo para uso em campanhas de marketing. No entanto, sem visibilidade sobre conversões offline, o anunciante do Facebook não pode saber quais anúncios são mais eficazes. Aqui está um exemplo.

>[!NOTE]
>
>**Exemplo**
>
>O facebook Lead Ads executa três anúncios.
>
>* Anúncio 1 gera 20 leads
>* Anúncio 2 gera 30 leads
>* Anúncio 3 gera 50 leads
>
>Baseado apenas nesses números, o anúncio 3 parece ser o mais eficaz.
>
>No entanto, ao analisar dados no Marketo, uma história diferente se desenvolve.
>
>* Anúncio 1 gera 10 vendas
>* Anúncio 3 gera 2 vendas
>
>Isso significa que o Anúncio 1, apesar de gerar menos leads, teve uma taxa de sucesso de 50%, enquanto o Anúncio 3 não foi nada eficaz.
>
>Sem conversões offline, o anunciante provavelmente investiria mais dinheiro no Anúncio 3. Com os dados de conversão offline, o anunciante provavelmente investirá no Anúncio 1.

Você pode [configurar conversões offline do Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) para enviar desempenho de anúncio offline para o Facebook.

1. Certifique-se de que [Integração do facebook LaunchPoint](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) está atualizado.
1. Mapeie os estágios no seu Modelo de ciclo de receita para estágios de conversão offline no Facebook.
1. Quando um lead para Facebook é gerado a partir de um anúncio de lead para Facebook e atinge um estágio mapeado, o Marketo envia dados de conversão offline de volta ao Facebook várias vezes por dia por meio de uma API segura e automatizada. Os dados são exibidos no Relatório do gerenciador de anúncios do Facebook.

>[!MORELIKETHIS]
>
>[Configurar conversões offline do Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
