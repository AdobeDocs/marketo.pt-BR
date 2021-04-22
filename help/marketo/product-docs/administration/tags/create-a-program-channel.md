---
unique-page-id: 2950682
description: Criar um canal do programa - Documentos do Marketo - Documentação do produto
title: Criar um canal de programa
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Criar um canal de programa {#create-a-program-channel}

Um programa é uma iniciativa específica de marketing. O canal deve ser o mecanismo de entrega, como Webinar ou Sponsorship ou Anúncio online.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>Saiba mais sobre os [programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md), o elemento mais importante no Marketo.

1. Na seção **Admin**, clique em **Tags**.

   ![](assets/image2014-9-24-12-3a57-3a27.png)

   >[!NOTE]
   >
   >Por que tags? Um canal é uma maneira de descrever um programa, assim como outras tags. O canal tem apenas recursos extras especiais.

1. Clique no sinal **+** ao lado de **Canal** para expandir e ver os canais existentes.

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
   >* Progressão: Membro, Envolvido (em caso de dúvida, funcionam bem)
   >* Sucesso: Envolvido

   >
   >Canal: Parte
   >
   >* Aplicar a: Evento
   >* Progressão: Convidado, Registrado, Sem Programa e Participado
   >* Sucesso: Participante

   >
   >Confira os Progressos dos canais existentes para ter uma ideia de como usá-los.

1. Vamos com o exemplo do canal de Partido. Nomeie seu novo **Canal** e selecione o tipo de programa ao qual ele será aplicado.

   ![](assets/image2014-9-24-13-3a0-3a17.png)

   >[!NOTE]
   >
   >Aplicar a quê? Existem vários tipos de programas. Corresponda o canal ao tipo correto. Em caso de dúvida, escolha **Default**.

   >[!NOTE]
   >
   >Ao usar &quot;Evento com webinar&quot;, os mapeamentos do sistema serão bloqueados (conforme exigido pelas integrações do webinar) e não poderão ser editados.

   Insira os dois primeiros nomes de status do programa e clique em Adicionar etapa.
   ![](assets/image2014-9-24-15-3a37-3a0.png)

1. Insira outro número de programa **Status** e **Etapa** e clique em **Adicionar Etapa**.

   ![](assets/image2014-9-24-15-3a37-3a30.png)

   >[!TIP]
   >
   >O número **Step** é usado para classificar os status do programa. Lembre-se de que as pessoas não podem retroceder nessas etapas de progressão. Eles só podem alterar o status para um status de valor maior ou igual. Use os valores iguais quando os status forem destinados a alternar para frente e para trás em vez de uma progressão.

1. Insira o último número do programa **Status** e **Step**.

   ![](assets/image2014-9-24-15-3a39-3a15.png)

   >[!NOTE]
   >
   >Ao usar o tipo &quot;Evento&quot;, é necessário o mapeamento de sistema para os status Registrado, Lista de Espera e Participado. Dessa forma, esses status não podem ser ocultos.

1. Escolha o **Status de Check-in Móvel** para **Registrado**.

   ![](assets/image2014-9-24-15-3a39-3a43.png)

1. Escolha o **Status de Check-in Móvel** para **Participado**.

   ![](assets/image2014-9-24-15-3a40-3a21.png)

   >[!NOTE]
   >
   >**As opções Mobile Check-in Status**** **só estarão disponíveis se o canal for para programas de evento.

   >[!NOTE]
   >
   >Somente as pessoas com um **Status de Check-in Móvel** de **Registradas** e **Participadas** estarão visíveis nos [Aplicativos de Check-in Móvel](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md).

   >[!TIP]
   >
   >Se uma nova pessoa for criada no aplicativo de check-in móvel, ela será definida como Registrado no programa de eventos. Se uma pessoa for verificada no evento no aplicativo, ela será definida como Participada no programa de eventos.

1. Selecione o status do programa **Sucesso** e clique em **Criar**.

   ![](assets/image2014-9-24-15-3a42-3a54.png)

   Muito bem! Quando você faz um novo programa desse tipo, esse novo canal será uma das opções.
