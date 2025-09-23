---
unique-page-id: 2359418
description: Importar uma lista de pessoas - Documentos do Marketo - Documentação do produto
title: Importar uma lista de pessoas
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 100%

---

# Importar uma lista de pessoas {#import-a-list-of-people}

## Missão: importar a lista de uma planilha de participantes de um evento comercial para seu banco de dados {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Configurar e adicionar uma pessoa](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}

Neste tutorial, saiba como importar pessoas de um arquivo de planilha para o Marketo.

## Etapa 1: baixar e editar uma planilha {#step-download-and-edit-a-spreadsheet}

1. Para começar, baixe nosso arquivo de planilha de prática ([**tradeshow-attendees.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target="_blank"}) no seu computador.

   ![](assets/import-a-list-of-people-1.png)

   >[!NOTE]
   >
   >Ao importar uma data, use este formato: **21/9/20** (Dia/Mês/Ano).

   >[!NOTE]
   >
   >Qualquer campo de data/hora importado será tratado como Horário central. Se você tiver campos de data/hora em um fuso horário diferente, poderá usar uma fórmula do Excel para convertê-los para o Horário central (América/Chicago).

1. Adicione seu próprio nome, sobrenome, endereço de email real (para receber os emails de incentivo que enviará na próxima missão) e cargo. Salve o arquivo no computador.

   ![](assets/import-a-list-of-people-2.png)

   >[!CAUTION]
   >
   >* Verifique se os endereços de email contêm apenas caracteres ASCII.
   >
   >* O Marketo **não** permite o uso de endereços de email com emojis.
   >
   >* A importação de valores `NULL` por meio de um CSV pode gerar uma “Alteração de valor dos dados” para campos numéricos no [log de atividades](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md){target="_blank"} de uma pessoa, _mesmo que os campos já estejam em branco_. Se você tiver [campanhas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md){target="_blank"} que usam o filtro “Valor de dados alterado” ou o acionador “Alterações no valor dos dados”, isso poderá fazer com que as pessoas se qualifiquem para essas campanhas, mesmo que os dados não estejam realmente mudando. Você pode usar [restrições](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"} para garantir que ninguém se qualifique para essas campanhas após a importação.

## Etapa 2: criar um programa {#step-create-a-program}

1. Acesse a área **[!UICONTROL Atividades de marketing]**.

   ![](assets/import-a-list-of-people-3.png)

1. Selecione a pasta **Aprendizado** e, em **[!UICONTROL Novo]**, clique em **[!UICONTROL Novo programa]**.

   ![](assets/import-a-list-of-people-4.png)

1. **Nomeie** o programa como “Meu programa de feira de negócios” e selecione “Evento” como o **[!UICONTROL Tipo de programa]**.

   ![](assets/import-a-list-of-people-5.png)

1. Selecione **[!UICONTROL Feira de negócios]** como o **[!UICONTROL Canal]** e clique em **[!UICONTROL Criar]**.

   ![](assets/import-a-list-of-people-6.png)

>[!NOTE]
>
>Os programas de eventos ocorrem em datas específicas. Saiba mais sobre [**Eventos**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target="_blank"}.

## Etapa 3: importar sua planilha para o Marketo {#step-import-your-spreadsheet-into-marketo}

1. Em **Meu programa de feira de negócios**, clique em **[!UICONTROL Novo]** e selecione **[!UICONTROL Novo ativo local]**.

   ![](assets/import-a-list-of-people-7.png)

1. Selecione **[!UICONTROL Lista]**.

   ![](assets/import-a-list-of-people-8.png)

1. **Nomeie** a lista como “Participantes da feira de negócios” e clique em **[!UICONTROL Criar]**.

   ![](assets/import-a-list-of-people-9.png)

1. Na lista de **[!UICONTROL Participantes da feira de negócios]**, clique em **[!UICONTROL Ações da lista]** e selecione **[!UICONTROL Importar lista]**.

   ![](assets/import-a-list-of-people-10.png)

   >[!CAUTION]
   >
   >Se você estiver usando seu próprio arquivo CSV, verifique se ele está codificado como UTF-8, UTF-16, Shift-JIS ou EUC-JP.

   >[!NOTE]
   >
   >O limite de tamanho para arquivos CSV é 100 MB.

1. **[!UICONTROL Navegue]** até o arquivo de planilha **tradeshow-attendees.csv** no seu computador e clique em **[!UICONTROL Avançar]**.

   ![](assets/import-a-list-of-people-11.png)

   >[!NOTE]
   >
   >No Modo de importação de lista, escolher **[!UICONTROL Ignorar novas pessoas e atualizações]** significa que você não afetará os registros de pessoas existentes nem registrará atividades. Use esse modo se desejar uma lista estática rápida e pré-filtrada das pessoas existentes para usar em suas atividades de marketing. Selecionar este modo:
   >
   > * Ignora a criação de uma nova pessoa
   > * Ignora atualizações de campos de pessoas
   > * Ignora o registro de atividades

1. Mapeie os campos de [!UICONTROL Coluna da lista] de acordo com o respectivo campo do Marketo e clique em **[!UICONTROL Avançar]**.

   ![](assets/import-a-list-of-people-12.png)

   >[!TIP]
   >
   >Os cabeçalhos de coluna devem sempre corresponder exatamente ao campo (maiúsculas de minúsculas são diferenciadas) para obter os melhores resultados de mapeamento automático. Se você estiver usando campos personalizados e não encontrá-los na lista suspensa, volte e [crie-os](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"} para disponibilizá-los como opções.

   >[!NOTE]
   >
   >Se houver campos que você não queira importar, selecione **Ignorar** no menu suspenso Campo do Marketo.

1. Selecione **Meu programa de feira de negócios** como o **[!UICONTROL Programa de aquisição]** e clique em **[!UICONTROL Importar]**.

   ![](assets/import-a-list-of-people-13.png)

1. Aguarde a importação das pessoas e feche o pop-up de andamento da importação.

   ![](assets/import-a-list-of-people-14.png)

1. De volta ao **Meu programa de feira de negócios**, clique na guia **[!UICONTROL Membros]**. Você verá todas as pessoas que acabou de importar.

   ![](assets/import-a-list-of-people-15.png)

>[!NOTE]
>
>Para analisar o sucesso de seu programa, acompanhe os membros associados. Saiba mais sobre [**Programas**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}.

## Missão cumprida {#mission-complete}

Agora os participantes de seu evento comercial são membros de seu programa do Marketo!

<br> 

[◄ Missão 4: resposta automática de email](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Missão 6: estímulo gota a gota ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
