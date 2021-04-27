---
unique-page-id: 2949865
description: Criar um evento com o Adobe Connect - Marketo Docs - Documentação do produto
title: Criar um evento com o Adobe Connect
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
translation-type: tm+mt
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Criar um evento com o Adobe Connect {#create-an-event-with-adobe-connect}

Sincronizar com o Adobe Connect permite gerenciar sua inscrição no webinário e presença no Marketo, o que garante que o envolvimento não seja desacompanhado.

>[!PREREQUISITES]
>
>* [Vincular a Adobe Connect e a Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [Criar um novo programa de evento](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


Primeiro, certifique-se de ter criado sua reunião ou seminário no Adobe Connect. Se precisar de ajuda, confira o [Guia do Usuário do Adobe Connect](https://help.adobe.com/en_US/connect/9.0/using/index.html).

As reuniões e os seminários criados no Adobe Connect devem ser criados na pasta especificada ao inserir suas credenciais no Marketo. Após criar a reunião ou seminário, anote todas as informações logísticas relevantes (como o número de telefone) a serem usadas no email de confirmação e no arquivo ICS.

>[!CAUTION]
>
>Como o host do evento, certifique-se de ingressar no aplicativo e **not** pelo link enviado aos participantes.

>[!NOTE]
>
>No momento, não oferecemos suporte ao Adobe Connect no local.

1. Na página inicial de um novo evento, selecione **Ações do Evento** e **Configurações do Evento**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Se você não vir **Configurações do evento** no menu suspenso, verifique se o canal do evento tem **Evento com webinar** selecionado em &quot;Aplica-se a&quot;.

1. Em **Parceiro de eventos**, selecione **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. Selecione sua ID de **Logon** e selecione seu **Evento**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Clique em **Salvar**.

   ![](assets/event-settings-overview.png)

   Legal! O evento do Adobe Connect agora é sincronizado com o evento do Marketo.

   >[!NOTE]
   >
   >Os campos que o Marketo envia são: Nome, Sobrenome, Endereço De Email.

   >[!TIP]
   >
   >Para inserir o URL exclusivo da pessoa em um email, use este token: `{{member.webinar url}}`. Quando o email é enviado, esse token resolve automaticamente o URL de confirmação exclusivo da pessoa do Adobe Connect.
   >
   >Defina seu email de confirmação para **Operacional** para garantir que as pessoas que se registram e podem ser canceladas ainda recebam suas informações de confirmação.

   As pessoas que se inscreverem no seu webinário serão encaminhadas para o seu provedor de webinário por meio da etapa de fluxo Alterar status do programa , quando o Novo status for definido como &quot;Registrado&quot;. Nenhum outro status empurrará a pessoa. Além disso, certifique-se de fazer a etapa 1 do fluxo Alterar status do programa e Enviar fluxo de email etapa 2.

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >Evite usar programas de email aninhados para enviar seus emails de confirmação. Em vez disso, use a campanha inteligente do programa de eventos, conforme mostrado acima.

   >[!TIP]
   >
   >Pode levar até 48 horas para que os dados apareçam no Marketo. Se, depois de esperar tanto tempo que você ainda não vir nada, selecione **Refresh from Webinar Provider** no menu Event Actions na guia Summary do seu evento.

   >[!MORELIKETHIS]
   >
   >* [Adicionar o Adobe Connect as a LaunchPoint Service](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [Editar um canal de evento](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)

