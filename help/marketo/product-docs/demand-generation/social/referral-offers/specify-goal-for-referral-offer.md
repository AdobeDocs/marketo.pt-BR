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

Ao [criar uma oferta](create-a-referral-offer.md)de referência, é necessário definir a meta de realização. A meta pode ser definida por atividade pessoal na página da Web, como visitas de página ou inscrições. Você pode até mesmo usar um evento [JavaScript](../../../../product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md)personalizado.

Como alternativa, você pode usar um acionador [de lista](specify-goal-for-referral-offer.md) inteligente em Marketo para aguardar qualquer marco, como uma oportunidade que está sendo criada para a pessoa referenciada.

Objetivos de exemplo:

* 10 visitas efetuadas
* 5 inscrições referenciadas
* 1 oportunidade de referência criada
* 2 compras de comércio eletrônico
* 5 participantes referenciados do webinário

1. Vá para **Marketing Atividade**.

   ![](assets/ma.png)

1. Selecione a oferta de referência e clique em **Editar rascunho.**

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. No editor de oferta de referência, vá para Configurações **do** aplicativo > Detalhes da **Oferta.**

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Em **Configurações**, escolha um tipo de evento no menu suspenso Objetivo de **disponibilização** .

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Se você planeja usar a etapa de fluxo **Conceder crédito à Quem indicou** , é necessário selecionar Acionador **de Lista** inteligente como o tipo de meta de cumprimento aqui.

* Visitas referenciadas: Os participantes da oferta recebem crédito por cada visita de um amigo para a página que hospeda sua oferta.
* Logotipos referenciados: Os participantes da oferta recebem crédito por cada amigo que se inscreve na oferta.
* Acionador de Lista inteligente: Os participantes da oferta recebem crédito por cada amigo que atende às condições de um acionador de lista [](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) inteligente em uma campanha [](http://docs.marketo.com/display/docs/smart+campaigns)inteligente. Por exemplo, você pode usar um acionador que é acionado quando um prospecto referenciado se inscreve para um webinar.

* Evento JavaScript personalizado: Os participantes da oferta recebem crédito por cada amigo que aciona um evento JavaScript definido na sua página. Consulte Script [de conversão para Eventos](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)personalizados.

>[!NOTE]
>
>Há novos filtros e acionadores disponíveis em campanhas inteligentes para monitorar a atividade social. Consulte [usar acionadores e filtros para atividades](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)sociais.

>[!MORELIKETHIS]
>
>Em seguida, você pode [selecionar os emails](send-referral-offer-fulfillment-email.md) de inscrição e preenchimento a serem enviados da sua oferta de referência.

