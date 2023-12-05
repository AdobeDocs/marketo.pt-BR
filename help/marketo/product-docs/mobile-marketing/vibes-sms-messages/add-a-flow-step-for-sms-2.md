---
description: Adicionar uma etapa de fluxo para SMS - Documentação do Marketo - Documentação do produto
title: Adicionar uma etapa de fluxo para SMS
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Adicionar uma etapa de fluxo para SMS {#add-a-flow-step-for-sms}

O Marketo Engage tem três etapas de fluxo que você pode usar nas Campanhas inteligentes de SMS:

* **Enviar mensagem SMS** - Essa ação de fluxo envia mensagens para pessoas da Smart List do Marketo que estão inscritas em uma lista de inscrição de vibrações de opt-in do usuário. Ele não inicia o processo de assinatura.
* **Inscrever-se na lista de visibilidade** - Essa ação de fluxo inicia o processo de assinatura do SMS por meio de uma campanha de aquisição do Vibes selecionada pelo usuário. A Vibes envia uma mensagem de confirmação; o recipient deve responder &quot;Y&quot; a ele para confirmar a aceitação em 24 horas. Depois que o usuário aceitar, ele se tornará membro da lista de inscrição do Vibes associada.
* **Cancelar inscrição na lista de vibrações** - Essa ação de fluxo cancela a assinatura de cada pessoa em uma lista de assinaturas de Vibes de opt-in do usuário. Quando um usuário digita &quot;stop&quot; para o seu código, o registro pessoal dele é atualizado para refletir que não é mais membro da lista de assinaturas do Vibes.

>[!NOTE]
>
>Ao enviar mensagens SMS:
>
>* A Marketo elimina a duplicação por número de telefone. Assim, se várias pessoas tiverem o mesmo número de telefone, somente uma pessoa receberá a mensagem se for membro de apenas uma lista de assinaturas Vibes. A desduplicação é feita no nível da lista de assinaturas Vibes, não no nível do programa Marketo.
>* O Marketo incluir na lista de bloqueios não enviará para as pessoas que estão aprovadas ou com suspensão de marketing.

Para obter informações gerais sobre a configuração de etapas de fluxo, consulte [Adicionar uma etapa de fluxo a uma campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Estas são as noções básicas para usar o SMS.

1. Em Meu Marketo, clique em **Atividades de marketing**.

   ![](assets/add-a-flow-step-for-sms-1.png)

1. Localize e selecione a Campanha inteligente à qual deseja adicionar o fluxo de SMS.

   CAPTURA DE TELA

1. Na guia Smart List, escolha o(s) acionador(es) desejado(s) (por exemplo, &quot;Formulário preenchido&quot;).

   CAPTURA DE TELA

1. No **Fluxo** arraste sobre a etapa de fluxo (por exemplo, **Enviar mensagem SMS**). Selecione a mensagem SMS e a lista Vibes nos menus suspensos.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >O seletor da Lista de vibrações atua como um filtro adicional para o público-alvo já identificado na lista inteligente para direcionar somente os leads que pertencem a essa lista de vibrações.
   >
   >A variável **Inscrever-se na lista de visibilidade** e **Cancelar inscrição na lista de vibrações** Os fluxos de trabalho têm requisitos diferentes. Para **Assinar**, você deve selecionar a lista Vibes e a campanha de aquisição Vibes. Para **Cancelar inscrição**, somente a lista Vibes é necessária.
