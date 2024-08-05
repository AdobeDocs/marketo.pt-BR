---
unique-page-id: 2359791
description: Especificar meta para oferta de referência - Documentação do Marketo - Documentação do produto
title: Especificar Meta para Oferta de Referência
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 0%

---

# Especificar Meta para Oferta de Referência {#specify-goal-for-referral-offer}

Quando você [cria uma oferta de referência](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md), é necessário definir a meta de preenchimento. A meta pode ser definida por atividade de pessoa na página da Web, como visitas de página ou inscrições. Você pode até mesmo usar um [evento personalizado do JavaScript](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

>[!IMPORTANT]
>
>Em 31 de julho de 2024, iniciamos o processo de desativação desse recurso. Não é mais possível criar novos ativos. Os ativos existentes continuarão a funcionar até 31 de janeiro de 2025. [Saiba mais](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

Como alternativa, você pode usar um acionador de lista inteligente no Marketo Engage para aguardar qualquer marco, como uma oportunidade que está sendo criada para a pessoa indicada.

Exemplo de metas:

* 10 visitas referidas
* 5 inscrições referenciadas
* 1 oportunidade referenciada criada
* 2 compras referidas de comércio eletrônico
* 5 participantes do webinário indicados

1. Vá para **Atividades de marketing**.

   ![](assets/ma.png)

1. Selecione a oferta de referência e clique em **Editar rascunho**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. No editor de oferta de referência, vá para **Configurações do Aplicativo** > **Detalhes da Oferta**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Em **Configurações**, escolha um tipo de evento na lista suspensa **Meta de Atendimento**.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Se você planeja usar a etapa de fluxo **Dar Crédito ao Referenciador**, selecione **Acionador da Smart List** como o tipo de meta de preenchimento aqui.

* Visitas referenciadas: os participantes da oferta recebem crédito por cada visita de um amigo à página que hospeda sua oferta.
* Inscrições referenciadas: os participantes da oferta recebem crédito por cada amigo que se inscreve na oferta.
* Acionador da lista inteligente: os participantes da oferta recebem crédito por cada amigo que atende às condições de um acionador de [lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) em uma [campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). Por exemplo, você pode usar um acionador que é acionado quando um cliente potencial indicado se inscreve em um webinário.

* Evento JavaScript personalizado: os participantes da oferta recebem crédito por cada amigo que aciona um evento JavaScript definido em sua página. Consulte [Script de conversão para eventos personalizados](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>Há novos filtros e acionadores disponíveis em campanhas inteligentes para monitorar a atividade social. Consulte [usar acionadores e filtros para atividades sociais](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Em seguida, você pode [selecionar os emails de inscrição e de preenchimento](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) a serem enviados a partir da sua oferta de referência.
