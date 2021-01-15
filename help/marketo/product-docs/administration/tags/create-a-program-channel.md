---
unique-page-id: 2950682
description: Criar um Canal de Programa - Documentos do Marketing - Documentação do produto
title: Criar um Canal de Programa
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---


# Criar um Canal de Programa {#create-a-program-channel}

Um programa é uma iniciativa de marketing específica. O canal deve ser o mecanismo do delivery, como Webinar ou Patrocínio ou Anúncio online.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>Saiba mais sobre [programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md), o elemento mais importante no Marketo.

1. Na seção **Admin**, clique em **Tags**.

   ![](assets/image2014-9-24-12-3a57-3a27.png)

   >[!NOTE]
   >
   >Por que etiquetas? Um canal é uma forma de descrever um programa, assim como outras tags. O canal tem apenas recursos extras especiais.

1. Clique no sinal de **+** ao lado de **Canal** para expandir e ver canais existentes.

   ![](assets/image2014-9-24-12-3a58-3a33.png)

1. Em **Novo**, clique em **Novo Canal**.

   ![](assets/image2014-9-24-12-3a58-3a53.png)

   >[!NOTE]
   >
   >**Exemplo**
   >
   >Canal: Outdoor
   >
   >* Aplicar a: Padrão
   >* Progressão: Membro, Envolvido (em caso de dúvida, estes funcionam bem)
   >* Sucesso: Envolvido

   >
   >Canal: Parte
   >
   >* Aplicar a: Evento
   >* Progressão: Convidado, Registrado, Sem Mostrar e Participante
   >* Sucesso: Participante

   >
   >Confira as Progressões de canais existentes para ter uma ideia de como usá-los.

1. Vamos ver o exemplo do canal do Partido. Nomeie seu novo **Canal** e selecione o tipo de programa ao qual ele será aplicado.

   ![](assets/image2014-9-24-13-3a0-3a17.png)

   >[!NOTE]
   >
   >Aplicar a quê? Há vários tipos de programas. Corresponder o canal ao tipo correto. Em caso de dúvida, escolha **Padrão**.

   >[!NOTE]
   >
   >Ao usar &quot;Evento com Webinar&quot;, os mapeamentos do sistema serão bloqueados (conforme exigido pelas integrações de webinar) e não poderão ser editados.

   Digite os dois primeiros nomes de Status do programa e clique em Adicionar etapa.
   ![](assets/image2014-9-24-15-3a37-3a0.png)

1. Digite outro número de programa **Status** e **Etapa**, em seguida, clique em **Adicionar Etapa**.

   ![](assets/image2014-9-24-15-3a37-3a30.png)

   >[!TIP]
   >
   >O número **Step** é usado para classificar os status dos programas. Lembre-se de que as pessoas não podem recuar nestes passos de progressão. Eles só podem alterar o status para um status de valor maior ou igual. Use os valores iguais quando os status forem destinados a alternar para frente e para trás em vez de uma progressão.

1. Digite o último número **Status** e **Etapa** do programa.

   ![](assets/image2014-9-24-15-3a39-3a15.png)

   >[!NOTE]
   >
   >Ao usar o tipo &quot;Evento&quot;, o mapeamento do sistema para status Registrado, Lista de Espera e Participante é necessário. Como tal, esses status não podem ser ocultos.

1. Escolha **Status de check-in móvel** para **Registrado**.

   ![](assets/image2014-9-24-15-3a39-3a43.png)

1. Escolha **Status de check-in móvel** para **Participado**.

   ![](assets/image2014-9-24-15-3a40-3a21.png)

   >[!NOTE]
   >
   >**As opções Mobile Check-in Status**** **só estarão disponíveis se o canal for para programas.

   >[!NOTE]
   >
   >Somente pessoas com **Status de check-in móvel** de **Registradas** e **Participadas** estarão visíveis nos [Aplicativos de check-in móveis](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md).

   >[!TIP]
   >
   >Se uma nova pessoa for criada no aplicativo de check-in móvel, ela será definida como Registrada no programa do evento. Se uma pessoa for verificada no evento do aplicativo, ele será definido como Participante no programa do evento.

1. Selecione o status do programa **Success** e clique em **Create**.

   ![](assets/image2014-9-24-15-3a42-3a54.png)

   Muito bem! Quando você fizer um novo programa desse tipo, esse novo canal será uma das opções.
