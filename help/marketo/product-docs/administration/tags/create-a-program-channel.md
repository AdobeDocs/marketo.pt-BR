---
unique-page-id: 2950682
description: Criar um canal de programa - Documentação do Marketo - Documentação do produto
title: Criar um canal de programa
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
feature: Tags
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Criar um canal de programa {#create-a-program-channel}

Um programa é uma iniciativa de marketing específica. O canal deve ser o mecanismo de entrega, como Webinar ou Patrocínio ou Anúncio online.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>Saiba mais sobre [programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md), o elemento mais importante do Marketo.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/create-a-program-channel-1.png)

1. Clique em **[!UICONTROL Marcas]**.

   ![](assets/create-a-program-channel-2.png)

   >[!NOTE]
   >
   >Por que tags? Um canal é uma maneira de descrever um programa, como outras tags. O canal tem apenas recursos extras especiais.

1. Clique no sinal **+** ao lado de [!UICONTROL Canal] para expandir e ver os canais existentes.

   ![](assets/create-a-program-channel-3.png)

1. Em **[!UICONTROL Novo]**, clique em **[!UICONTROL Novo canal]**.

   ![](assets/create-a-program-channel-4.png)

   >[!NOTE]
   >
   >**Exemplo**
   >
   >Canal: Outdoor
   >
   >* Aplicar a: Padrão
   >* Progressão: Membro, Envolvido (em caso de dúvida, esses trabalhos funcionam bem)
   >* Sucesso: Envolvido
   >
   >Canal: Festa
   >
   >* Aplicar a: Evento
   >* Progressão: Convidado, Inscrito, Sem Apresentação e Presente
   >* Sucesso: Participou
   >
   >Confira as Progressões dos canais existentes para ter uma ideia de como usá-los.

1. Vamos seguir o exemplo do Canal de partido. Nomeie seu novo **[!UICONTROL Canal]** e selecione o tipo de programa ao qual ele será aplicado.

   ![](assets/create-a-program-channel-5.png)

   >[!NOTE]
   >
   >Aplicar a quê? Existem vários tipos de programas. Corresponda o canal ao tipo certo. Em caso de dúvida, escolha **[!UICONTROL Padrão]**.

   >[!NOTE]
   >
   >Ao usar o &quot;[!UICONTROL Evento com o Webinar]&quot;, os mapeamentos do sistema serão bloqueados (conforme exigido pelas integrações do webinário) e não poderão ser editados.

1. Insira os dois primeiros nomes de Status do programa e clique em **[!UICONTROL Adicionar etapa]**.

   ![](assets/create-a-program-channel-6.png)

1. Digite o número da **[!UICONTROL Status]** e da **[!UICONTROL Etapa]** de outro programa e clique em **[!UICONTROL Adicionar Etapa]**.

   ![](assets/create-a-program-channel-7.png)

   >[!TIP]
   >
   >O número **[!UICONTROL Etapa]** é usado para classificar os status do programa. Lembre-se de que as pessoas não podem retroceder nesses passos de progressão. Eles só podem alterar o status para um status de valor maior ou igual. Use os valores iguais quando os status pretenderem alternar entre si, em vez de uma progressão.

1. Insira o número do último programa **[!UICONTROL Status]** e **[!UICONTROL Etapa]**.

   ![](assets/create-a-program-channel-8.png)

   >[!NOTE]
   >
   >Ao usar o tipo &quot;[!UICONTROL Evento]&quot;, o mapeamento do sistema para os status Registrado, Lista de Espera e Participou é necessário. Sendo assim, esses status não podem ser ocultos.

1. Escolha o **[!UICONTROL Status do Check-in para Dispositivos Móveis]** para **[!UICONTROL Registrado]**.

   ![](assets/create-a-program-channel-9.png)

1. Escolha o **[!UICONTROL Status de check-in móvel]** para **[!UICONTROL Participou]**.

   ![](assets/create-a-program-channel-10.png)

   >[!NOTE]
   >
   >As opções de **[!UICONTROL Status do Check-in para Dispositivos Móveis]** só estarão disponíveis se o canal for para programas de eventos.

   >[!NOTE]
   >
   >Somente as pessoas com **[!UICONTROL Status do Check-in para Dispositivos Móveis]** de **[!UICONTROL Registradas]** e **[!UICONTROL Participadas]** estarão visíveis nos [Aplicativos de Check-in para Dispositivos Móveis](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md).

   >[!TIP]
   >
   >Se uma nova pessoa for criada no aplicativo de check-in para dispositivos móveis, ela será definida como [!UICONTROL Registrada] no programa de evento. Se uma pessoa tiver feito o check-in no evento no aplicativo, ele será definido como [!UICONTROL Participou] do programa de evento.

1. Selecione o status do programa **[!UICONTROL Sucesso]** e clique em **[!UICONTROL Criar]**.

   ![](assets/create-a-program-channel-11.png)

   Muito bem! Quando você cria um novo programa desse tipo, esse novo canal será uma das opções.
