---
unique-page-id: 1147154
description: Sincronizar uma campanha do SFDC com um programa - Documentação do Marketo - Documentação do produto
title: Sincronizar uma campanha do SFDC com um programa
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 9%

---

# Sincronizar uma campanha do SFDC com um programa {#sync-an-sfdc-campaign-with-a-program}

O Marketo Engage permite sincronizar seus programas com as campanhas do [!DNL Salesforce] para manter a mesma lista de pessoas nos dois sistemas, incluindo seus status. Vamos começar!

>[!PREREQUISITES]
>
>Você precisará [habilitar [!DNL Salesforce] sincronização de campanha](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"} primeiro.

>[!CAUTION]
>
>Ao sincronizar uma campanha do SFDC com um programa do Marketo Engage, as ações implícitas do SFDC (por exemplo, adicionar ao SFDC Campaign, Sincronizar com o SFDC) serão desativadas para campanhas filho do programa.

1. Vá para **[!UICONTROL Atividades de marketing]**.

   ![](assets/login-marketing-activities-1.png)

1. Selecione seu programa.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Clique em **[!UICONTROL Ações do Programa]** e selecione **[!UICONTROL Sincronização do Salesforce Campaign]**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Selecione **[!UICONTROL Criar novo]** ou escolha uma campanha [!DNL Salesforce] existente.

   >[!TIP]
   >
   >Se você selecionar uma campanha [!DNL Salesforce] existente, certifique-se de [corresponder aos status dos programas da [!DNL Salesforce] campanha e do programa Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}.

1. Insira um nome para a nova campanha e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Agora é possível verificar os detalhes da sincronização da campanha na página de resumo do programa.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Excelente! Agora, todas as alterações de status do programa no Marketo são sincronizadas com a campanha do SFDC e vice-versa.
