---
unique-page-id: 7504923
description: Definir conversões do Google AdWords no modelo de receita com uma conta do gerente - documentos do marketing - documentação do produto
title: Definir conversões do Google AdWords no modelo de receita com uma conta de gerente
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---


# Definir conversões do Google AdWords no modelo de receita com uma conta de gerente {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Vincule sua conta do Google AdWords ao Marketo para fazer upload automático de dados de conversão offline do Marketo para o Google AdWords. Em seguida, na interface do usuário do AdWords, você poderá ver com facilidade quais cliques resultaram em clientes potenciais qualificados, oportunidades e novos clientes (ou quaisquer estágios de receita que deseja rastrear) depois de [adicionar colunas](https://support.google.com/adwords/answer/3073556) personalizadas no AdWords.

Se você tiver várias contas do Google Adwords, poderá usar uma conta [do](https://www.google.com/adwords/manager-accounts/) Google AdWords Manager (anteriormente conhecida como My Client Center) para integrá-las ao Marketo.

É possível mapear conversões offline do AdWords para uma ou mais etapas em um modelo de Receita. Há duas maneiras:

* Ação de estágio
* Mapeamento de AdWords

>[!PREREQUISITES]
>
>* [Adicionar o Google AdWords como um serviço Launchpoint com uma conta de gerente](../../../../product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

>



## Usar ação de estágio {#use-stage-action}

Mapeie uma conversão AdWords em Ações de estágio.

1. Selecione a etapa que deseja mapear para uma conversão AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Na lista suspensa Ações **do** palco, selecione **Definir conversão** do AdWords.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Defina uma conversão **AdWords**.

   >[!NOTE]
   >
   >Uma conversão AdWords diferente pode ser selecionada para cada conta filho.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Dica: Se você não tiver conversões AdWords, crie uma clicando em **+Nova conversão**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Clique em **Salvar**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

1. Após concluir o mapeamento de todas as conversões do AdWords para estágios de receita, volte para a página de resumo. Selecione Ações **** do modelo e escolha **Aprovar etapas**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Dica do Pro: Adicionar uma nova conversão {#pro-tip-add-a-new-conversion}

Dica profissional! Uma nova conversão offline do AdWords pode ser criada a partir de Marketo.

>[!CAUTION]
>
>Novas conversões criadas no Marketo têm a configuração de &quot;otimização&quot; ativada. Isso significa que as estratégias de lances do AdWords têm permissão para otimizar seus lances para essas conversões. Você pode alterar essa configuração da sua conta AdWords.

1. Na lista suspensa Ações **do** palco, selecione **Definir conversão** do AdWords.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Selecione **Nova conversão**.

   ** ![](assets/image2015-3-27-17-3a23-3a13.png)

   **

1. Insira um Nome **de conversão**. Clique em **Salvar**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   Excelente! Essa nova conversão aparecerá em sua conta AdWords.

## Usar mapeamento AdWords {#use-adwords-mapping}

Você pode associar todos os estágios do modelo à Conversão do AdWords em um único lugar usando Mapeamentos do AdWords.

1. Selecione **Editar mapeamentos** do AdWords.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Selecione a Conta **** AdWords desejada e a Conversão **** AdWords desejada para cada estágio que você deseja rastrear.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Depois de mapear seus estágios, clique em **Salvar**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Após concluir o mapeamento de todas as conversões do AdWords para estágios de receita, volte para a página de resumo. Selecione Ações **** do modelo e escolha **Aprovar etapas**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Para visualização dos dados de conversão offline, você precisará fazer logon em sua conta AdWords. Recomendamos que você use o recurso [Colunas](https://support.google.com/adwords/answer/3073556) personalizadas para criar colunas de contagem de conversão para cada conversão offline importada do Marketo.
