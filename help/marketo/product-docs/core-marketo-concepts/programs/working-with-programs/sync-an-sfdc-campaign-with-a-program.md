---
unique-page-id: 1147154
description: Sincronizar uma Campanha SFDC com um Programa - Documentos do Marketing - Documentação do produto
title: Sincronizar uma Campanha SFDC com um Programa
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Sincronizar uma Campanha SFDC com um Programa {#sync-an-sfdc-campaign-with-a-program}

O Marketo permite sincronizar seus programas com as campanhas do Salesforce para manter a mesma lista de pessoas em ambos os sistemas, incluindo seus status. Vamos começar!

>[!PREREQUISITES]
>
>Será necessário [ativar a sincronização](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) de campanha do Salesforce primeiro.

>[!CAUTION]
>
>Ao sincronizar uma campanha SFDC com um programa Marketo, as ações SFDC implícitas (por exemplo, adicionar à Campanha SFDC, Sincronizar com SFDC) serão desativadas para campanhas filhas do programa.

1. Vá para **Marketing Atividade**.

   ![](assets/login-marketing-activities-1.png)

1. Selecione seu programa.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Clique em Ações **de** Programa e selecione Sincronização **de Campanha do** Salesforce.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Selecione **Criar novo **ou escolha uma campanha existente do Salesforce.

   >[!TIP]
   >
   >Se você selecionar uma campanha Salesforce existente, certifique-se de [corresponder aos status do programa da campanha do Salesforce e do programa](../../../../product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)Marketo.

1. Digite um nome para a nova campanha e clique em **Salvar**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Agora você pode verificar os detalhes da sincronização da campanha na página de resumo do programa.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Excelente! Agora, qualquer alteração no status do programa no Marketo é sincronizada com a campanha SFDC e vice-versa.

