---
unique-page-id: 6095029
description: Definir conversões do Google AdWords no modelo de receita - Documentação do Marketo - Documentação do produto
title: Definir conversões do Google AdWords no modelo de receita
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Definir conversões do Google AdWords no modelo de receita {#set-google-adwords-conversions-in-the-revenue-model}

Vincule sua conta do Google AdWords ao Marketo para carregar automaticamente dados de conversão offline do Marketo para o Google AdWords. Em seguida, na interface do usuário do AdWords, você poderá ver facilmente quais cliques resultaram em clientes potenciais qualificados, oportunidades e novos clientes (ou quaisquer estágios de receita que deseja rastrear) depois de clicar [adicionar colunas personalizadas](https://support.google.com/adwords/answer/3073556) no AdWords.

>[!NOTE]
>
>Esta é uma integração por push do Marketo para o Google AdWords. Os dados de conversão serão exibidos _somente_ no portal Google AdWords, _não na interface do usuário do Marketo_.

Saiba mais sobre [Recurso de importação de conversão offline do Google](https://support.google.com/adwords/answer/2998031?hl=en). Mapeie as conversões offline do AdWords para um ou mais estágios em um modelo de Receita. Há três maneiras de fazer o mapeamento:

* Conversão do AdWords
* Ação de preparo
* Mapeamento do AdWords

Você pode criar uma nova conversão offline do AdWords no Marketo se usar a Ação de preparo.

>[!PREREQUISITES]
>
>[Adicionar o Google AdWords como um serviço LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## Usar a conversão do AdWords {#use-adwords-conversion}

1. Vá para a **Analytics** área.

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Selecione um modelo.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Clique em **Editar rascunho**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Selecione o estágio de receita que deseja mapear para uma conversão do AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Selecione o **Conversão do AdWords** você gostaria de mapear para o estágio do Marketo.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   Legal! Os dados de conversão do AdWords serão carregados no Google AdWords na cadência selecionada.

## Usar ação de preparo {#use-stage-action}

Você também pode mapear uma Conversão do AdWords em Ações de preparo.

1. Selecione a etapa que deseja mapear para uma conversão do AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. No **Ações de preparo** selecione **Definir a conversão do AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Selecione um **Conversão do AdWords**.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Dica**: Se você não tiver nenhuma conversão do AdWords, crie uma clicando em **+Nova conversão**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Clique em **Salvar**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. Depois de concluir o mapeamento de todas as conversões do AdWords em estágios de receita, volte para a página de resumo. Selecionar **Ações do modelo** e escolha **Aprovar estágios**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Dica profissional: adicionar uma nova conversão {#pro-tip-add-a-new-conversion}

Dica profissional! Uma nova conversão offline do AdWords pode ser criada no Marketo.

>[!CAUTION]
>
>As novas conversões criadas no Marketo têm a configuração de &quot;otimização&quot; ativada. Isso significa que as estratégias de oferta do AdWords têm permissão para otimizar suas ofertas para essas conversões. Você pode alterar essa configuração da sua conta do AdWords.

1. No **Ações de preparo** selecione **Definir a conversão do AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Selecionar **Nova conversão**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Insira um **Nome da conversão**. Clique em **Salvar**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   Excelente! Essa nova conversão aparecerá na sua conta do AdWords.

## Usar o mapeamento do AdWords {#use-adwords-mapping}

Você pode associar todos os estágios de modelo à sua Conversão do AdWords em um único local usando os Mapeamentos do AdWords.

1. Selecionar **Editar mapeamentos do AdWords**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Selecione o desejado **Conversão do AdWords** para cada estágio que você deseja rastrear.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Depois de mapear os estágios, clique em **Salvar**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Depois de concluir o mapeamento de todas as conversões do AdWords em estágios de receita, volte para a página de resumo. Selecionar **Ações do modelo** e escolha **Aprovar estágios**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Para visualizar os dados de conversão offline, você precisará fazer logon em sua conta do AdWords. Recomendamos que você use a [Recurso Colunas personalizadas](https://support.google.com/adwords/answer/3073556) para criar colunas de contagem de conversão para cada conversão offline importada do Marketo.
