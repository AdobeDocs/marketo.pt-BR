---
unique-page-id: 6095029
description: Definir conversões do Google AdWords no modelo de receita - Documentos do marketing - Documentação do produto
title: Definir conversões do Google AdWords no modelo de receita
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---


# Definir conversões do Google AdWords no modelo de receita {#set-google-adwords-conversions-in-the-revenue-model}

Vincule sua conta do Google AdWords ao Marketo para fazer upload automático de dados de conversão offline do Marketo para o Google AdWords. Em seguida, na interface do usuário do AdWords, você poderá ver com facilidade quais cliques resultaram em clientes potenciais qualificados, oportunidades e novos clientes (ou quaisquer estágios de receita que deseja rastrear) depois de [adicionar colunas](https://support.google.com/adwords/answer/3073556) personalizadas no AdWords.

>[!NOTE]
>
>Esta é uma integração de push do Marketo para o Google AdWords. Os dados de conversão aparecerão *somente* no portal do Google AdWords,** não na interface do usuário do Marketing. **

Saiba mais sobre o recurso [de importação de conversão offline do](https://support.google.com/adwords/answer/2998031?hl=en)Google.  Mapeie as conversões offline do AdWords para um ou mais estágios em um modelo de Receita. Há três maneiras de fazer o mapeamento:

* Conversão de AdWords
* Ação de estágio
* Mapeamento de AdWords

Você pode criar uma nova conversão offline AdWords de Marketo se usar a Ação do palco.

>[!NOTE]
>
>**Pré-requisitos**
>
>* [Adicionar Google AdWords como um Serviço LaunchPoint](../../../../product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

>



## Usar conversão do AdWords {#use-adwords-conversion}

1. Vá para a área **do Analytics** .

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Selecione um modelo.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Clique em **Editar rascunho**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Selecione o estágio de receita que deseja mapear para uma conversão do AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Selecione a Conversão **de** AdWords que deseja mapear para o estágio de Marketo.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   Legal! Os dados de conversão do AdWords serão carregados no Google AdWords na cadência selecionada.

## Usar ação de estágio {#use-stage-action}

Você também pode mapear uma Conversão AdWords em Ações do palco.

1. Selecione a etapa que deseja mapear para uma conversão AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Na lista suspensa Ações **do** palco, selecione **Definir conversão** do AdWords.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Selecione uma conversão **AdWords**.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Dica**: Se você não tiver conversões AdWords, crie uma clicando em **+Nova conversão**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Clique em **Salvar**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

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

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Insira um Nome **de conversão**. Clique em **Salvar**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   Excelente! Essa nova conversão aparecerá em sua conta AdWords.

## Usar mapeamento AdWords {#use-adwords-mapping}

Você pode associar todos os estágios do modelo à Conversão do AdWords em um único lugar usando Mapeamentos do AdWords.

1. Selecione **Editar mapeamentos** do AdWords.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Selecione a Conversão **de** AdWords desejada para cada estágio que você deseja rastrear.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Depois de mapear seus estágios, clique em **Salvar**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Após concluir o mapeamento de todas as conversões do AdWords para estágios de receita, volte para a página de resumo. Selecione Ações **** do modelo e escolha **Aprovar etapas**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Para visualização dos dados de conversão offline, você precisará fazer logon em sua conta AdWords. Recomendamos que você use o recurso [Colunas](https://support.google.com/adwords/answer/3073556) personalizadas para criar colunas de contagem de conversão para cada conversão offline importada do Marketo.
