---
unique-page-id: 2950682
description: Etapas para criar um canal de programa com status e etapas de progressão, incluindo tipo de programa, status de sucesso e opções de check-in móvel para eventos.
title: Criar um canal de programa
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
feature: Tags
TQID: https://experienceleague.adobe.com/Ficlv7OfEScqLRVbOfc2hc-S3cQ2YjriiKWnbS1Op9A
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2: id: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 435
ht-degree: 2%

---

# Criar um canal de programa {#create-a-program-channel}

Um programa é uma iniciativa de marketing específica. O canal deve ser o mecanismo de entrega, como Webinar ou Patrocínio ou Anúncio online.

>[!NOTE]
>
>**Permissões de administrador são necessárias**

>[!NOTE]
>
>Saiba mais sobre [programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md), o elemento mais importante do Marketo.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/create-a-program-channel-1.png)

1. Clique em **[!UICONTROL Marcas]**.

   ![](assets/create-a-program-channel-2.png)

   >[!NOTE]
   >
   >Por que tags? Um canal é uma maneira de descrever um programa, como outras tags. O canal tem recursos extras especiais.

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
   >* Progressão: Membro, Envolvido (são padrões adequados)
   >* Sucesso: Envolvido
   >
   >Canal: Festa
   >
   >* Aplicar a: Evento
   >* Progressão: Convidado, Inscrito, Sem Apresentação e Presente
   >* Sucesso: Participou
   >
   >Revise o andamento dos canais existentes para obter orientação sobre como usá-los.

1. Usando o Canal de participante como exemplo, nomeie seu novo **[!UICONTROL Canal]** e selecione o tipo de programa ao qual ele será aplicado.

   ![](assets/create-a-program-channel-5.png)

   >[!NOTE]
   >
   >Existem vários tipos de programas. Corresponda o canal ao tipo certo. Se não tiver certeza, escolha **[!UICONTROL Padrão]**.

   >[!NOTE]
   >
   >Ao usar o &quot;[!UICONTROL Evento com o Webinar]&quot;, os mapeamentos do sistema serão bloqueados (conforme exigido pelas integrações do webinário) e não poderão ser editados.

1. Insira os dois primeiros nomes de Status do programa e clique em **[!UICONTROL Adicionar etapa]**.

   ![](assets/create-a-program-channel-6.png)

1. Digite o número da **[!UICONTROL Status]** e da **[!UICONTROL Etapa]** de outro programa e clique em **[!UICONTROL Adicionar Etapa]**.

   ![](assets/create-a-program-channel-7.png)

   >[!TIP]
   >
   >O número **[!UICONTROL Etapa]** é usado para classificar os status do programa. Observe que as pessoas não podem retroceder nesses passos de progressão. Eles só podem alterar o status para um status de valor maior ou igual. Use os valores iguais quando os status pretenderem alternar entre si, em vez de uma progressão.

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

   Quando você cria um novo programa desse tipo, esse novo canal será uma das opções.
