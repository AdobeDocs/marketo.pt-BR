---
unique-page-id: 7504923
description: Definir conversões do Google AdWords no modelo de receita com uma conta de gerente - Marketo Docs - Documentação do produto
title: Definir conversões do Google AdWords no modelo de receita com uma conta de gerente
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Definir conversões do Google AdWords no modelo de receita com uma conta de gerente {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Vincule sua conta do Google AdWords ao Marketo para carregar automaticamente dados de conversão offline do Marketo para o Google AdWords. Em seguida, na interface do usuário do AdWords, você poderá ver facilmente quais cliques resultaram em clientes potenciais qualificados, oportunidades e novos clientes (ou quaisquer estágios de receita que deseja rastrear) depois de clicar [adicionar colunas personalizadas](https://support.google.com/adwords/answer/3073556) no AdWords.

Se você tiver várias contas do Google Adwords, poderá usar um [Conta do gerenciador do Google AdWords](https://www.google.com/adwords/manager-accounts/) (anteriormente conhecido como My Client Center) para integrá-los ao Marketo.

Você pode mapear conversões offline do AdWords para um ou mais estágios em um modelo de Receita. Há duas maneiras:

* Ação de preparo
* Mapeamento do AdWords

>[!PREREQUISITES]
>
>[Adicionar o Google AdWords como um serviço de ponto de partida com uma conta de gerente](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Usar ação de preparo {#use-stage-action}

Mapeie uma conversão do AdWords em Ações de preparo.

1. Selecione a etapa que deseja mapear para uma conversão do AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. No **Ações de preparo** selecione **Definir a conversão do AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Defina um **Conversão do AdWords**.

   >[!NOTE]
   >
   >Uma conversão diferente do AdWords pode ser selecionada para cada conta de criança.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Dica: se você não tiver nenhuma conversão do AdWords, crie uma clicando em **+Nova conversão**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Clique em **Salvar**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

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

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. Insira um **Nome da conversão**. Clique em **Salvar**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   Excelente! Essa nova conversão aparecerá na sua conta do AdWords.

## Usar o mapeamento do AdWords {#use-adwords-mapping}

Você pode associar todos os estágios de modelo à sua Conversão do AdWords em um único local usando os Mapeamentos do AdWords.

1. Selecionar **Editar mapeamentos do AdWords**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Selecione o desejado **Conta do AdWords** e desejada **Conversão do AdWords** para cada estágio que você deseja rastrear.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Depois de mapear os estágios, clique em **Salvar**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Depois de concluir o mapeamento de todas as conversões do AdWords em estágios de receita, volte para a página de resumo. Selecionar **Ações do modelo** e escolha **Aprovar estágios**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Para visualizar os dados de conversão offline, você precisará fazer logon em sua conta do AdWords. Recomendamos que você use a [Recurso Colunas personalizadas](https://support.google.com/adwords/answer/3073556) para criar colunas de contagem de conversão para cada conversão offline importada do Marketo.
