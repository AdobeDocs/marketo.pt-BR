---
unique-page-id: 6095029
description: Definir  [!DNL Google AdWords] Conversões no Modelo de receita - Documentação do Marketo - Documentação do produto
title: Definir [!DNL Google AdWords] Conversões no Modelo de Receita
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# Definir [!DNL Google AdWords] conversões no modelo de receita {#set-google-adwords-conversions-in-the-revenue-model}

Vincule sua conta do [!DNL Google AdWords] ao Marketo para carregar automaticamente dados de conversão offline do Marketo para o [!DNL Google AdWords]. Na interface do usuário do [!DNL AdWords], você poderá ver facilmente quais cliques resultaram em clientes potenciais qualificados, oportunidades e novos clientes (ou quaisquer estágios de receita que você queira rastrear) depois de [adicionar colunas personalizadas](https://support.google.com/adwords/answer/3073556) no [!DNL AdWords].

>[!NOTE]
>
>Esta é uma integração por push do Marketo para [!DNL Google AdWords]. Os dados de conversão aparecerão _somente_ no portal [!DNL Google AdWords], _não na interface do usuário do Marketo_.

Saiba mais sobre o [recurso de importação de conversão offline do Google](https://support.google.com/adwords/answer/2998031?hl=en). Mapeie [!DNL AdWords] conversões offline para um ou mais estágios em um modelo de Receita. Há três maneiras de fazer o mapeamento:

* Conversão de [!DNL AdWords]
* Ação de preparo
* Mapeamento de [!DNL AdWords]

Você pode criar uma nova conversão offline de [!DNL AdWords] no Marketo se usar a Ação de preparo.

>[!PREREQUISITES]
>
>[Adicionar [!DNL Google AdWords] como um Serviço do LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## Usar Conversão [!DNL AdWords] {#use-adwords-conversion}

1. Vá para a área **[!UICONTROL Analytics]**.

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Selecione um modelo.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Clique em **[!UICONTROL Editar rascunho]**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Selecione o estágio de receita que você deseja mapear para uma conversão de [!DNL AdWords].

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Selecione a **[!UICONTROL Conversão do AdWords]** que você deseja mapear para o estágio do Marketo.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   Legal! Os dados de conversão do [!DNL AdWords] serão carregados no [!DNL Google AdWords] na cadência selecionada.

## Usar ação de preparo {#use-stage-action}

Você também pode mapear uma [!UICONTROL Conversão do AdWords] em **[!UICONTROL Ações de Preparo]**.

1. Selecione a etapa que deseja mapear para uma conversão de [!DNL AdWords].

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. No menu suspenso **[!UICONTROL Ações de Preparo]**, selecione **[!UICONTROL Definir Conversão do AdWords]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Selecione uma **[!UICONTROL Conversão do AdWords]**.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Dica**: se você não tiver nenhuma conversão de [!DNL AdWords], crie uma clicando em **[!UICONTROL +Nova Conversão]**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. Depois de concluir o mapeamento de todas as conversões do [!DNL AdWords] para estágios de receita, volte para a página de resumo. Selecione **[!UICONTROL Ações de Modelo]** e escolha **[!UICONTROL Aprovar Estágios]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Dica profissional: adicionar uma nova conversão {#pro-tip-add-a-new-conversion}

Dica profissional! Uma nova conversão offline de [!DNL AdWords] pode ser criada no Marketo.

>[!CAUTION]
>
>As novas conversões criadas no Marketo têm a configuração de &quot;otimização&quot; ativada. Isso significa que [!DNL AdWords] estratégias de oferta têm permissão para otimizar suas ofertas para essas conversões. Você pode alterar esta configuração da sua conta [!DNL AdWords].

1. No menu suspenso **[!UICONTROL Ações de Preparo]**, selecione **[!UICONTROL Definir Conversão do AdWords]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Selecione **[!UICONTROL Nova Conversão]**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Insira um **[!UICONTROL Nome de Conversão]**. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   Excelente! Esta nova conversão aparecerá na sua conta [!DNL AdWords].

## Usar Mapeamento [!DNL AdWords] {#use-adwords-mapping}

Você pode associar todos os estágios de modelo à [!UICONTROL Conversão do AdWords] em um único local usando os Mapeamentos do [!DNL AdWords].

1. Selecione **[!UICONTROL Editar mapeamentos do AdWords]**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Selecione a **[!UICONTROL Conversão do AdWords]** desejada para cada estágio que você deseja rastrear.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Depois de mapear seus estágios, clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Depois de concluir o mapeamento de todas as conversões do [!DNL AdWords] para estágios de receita, volte para a página de resumo. Selecione **[!UICONTROL Ações de Modelo]** e escolha **[!UICONTROL Aprovar Estágios]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Para exibir os dados de conversão offline, você precisará fazer logon em sua conta do [!DNL AdWords]. Recomendamos que você use o [recurso Colunas personalizadas](https://support.google.com/adwords/answer/3073556) para criar colunas de contagem de conversão para cada conversão offline importada do Marketo.
