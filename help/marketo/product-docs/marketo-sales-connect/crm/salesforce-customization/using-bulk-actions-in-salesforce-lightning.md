---
unique-page-id: 42762825
description: Uso de ações em massa no Salesforce Lightning - Documentação do Marketo - Documentação do produto
title: Utilização de ações em massa no Salesforce Lightning
exl-id: 72022507-6568-4cc2-b3b5-c1703a1493ad
feature: Marketo Sales Connect
source-git-commit: fad80e8dccbad19b76570ee49fd8e7def0103fb1
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# Usando Ações em Massa em [!DNL Salesforce Lightning] {#using-bulk-actions-in-salesforce-lightning}

Saiba como executar ações em massa, como adicionar leads a uma campanha, enviar um email em massa ou enviar leads de [!DNL Salesforce] para [!DNL Sales Connect].

>[!PREREQUISITES]
>
>Atualize para a versão mais recente do pacote [!DNL Sales Connect] e instale os botões de ação em massa na exibição de cliente potencial/contato.
>* [Instruções em inglês] (assets/SF+Guide+for+Lightning-EN)
>* [Instruções em japonês, coreano, chinês] (assets/SF+Guide+for+Lightning-JA-KO-ZH)
>* [Instruções em espanhol, francês, alemão, italiano, sueco] (assets/SF+Guide+for+Lightning-ES-FR-DE-IT-SV)

>[!NOTE]
>
>Antes de seguir as etapas abaixo, verifique se você está conectado à sua conta do [!DNL Marketo Sales Connect].

## Email em massa {#bulk-email}

1. Em [!DNL Salesforce], clique na guia **[!UICONTROL Clientes potenciais]** e escolha a lista de clientes potenciais desejados.

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >Se você já estiver na lista que será usada, precisará executá-la novamente escolhendo-a no menu suspenso para garantir que os botões de ação em massa do MSC sejam exibidos. Este é um comportamento de [!DNL Salesforce] que não pode ser alterado.

1. Clique na lista suspensa de setas (na extremidade direita da tela) e selecione **[!UICONTROL Email with MSC]**.

   ![](assets/two-6.png)

1. Um email do MSC será exibido. Ele inclui os seguintes recursos:

   a. O campo &quot;[!UICONTROL Para]&quot; mostra &quot;Todos os recibos&quot; - isso corresponde à lista de clientes potenciais escolhida na Exibição da Lista de Clientes Potenciais
b. Esta lista está visível no painel esquerdo chamado &quot;Composição em massa&quot; - você pode adicionar/remover destinatários aqui
c. Você pode escolher um modelo ou criar seu próprio email
d. Você pode enviar o email imediatamente ou agendar o envio posteriormente

   ![](assets/three-5.png)

## Adicionar à campanha {#add-to-campaign}

1. Em [!DNL Salesforce], clique na guia **[!UICONTROL Clientes potenciais]** e escolha a lista de clientes potenciais desejados.

   ![](assets/four-4.png)

1. Clique na lista suspensa de setas (na extremidade direita da tela) e selecione **[!UICONTROL Adicionar à campanha MSC]**.

   ![](assets/five-4.png)

1. Um pop-up &quot;[!UICONTROL Adicionar pessoas à sua campanha]&quot; será exibido. Clique em **[!UICONTROL Avançar]** e passe pelo fluxo de campanha típico para acionar uma campanha MSC.

   ![](assets/six-1.png)

## Encaminhar para [!DNL Marketo Sales Connect] {#push-to-marketo-sales-connect}

1. Em [!DNL Salesforce], clique na guia **[!UICONTROL Clientes potenciais]** e escolha a lista de clientes potenciais desejados.

   ![](assets/seven-2.png)

1. Clique na lista suspensa de setas (na extremidade direita da tela) e selecione **[!UICONTROL Enviar para o MSC]**.

   ![](assets/eight-2.png)

1. Uma nova guia chamada &quot;[!DNL Salesforce] Bridge&quot; será aberta. Clique no botão **[!UICONTROL Prosseguir para o Grupo] →**.

   ![](assets/nine-2.png)

1. Você será encaminhado para sua conta MSC, onde verá um grupo criado com carimbo de data/hora. Você receberá uma notificação quando a sincronização for concluída e o grupo incluirá os clientes em potencial sincronizados de [!DNL Salesforce].

   ![](assets/ten-1.png)

>[!NOTE]
>
>Você pode seguir as mesmas etapas para usar ações em massa na Exibição da lista de contatos também.

>[!MORELIKETHIS]
>
>* [Enviando Emails por Email de Grupo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Compondo Emails em Massa com Selecionar e Enviar](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
