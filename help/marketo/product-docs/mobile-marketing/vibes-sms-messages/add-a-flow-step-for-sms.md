---
unique-page-id: 11379045
description: Adicionar uma etapa de fluxo para SMS - Documentos do Marketo - Documentação do produto
title: Adicionar uma etapa de fluxo para SMS
exl-id: 8e96f6ad-43c9-4d64-8cb6-241664956d72
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Adicionar uma etapa de fluxo para SMS {#add-a-flow-step-for-sms}

O Marketo tem três etapas de fluxo que você pode usar em suas campanhas inteligentes de SMS:

* **Enviar mensagem SMS** - Essa ação de fluxo envia mensagens para pessoas da lista inteligente do Marketo que assinaram uma lista de assinaturas Vibes selecionada pelo usuário. Ele não inicia o processo de assinatura.
* **Inscrever-se na Lista de Vibes** - Essa ação de fluxo inicia o processo de assinatura do SMS por meio de uma Campanha de aquisição de Vibes selecionada pelo usuário. Vibes envia uma mensagem de confirmação; o recipient deve responder a ele para concluir o processo de assinatura.
* **Cancelar assinatura da lista de vibes** - Essa ação de fluxo cancela a assinatura de cada pessoa de uma lista de assinaturas Vibes selecionada pelo usuário.

>[!NOTE]
>
>Ao enviar mensagens SMS:
>
>* Desduplicação do Marketo por número de telefone. Portanto, se várias pessoas tiverem o mesmo número de telefone, somente uma pessoa receberá a mensagem.
>* O Marketo não será enviado para pessoas incluir na lista de bloqueios ou com Suspensão de Marketing.


Para obter informações gerais sobre como configurar etapas de fluxo, consulte [Adicionar uma etapa de fluxo a uma campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Estas são as noções básicas para usar o SMS.

1. Em Minha Marketo, clique em **Atividades de marketing**.

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. Encontre a campanha inteligente à qual deseja adicionar o fluxo de SMS. Clique no botão **Fluxo** guia .

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. Arraste sobre o fluxo, por exemplo, **Enviar mensagem SMS**. Selecione a Mensagem SMS e a lista de Vibes nos menus suspensos.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >O seletor de Lista de Vibes atua como um outro filtro para o público-alvo já identificado na lista inteligente para direcionar somente os leads que pertencem a essa lista de Vibes.
   >
   >O **Inscrever-se na Lista de Vibes** e **Cancelar assinatura da lista de vibes** os fluxos têm requisitos diferentes. Para **Assinar**, selecione a lista Vibes e a campanha de aquisição Vibes . Para **Cancelar inscrição**, somente a lista Vibes é obrigatória.
