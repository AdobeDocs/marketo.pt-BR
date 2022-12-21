---
unique-page-id: 2359791
description: Especificar meta para oferta de referência - Documentos do Marketo - Documentação do produto
title: Especificar meta para oferta de referência
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Especificar meta para oferta de referência {#specify-goal-for-referral-offer}

Quando você [criar uma oferta de referência](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md), é necessário definir a meta de realização. A meta pode ser definida por atividade de pessoa na página da Web, como visitas de página ou inscrições. Você também pode usar um [evento JavaScript personalizado](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

Como alternativa, você pode usar um acionador de lista inteligente no Marketo para aguardar qualquer marco, como uma oportunidade de criação para a pessoa referenciada.

Objetivos de exemplo:

* 10 visitas de peritos
* 5 assinaturas referidas
* 1 oportunidade de referência criada
* 2 compras de comércio eletrônico referidas
* 5 participantes referenciados do webinário

1. Ir para **Atividades de marketing**.

   ![](assets/ma.png)

1. Selecione a oferta de referência e clique em **Editar rascunho**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. No editor de ofertas de referência, acesse **Configurações do aplicativo** > **Detalhes da oferta**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Em **Configurações**, escolha um tipo de evento no **Objetivo de Cumprimento** lista suspensa.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Se planeja usar a variável **Conceder crédito ao referenciador** etapa de fluxo, você deve selecionar **Acionador da Smart List** como o tipo de meta de cumprimento aqui.

* Visitas referenciadas: Os participantes da oferta recebem crédito por cada visita de um amigo para a página que hospeda sua oferta.
* Logotipos referenciados: Os participantes da oferta recebem crédito por cada amigo que se inscreve na oferta.
* Acionador da Smart List: Os participantes da oferta recebem crédito por cada amigo que atende às condições de um [lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) acionar em um [campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). Por exemplo, você pode usar um acionador que é acionado quando um prospecto referenciado se inscreve para um webinário.

* Evento JavaScript personalizado: Os participantes da oferta recebem crédito por cada amigo que aciona um evento JavaScript definido em sua página. Consulte [Script de conversão para eventos personalizados](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>Existem novos filtros e acionadores disponíveis em campanhas inteligentes para monitorar a atividade social. Consulte [usar acionadores e filtros para atividades sociais](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Em seguida, você pode [selecione os emails de inscrição e preenchimento](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) para enviar a partir da sua oferta de referência.
