---
unique-page-id: 2359791
description: Especificar meta para a Oferta de referência - Documentos do marketing - Documentação do produto
title: Especificar meta para a Oferta de referência
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# Especificar meta para a Oferta de referência {#specify-goal-for-referral-offer}

Ao [criar uma oferta de referência](create-a-referral-offer.md), é necessário definir a meta de cumprimento. A meta pode ser definida por atividade pessoal na página da Web, como visitas de página ou inscrições. Você pode até mesmo usar um [evento JavaScript personalizado](../../../../product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

Como alternativa, você pode usar um [acionador de lista inteligente](specify-goal-for-referral-offer.md) no Marketo para aguardar qualquer marco, como uma oportunidade sendo criada para a pessoa referenciada.

Objetivos de exemplo:

* 10 visitas efetuadas
* 5 inscrições referenciadas
* 1 oportunidade de referência criada
* 2 compras de comércio eletrônico
* 5 participantes referenciados do webinário

1. Vá para **Atividades de marketing**.

   ![](assets/ma.png)

1. Selecione a oferta de referência e clique em **Editar Rascunho.**

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. No editor de oferta de referência, vá para **Configurações do aplicativo** > **Detalhes da Oferta.**

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Em **Settings**, escolha um tipo de evento no menu suspenso **Fulfillment Goal**.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Se você planeja usar a etapa de fluxo **Conceder crédito à Quem indicou**, selecione **Acionador de Lista inteligente** como o tipo de meta de cumprimento aqui.

* Visitas referenciadas: Os participantes da oferta recebem crédito por cada visita de um amigo para a página que hospeda sua oferta.
* Logotipos referenciados: Os participantes da oferta recebem crédito por cada amigo que se inscreve na oferta.
* Acionador de Lista inteligente: Os participantes da oferta recebem crédito por cada amigo que atende às condições de um acionador [lista inteligente](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) em uma [campanha inteligente](http://docs.marketo.com/display/docs/smart+campaigns). Por exemplo, você pode usar um acionador que é acionado quando um prospecto referenciado se inscreve para um webinar.

* Evento JavaScript personalizado: Os participantes da oferta recebem crédito por cada amigo que aciona um evento JavaScript definido na sua página. Consulte [Script de conversão para Eventos personalizados](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>Há novos filtros e acionadores disponíveis em campanhas inteligentes para monitorar a atividade social. Consulte [usar acionadores e filtros para atividades sociais](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Em seguida, você pode [selecionar os emails de inscrição e preenchimento](send-referral-offer-fulfillment-email.md) para enviar da sua oferta de referência.

