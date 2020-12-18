---
unique-page-id: 11379045
description: Adicionar uma Etapa de Fluxo para SMS - Documentos do Marketing - Documentação do Produto
title: Adicionar uma Etapa de Fluxo para SMS
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# Adicionar uma Etapa de Fluxo para SMS {#add-a-flow-step-for-sms}

O Marketo tem três etapas de fluxo que podem ser usadas em suas campanhas inteligentes SMS:

* **Enviar mensagem**  SMS - esta ação de fluxo envia mensagens para pessoas da lista inteligente de marketing que se inscrevem em uma lista de subscrição Vibes selecionada pelo usuário. Ele não inicia o processo de subscrição.
* **Assinar a Lista**  do Vibes - Essa ação de fluxo inicia o processo de subscrição do SMS por meio de uma Campanha de aquisição do Vibes selecionada pelo usuário. Em seguida, as Vibes enviam uma mensagem de confirmação; o recipient deve responder a ele para concluir o processo de subscrição.
* **Cancelar inscrição da Lista**  Vibes - Esta ação de fluxo cancela a inscrição de cada pessoa de uma lista de subscrição Vibes selecionada pelo usuário.

>[!NOTE]
>
>Ao enviar mensagens SMS:
>
>* Desduplicação de marketing por número de telefone. Portanto, se várias pessoas tiverem o mesmo número de telefone, apenas uma pessoa receberá a mensagem.
>* O Marketo não enviará para pessoas incluir na lista de bloqueios ou com Suspensão de marketing.

>



Para obter informações gerais sobre como configurar etapas de fluxo, consulte [Adicionar uma Etapa de fluxo a uma Campanha inteligente](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Aqui estão os fundamentos para o uso do SMS.

1. Em Meu marketing, clique em **Atividades de marketing**.

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. Encontre a campanha inteligente à qual deseja adicionar o fluxo SMS. Clique na guia **Fluxo**.

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. Arraste sobre o fluxo, por exemplo, **Enviar mensagem SMS**. Selecione a Mensagem SMS e a lista Vibes nos menus suspensos.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >O seletor de Lista Vibes atua como um filtro adicional para a audiência já identificada na lista inteligente para público alvo somente dos clientes potenciais que pertencem a essa lista Vibes.
   >
   >
   >Os fluxos **Inscrever-se na Lista do Vibes** e **Cancelar inscrição da Lista do Vibes** têm requisitos diferentes. Para **Subscribe**, tem de selecionar a lista Vibes e a campanha de aquisição Vibes. Para **Cancelar assinatura**, somente a lista Vibes é necessária.

