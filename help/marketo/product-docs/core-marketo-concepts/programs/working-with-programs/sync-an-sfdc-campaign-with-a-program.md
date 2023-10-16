---
unique-page-id: 1147154
description: Sincronizar uma campanha SFDC com um programa - Documentação do Marketo - Documentação do produto
title: Sincronizar uma campanha SFDC com um programa
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: e49860ae611f2f77789bb491aeccbee46a911a2c
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 1%

---

# Sincronizar uma campanha SFDC com um programa {#sync-an-sfdc-campaign-with-a-program}

O Marketo Engage permite sincronizar seus programas com [!DNL Salesforce] campanhas para manter a mesma lista de pessoas em ambos os sistemas, incluindo seus status. Vamos começar!

>[!PREREQUISITES]
>
>Você precisará [habilitar [!DNL Salesforce] sincronização de campanha](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) primeiro.

>[!CAUTION]
>
>Ao sincronizar uma campanha do SFDC com um programa Marketo Engage, as ações implícitas do SFDC (por exemplo, adicionar à campanha do SFDC, Sincronizar com o SFDC) serão desativadas para campanhas filho do programa.

1. Ir para **[!UICONTROL Atividades de marketing]**.

   ![](assets/login-marketing-activities-1.png)

1. Selecione seu programa.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Clique em **[!UICONTROL Ações do programa]** e selecione **[!UICONTROL Sincronização de campanha do Salesforce]**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Selecionar **[!UICONTROL Criar novo]** ou escolha uma campanha existente do Salesforce.

   >[!TIP]
   >
   >Se você selecionar uma campanha existente do Salesforce, certifique-se de [combinar os status do programa da campanha do Salesforce e do programa Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. Insira um nome para a nova campanha e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Agora é possível verificar os detalhes da sincronização da campanha na página de resumo do programa.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Excelente! Agora, qualquer alteração no status do programa no Marketo é sincronizada com a campanha do SFDC e vice-versa.
