---
unique-page-id: 11379045
description: Adicionar uma etapa de fluxo para SMS - Documentação do Marketo - Documentação do produto
title: Adicionar uma etapa de fluxo para SMS
exl-id: 8e96f6ad-43c9-4d64-8cb6-241664956d72
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Adicionar uma etapa de fluxo para SMS {#add-a-flow-step-for-sms}

O Marketo tem três etapas de fluxo que você pode usar em suas campanhas inteligentes de SMS:

* **Enviar mensagem SMS** - Essa ação de fluxo envia mensagens para pessoas da smartlist Marketo que estão inscritas em uma lista de inscrição de Vibes selecionada pelo usuário. Ele não inicia o processo de assinatura.
* **Inscrever-se na lista de visibilidade** - Essa ação de fluxo inicia o processo de assinatura do SMS por meio de uma campanha de aquisição do Vibes selecionada pelo usuário. A Vibes envia uma mensagem de confirmação; o recipient deve responder a ele para concluir o processo de assinatura.
* **Cancelar inscrição na lista de vibrações** - Essa ação de fluxo cancela a assinatura de cada pessoa em uma lista de assinaturas de Vibes selecionada pelo usuário.

>[!NOTE]
>
>Ao enviar mensagens SMS:
>
>* A Marketo elimina a duplicação por número de telefone. Portanto, se várias pessoas tiverem o mesmo número de telefone, somente uma pessoa receberá a mensagem.
>* O Marketo incluir na lista de bloqueios não enviará para as pessoas que estão aprovadas ou com suspensão de marketing.

Para obter informações gerais sobre a configuração de etapas de fluxo, consulte [Adicionar uma etapa de fluxo a uma campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Estas são as noções básicas para usar o SMS.

1. Em Meu Marketo, clique em **Atividades de marketing**.

   ![](assets/add-a-flow-step-for-sms-1.png)

1. Encontre a campanha inteligente à qual você deseja adicionar o fluxo de SMS. Clique em **Fluxo** guia.

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. Arraste sobre o fluxo, por exemplo, **Enviar mensagem SMS**. Selecione a mensagem SMS e a lista Vibes nos menus suspensos.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >O seletor da Lista de vibrações atua como um filtro adicional para o público-alvo já identificado na lista inteligente para direcionar somente os leads que pertencem a essa lista de vibrações.
   >
   >A variável **Inscrever-se na lista de visibilidade** e **Cancelar inscrição na lista de vibrações** Os fluxos de trabalho têm requisitos diferentes. Para **Assinar**, você deve selecionar a lista Vibes e a campanha de aquisição Vibes. Para **Cancelar inscrição**, somente a lista Vibes é necessária.
