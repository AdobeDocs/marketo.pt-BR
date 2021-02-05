---
unique-page-id: 2359791
description: Especificar meta para a Oferta de referência - Documentos do marketing - Documentação do produto
title: Especificar meta para a Oferta de referência
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Especificar meta para a Oferta de referência {#specify-goal-for-referral-offer}

Ao [criar uma oferta de referência](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md), é necessário definir a meta de cumprimento. A meta pode ser definida por atividade pessoal na página da Web, como visitas de página ou inscrições. Você pode até mesmo usar um [evento JavaScript personalizado](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

Como alternativa, você pode usar um acionador de lista inteligente no Marketo para aguardar qualquer marco, como uma oportunidade que está sendo criada para a pessoa referenciada.

Objetivos de exemplo:

* 10 visitas efetuadas
* 5 inscrições referenciadas
* 1 oportunidade de referência criada
* 2 compras de comércio eletrônico
* 5 participantes referenciados do webinário

1. Vá para **Atividades de marketing**.

   ![](assets/ma.png)

1. Selecione a oferta de referência e clique em **Editar rascunho**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. No editor de oferta de referência, vá para **Configurações do aplicativo** > **Detalhes da Oferta**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Em **Settings**, escolha um tipo de evento no menu suspenso **Fulfillment Goal**.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Se você planeja usar a etapa de fluxo **Conceder crédito à Quem indicou**, selecione **Acionador de Lista inteligente** como o tipo de meta de cumprimento aqui.

* Visitas referenciadas: Os participantes da oferta recebem crédito por cada visita de um amigo para a página que hospeda sua oferta.
* Logotipos referenciados: Os participantes da oferta recebem crédito por cada amigo que se inscreve na oferta.
* Acionador de Lista inteligente: Os participantes da oferta recebem crédito por cada amigo que atende às condições de um acionador [lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) em uma [campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). Por exemplo, você pode usar um acionador que é acionado quando um prospecto referenciado se inscreve para um webinar.

* Evento JavaScript personalizado: Os participantes da oferta recebem crédito por cada amigo que aciona um evento JavaScript definido na sua página. Consulte [Script de conversão para Eventos personalizados](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>Há novos filtros e acionadores disponíveis em campanhas inteligentes para monitorar a atividade social. Consulte [usar acionadores e filtros para atividades sociais](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Em seguida, você pode [selecionar os emails de inscrição e preenchimento](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) para enviar da sua oferta de referência.
