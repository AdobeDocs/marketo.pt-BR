---
unique-page-id: 1147154
description: Sincronizar uma campanha SFDC com um programa - Documentos do Marketo - Documentação do produto
title: Sincronizar uma campanha SFDC com um programa
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
source-git-commit: 8781c6cf2e64543809fe697e75ae6884969a4e40
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 1%

---

# Sincronizar uma campanha SFDC com um programa {#sync-an-sfdc-campaign-with-a-program}

O Marketo permite sincronizar seus programas com campanhas do Salesforce para manter a mesma lista de pessoas em ambos os sistemas, incluindo seus status. Vamos começar? 

>[!PREREQUISITES]
>
>Você precisará [ativar a sincronização de campanha do Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) primeiro.

>[!CAUTION]
>
>Ao sincronizar uma campanha SFDC com um programa Marketo, as ações SFDC implícitas (por exemplo, adicionar à campanha SFDC, Sincronizar para SFDC) serão desativadas para campanhas filho do programa.

1. Vá para **Marketing Activities**.

   ![](assets/login-marketing-activities-1.png)

1. Selecione o programa.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Clique em **Program Actions** e selecione **Salesforce Campaign Sync**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Selecione **Criar novo** ou escolha uma campanha Salesforce existente.

   >[!TIP]
   >
   >Se você selecionar uma campanha Salesforce existente, certifique-se de [corresponder aos status do programa da campanha Salesforce e do programa Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. Insira um nome para a nova campanha e clique em **Save**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Agora você pode verificar os detalhes de sincronização da campanha na página de resumo do programa.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Excelente! Agora, todas as alterações de status do programa no Marketo são sincronizadas com a campanha SFDC e vice-versa.
