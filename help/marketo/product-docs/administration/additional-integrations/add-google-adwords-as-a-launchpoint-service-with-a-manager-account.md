---
unique-page-id: 7504893
description: Integre várias contas do  [!DNL Google AdWords]  com a Marketo usando uma Conta de Gerente no LaunchPoint.
title: Adicionar [!DNL Google AdWords] como um [!DNL Launchpoint] Serviço com uma Conta de Gerente
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
feature: Administration, Integrations
TQID: https://experienceleague.adobe.com/fQYFZRLEULbnvJnYh1Yp9ziGIz1KPYwUPSqeo5Et63Y
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 309
ht-degree: 2%

---

# Adicionar [!DNL Google AdWords] como um Serviço [!DNL Launchpoint] com uma Conta de Gerente {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Vincule sua conta do [!DNL Google AdWords] ao Marketo para carregar automaticamente dados de conversão offline do Marketo para o [!DNL Google AdWords]. Na interface do usuário do [!DNL AdWords], você pode ver quais cliques resultaram em clientes potenciais qualificados, oportunidades e novos clientes (ou qualquer estágio de receita que você queira rastrear) depois de [adicionar colunas personalizadas](https://support.google.com/adwords/answer/3073556){target="_blank"} em [!DNL AdWords]. Essas informações não aparecem na interface do usuário do Marketo.

Se você tiver várias contas do [!DNL Google Adwords], poderá usar um [[!DNL Google AdWords Manager Account]](https://www.google.com/adwords/manager-accounts/){target="_blank"} (conhecido anteriormente como [!DNL My Client Center]) para integrá-las ao Marketo.

Saiba mais sobre o [recurso de importação de conversão offline do Google](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>Nem todos os usuários do Marketo Engage compraram essa funcionalidade. Entre em contato com a equipe de conta da Adobe (seu gerente de conta) para obter mais detalhes.

>[!NOTE]
>
>**Permissões de administrador são necessárias**

>[!NOTE]
>
>Você também pode integrar uma conta [independente [!DNL Google AdWords] como um [!DNL Launchpoint] serviço](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md){target="_blank"}.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-1.png)

1. Selecione **[!UICONTROL LaunchPoint]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-2.png)

1. Clique no menu suspenso **[!UICONTROL Novo]** e selecione **[!UICONTROL Novo serviço]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-3.png)

1. Insira um **[!UICONTROL Nome para Exibição]** e selecione **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-4.png)

1. Selecione **[!UICONTROL Autorizar Marketo]**.

   >[!NOTE]
   >
   >Saia da sua conta pessoal do [!DNL Gmail] e habilite pop-ups.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-5.png)

1. Selecione sua conta associada a **[!DNL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-6.png)

1. Clique em **[!UICONTROL Aceitar]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-7.png)

1. O status é exibido como **[!UICONTROL Sucesso]**. Selecione **[!UICONTROL Próximo]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-8.png)

1. Carregue suas conversões offline do Marketo para o [!DNL Google AdWords] **[!UICONTROL Semanalmente]** ou **[!UICONTROL Diariamente]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-9.png)

1. Conversão de atributo para **[!UICONTROL Primeiro clique]** ou **[!UICONTROL Último clique]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-10.png)

   | Tipo | Definição |
   |---|---|
   | [!UICONTROL Primeiro clique] | As conversões offline serão atribuídas ao primeiro [!DNL AdWords] e que uma pessoa clicou nos últimos 90 dias |
   | [!UICONTROL Último clique] | As conversões offline serão atribuídas aos últimos [!DNL AdWords] e que uma pessoa clicou |

   >[!NOTE]
   >
   >[A marcação automática](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} deve ser selecionada para que este recurso funcione. Deve ser ativado dentro de [!DNL AdWords].

1. Clique em **[!UICONTROL Next]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-11.png)

1. Desmarque as contas que você não quer atualizar. Clique em **[!UICONTROL Criar]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-12.png)

   Consulte o Artigo Relacionado abaixo para saber como mapear [!DNL AdWords] conversões offline no seu modelo de receita.
