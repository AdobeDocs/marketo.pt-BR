---
unique-page-id: 6095008
description: "Adicionar [!DNL Google AdWords] as a [!DNL LaunchPoint] Serviço - Documentação do Marketo - Documentação do produto"
title: "Adicionar [!DNL Google AdWords] as a [!DNL LaunchPoint] Serviço"
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
feature: Administration, Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 3%

---

# Adicionar [!DNL Google AdWords] as a [!DNL LaunchPoint] Serviço {#add-google-adwords-as-a-launchpoint-service}

Vincule seu [!DNL Google AdWords] para o Marketo para carregar automaticamente dados de conversão offline do Marketo para o [!DNL Google AdWords]. Em seguida, do [!DNL AdWords] Interface do usuário do, você poderá ver facilmente quais cliques resultaram em clientes potenciais qualificados, oportunidades e novos clientes (ou quaisquer estágios de receita que deseja rastrear) depois de você [adicionar colunas personalizadas](https://support.google.com/adwords/answer/3073556){target="_blank"} in [!DNL AdWords]. Essas informações não aparecem na interface do usuário do Marketo.

Saiba mais sobre [Recurso de importação de conversão offline do Google](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>Nem todos os usuários do Marketo Engage compraram essa funcionalidade. Entre em contato com a equipe de conta do Adobe (seu gerente de conta) para obter mais detalhes.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>Também é possível integrar um [[!DNL Google AdWords] as a [!DNL Launchpoint] serviço com uma conta de gerente](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md){target="_blank"}.

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/add-google-adwords-as-a-launchpoint-service-1.png)

1. Selecionar **[!UICONTROL LaunchPoint]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-2.png)

1. Selecionar **[!UICONTROL Novo]** e **[!UICONTROL Novo serviço]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-3.png)

1. Insira um [!UICONTROL nome de exibição] e selecione **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-4.png)

1. Selecionar **[!UICONTROL Autorizar Marketo]**.

   >[!NOTE]
   >
   >Não se esqueça de fazer logoff do seu pessoal [!DNL Gmail] conta e ativar pop-ups.

   ![](assets/add-google-adwords-as-a-launchpoint-service-5.png)

1. Selecione sua conta associada ao [!DNL Google AdWords].

   ![](assets/add-google-adwords-as-a-launchpoint-service-6.png)

1. Selecionar **[!UICONTROL Aceitar]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-7.png)

1. O status será exibido como **[!UICONTROL Sucesso]**. Selecionar **[!UICONTROL Próxima]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-8.png)

1. Fazer upload das conversões offline do Marketo para [!DNL Google AdWords] **[!UICONTROL Semanalmente]** ou **[!UICONTROL Diariamente]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-9.png)

1. Conversão de atributo para o **[!UICONTROL Primeiro clique]** ou **[!UICONTROL Último clique]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-10.png)

   | Tipo | Definição |
   |---|---|
   | [!UICONTROL Primeiro clique] | As conversões offline serão atribuídas à primeira [!DNL AdWords] anúncio em que uma pessoa clicou nos últimos 90 dias |
   | [!UICONTROL Último clique] | As conversões offline serão atribuídas ao último [!DNL AdWords] anúncio em que uma pessoa clicou |

   >[!NOTE]
   >
   >Uso de um modelo de atribuição consistente no Marketo e [!DNL AdWords] O fornece os dados mais precisos.

1. Clique em **[!UICONTROL Criar]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-11.png)

   >[!NOTE]
   >
   >[Marcação automática](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} deve ser selecionado para que este recurso funcione. A desativação deve ser feita dentro de [!DNL AdWords].

Ótimo! Agora veja o Artigo Relacionado abaixo para saber como mapear [!DNL AdWords] conversões offline no seu modelo de receita.

>[!MORELIKETHIS]
>
>[Definir [!DNL Google AdWords] Conversões no modelo de receita](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md){target="_blank"}
