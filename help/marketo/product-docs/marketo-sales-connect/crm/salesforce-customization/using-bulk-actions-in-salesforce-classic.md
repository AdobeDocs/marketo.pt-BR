---
unique-page-id: 42762794
description: Uso de Ações em Massa no  [!DNL Salesforce] Classic - Documentação do Marketo - Documentação do produto
title: Usando Ações em Massa no  [!DNL Salesforce] Classic
exl-id: f676ba65-6bc9-41e5-aa70-0f10bceedab7
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 2%

---

# Usando Ações em Massa no [!DNL Salesforce] Classic {#using-bulk-actions-in-salesforce-classic}

Saiba como executar ações em massa, como adicionar leads a uma campanha, enviar um email em massa ou enviar leads de [!DNL Salesforce] para [!DNL Sales Connect].

>[!PREREQUISITES]
>
>Atualize para a versão mais recente do pacote [!DNL Sales Connect] e instale os botões de ação em massa na exibição de cliente potencial/contato. [Clique aqui para obter instruções](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Antes de seguir as etapas descritas, verifique se você está conectado à sua conta Marketo Sales Connect.

## Email em massa {#bulk-email}

1. Em [!DNL Salesforce], clique na guia **[!UICONTROL Clientes Potenciais]** e, em seguida, no botão **[!UICONTROL Ir]**.

   ![](assets/one-5.png)

1. Escolha os clientes em potencial desejados e clique no botão **[!UICONTROL Email com MSC (Classic)]**.

   ![](assets/two-5.png)

1. Um email do MSC será exibido. Ele inclui os seguintes recursos:

   a. O campo &quot;[!UICONTROL Para]&quot; mostra &quot;[!UICONTROL Todos os Destinatários]&quot; - isso corresponde à lista de clientes potenciais escolhidos na Exibição da Lista de Clientes Potenciais
b. Esta lista está visível no painel esquerdo chamado &quot;[!UICONTROL Composição em Massa]&quot; - você pode adicionar/remover destinatários aqui
c. Você pode escolher um modelo ou criar seu próprio email
d. Você pode visualizar os campos dinâmicos que serão preenchidos no seu email
e. Você pode enviar o email imediatamente ou agendar o envio posteriormente

   ![](assets/three-4.png)

## Adicionar à campanha {#add-to-campaign}

1. Em [!DNL Salesforce], clique na guia **[!UICONTROL Clientes Potenciais]** e, em seguida, no botão **[!UICONTROL Ir]**.

   ![](assets/four-3.png)

1. Escolha os clientes em potencial desejados e clique no botão **[!UICONTROL Adicionar ao MSC Campaign (Classic)]**.

   ![](assets/five-3.png)

1. Um pop-up &quot;[!UICONTROL Adicionar pessoas à sua campanha]&quot; será exibido. Clique em **[!UICONTROL Avançar]** e passe pelo fluxo de campanha típico para acionar uma campanha MSC.

   ![](assets/six.png)

## Enviar por push ao Marketo Sales Connect {#push-to-marketo-sales-connect}

1. Em [!DNL Salesforce], clique na guia **[!UICONTROL Clientes Potenciais]** e, em seguida, no botão **[!UICONTROL Ir]**.

   ![](assets/seven-1.png)

1. Escolha os clientes em potencial desejados e clique no botão **[!UICONTROL Encaminhar para MSC (Clássico)]**.

   ![](assets/eight-1.png)

1. Uma nova guia chamada &quot;[!UICONTROL Salesforce Bridge]&quot; será aberta. Clique no botão **[!UICONTROL Prosseguir para o grupo →]**.

   ![](assets/nine-1.png)

1. Você será encaminhado para sua conta MSC, onde verá um grupo criado com carimbo de data/hora. Você receberá uma notificação quando a sincronização for concluída e o grupo incluirá os clientes em potencial sincronizados de [!DNL Salesforce].

   ![](assets/ten.png)

>[!NOTE]
>
>Você pode seguir as mesmas etapas para usar ações em massa na Exibição da lista de contatos também.

>[!MORELIKETHIS]
>
>* [Enviando Emails por Email de Grupo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Compondo Emails em Massa com Selecionar e Enviar](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
