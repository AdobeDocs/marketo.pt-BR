---
unique-page-id: 7504923
description: Definir [!DNL Google AdWords] Conversões no Modelo de Receita com uma Conta de Gerente - Marketo Docs - Documentação do Produto
title: Definir [!DNL Google AdWords] Conversões no Modelo de Receita com uma Conta de Gerente
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Definir [!DNL Google AdWords] conversões no modelo de receita com uma conta de gerente {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Vincule sua conta do [!DNL Google AdWords] ao Marketo para carregar automaticamente dados de conversão offline do Marketo para o [!DNL Google AdWords]. Na interface do usuário do [!DNL AdWords], você poderá ver facilmente quais cliques resultaram em clientes potenciais qualificados, oportunidades e novos clientes (ou quaisquer estágios de receita que você queira rastrear) depois de [adicionar colunas personalizadas](https://support.google.com/adwords/answer/3073556) no [!DNL AdWords].

Se você tiver várias contas do [!DNL Google Adwords], poderá usar uma [[!DNL Google AdWords] Conta de Gerente](https://www.google.com/adwords/manager-accounts/) (antes conhecida como Meu Centro de Clientes) para integrá-las ao Marketo.

Você pode mapear [!DNL AdWords] conversões offline para um ou mais estágios em um modelo de Receita. Há duas maneiras:

* Ação de preparo
* Mapeamento de [!DNL AdWords]

>[!PREREQUISITES]
>
>[Adicionar [!DNL Google AdWords] como um Serviço de Ponto de Inicialização com uma Conta de Gerente](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Usar ação de preparo {#use-stage-action}

Mapeie uma Conversão [!DNL AdWords] em Ações de preparo.

1. Selecione a etapa que deseja mapear para uma conversão de [!DNL AdWords].

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. No menu suspenso **[!UICONTROL Ações de Preparo]**, selecione **[!UICONTROL Definir Conversão do AdWords]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Defina uma **[!DNL AdWords]Conversão**.

   >[!NOTE]
   >
   >Uma conversão [!DNL AdWords] diferente pode ser selecionada para cada conta de criança.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Dica: se você não tiver nenhuma conversão de [!DNL AdWords], crie uma clicando em **[!UICONTROL +Nova conversão]**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

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

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. Insira um **Nome de Conversão**. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   Excelente! Esta nova conversão aparecerá na sua conta [!DNL AdWords].

## Usar Mapeamento [!DNL AdWords] {#use-adwords-mapping}

Você pode associar todos os estágios de modelo à sua Conversão do [!DNL AdWords] em um único local usando os Mapeamentos do [!DNL AdWords].

1. Selecione **[!UICONTROL Editar mapeamentos do AdWords]**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Selecione a **[!DNL AdWords]Conta** desejada e a **[!DNL AdWords]Conversão** desejada para cada estágio que você deseja rastrear.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Depois de mapear seus estágios, clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Depois de concluir o mapeamento de todas as conversões do [!DNL AdWords] para estágios de receita, volte para a página de resumo. Selecione **[!UICONTROL Ações de Modelo]** e escolha **[!UICONTROL Aprovar Estágios]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Para exibir os dados de conversão offline, você precisará fazer logon em sua conta do [!DNL AdWords]. Recomendamos que você use o [recurso Colunas personalizadas](https://support.google.com/adwords/answer/3073556) para criar colunas de contagem de conversão para cada conversão offline importada do Marketo.
