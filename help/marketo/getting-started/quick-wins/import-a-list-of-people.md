---
unique-page-id: 2359418
description: Importar uma lista de pessoas - Documentação do Marketo - Documentação do produto
title: Importar uma lista de pessoas
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 15%

---

# Importar uma lista de pessoas {#import-a-list-of-people}

## Missão: importar a lista de uma planilha de participantes de um evento comercial para seu banco de dados {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Configurar e adicionar uma pessoa](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}

Neste tutorial, você aprenderá a importar pessoas de um arquivo de planilha para o Marketo.

## Etapa 1: baixar e editar uma planilha {#step-download-and-edit-a-spreadsheet}

1. Para iniciar, baixe nosso arquivo de planilha de práticas ([**tradeshow-attendees.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target="_blank"}) ao seu computador.

   ![](assets/import-a-list-of-people-1.png)

   >[!NOTE]
   >
   >Ao importar uma data, use este formato: **21/09/20** (Mês/Dia/Ano).

   >[!NOTE]
   >
   >Qualquer campo de data/hora que for importado será tratado como Hora central. Se você tiver campos de data/hora em um fuso horário diferente, poderá usar uma fórmula do Excel para transformá-la na Hora Central (América/Chicago).

1. Adicione seu próprio nome, sobrenome, endereço de email real (para que você possa receber os emails de incentivo que enviará na próxima missão) e cargo. Salve o arquivo no computador.

   ![](assets/import-a-list-of-people-2.png)

   >[!CAUTION]
   >
   >A Marketo faz **não** endereços de email de suporte que contêm emojis.

## Etapa 2: &#x200B;criar um programa {#step-create-a-program}

1. Vá para a **[!UICONTROL Atividades de marketing]** área.

   ![](assets/import-a-list-of-people-3.png)

1. Selecione o **Aprendizado** , em seguida, em **[!UICONTROL Novo]** click **[!UICONTROL Novo programa]**.

   ![](assets/import-a-list-of-people-4.png)

1. **Nome** programa &quot;Meu programa de feiras&quot; e selecione &quot;Evento&quot; para o **[!UICONTROL Tipo de programa]**.

   ![](assets/import-a-list-of-people-5.png)

1. Selecionar **[!UICONTROL Tradeshow]** para o **[!UICONTROL Canal]** e clique em **[!UICONTROL Criar]**.

   ![](assets/import-a-list-of-people-6.png)

>[!NOTE]
>
>Os programas de eventos ocorrem em datas específicas. Saiba mais sobre [**Eventos**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target="_blank"}.

## Etapa 3: importar sua planilha para o Marketo {#step-import-your-spreadsheet-into-marketo}

1. Entrada **Meu programa de feiras**, clique em **[!UICONTROL Novo]** e selecione **[!UICONTROL Novo ativo local]**.

   ![](assets/import-a-list-of-people-7.png)

1. Selecionar **[!UICONTROL Lista]**.

   ![](assets/import-a-list-of-people-8.png)

1. **Nome** listar &quot;Participantes do Tradeshow&quot; e clicar em **[!UICONTROL Criar]**.

   ![](assets/import-a-list-of-people-9.png)

1. No seu **[!UICONTROL Participantes do show]** clique em **[!UICONTROL Ações da lista]** e selecione **[!UICONTROL Importar lista]**.

   ![](assets/import-a-list-of-people-10.png)

   >[!CAUTION]
   >
   >Se você estiver usando seu próprio arquivo CSV, verifique se ele está codificado como UTF-8, UTF-16, Shift-JIS ou EUC-JP.

   >[!NOTE]
   >
   >O limite de tamanho para arquivos CSV é 100 MB.

1. **[!UICONTROL Procurar]** para o **tradeshow-attendees.csv** no computador e clique em **[!UICONTROL Próxima]**.

   ![](assets/import-a-list-of-people-11.png)

   >[!NOTE]
   >
   >No Modo de Importação de Lista, escolhendo **[!UICONTROL Ignorar novas pessoas e atualizações]** significa que você não afetará registros pessoais existentes nem registrará atividades. Use esse modo se desejar uma lista estática rápida e pré-filtrada das pessoas existentes para uso em suas atividades de marketing. Selecionar este modo irá:
   >
   > * Ignorar criação de nova pessoa
   > * Ignorar atualizações de campos de pessoas
   > * Ignorar registro de atividade

1. Mapeie seu [!UICONTROL Coluna da lista] aos respectivos Campos da Marketo e clique em **[!UICONTROL Próxima]**.

   ![](assets/import-a-list-of-people-12.png)

   >[!TIP]
   >
   >Os cabeçalhos de coluna devem sempre corresponder exatamente ao campo (diferencia maiúsculas de minúsculas) para obter os melhores resultados de mapeamento automático. Se você estiver usando campos personalizados e não os vir na lista suspensa, volte e [criar](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"} para que possam se tornar opções.

   >[!NOTE]
   >
   >Se houver campos que você não deseja importar, selecione **Ignorar** no menu suspenso Marketo Field.

1. Selecionar **Meu programa de feiras** para o **[!UICONTROL Programa de aquisição]** e, em seguida, clique em **[!UICONTROL Importar]**.

   ![](assets/import-a-list-of-people-13.png)

1. Aguarde até que seus funcionários importem e feche a janela pop-up de progresso da importação.

   ![](assets/import-a-list-of-people-14.png)

1. Voltar para **Meu programa de feiras**, clique no link **[!UICONTROL Membros]** guia. Você verá todas as pessoas que acabou de importar.

   ![](assets/import-a-list-of-people-15.png)

>[!NOTE]
>
>Para analisar o sucesso de seu programa, acompanhe os membros a ele associados. Saiba mais sobre [**Programas**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}.

## Missão cumprida {#mission-complete}

Agora os participantes de seu evento comercial são membros de seu programa do Marketo!

<br> 

[◄ Missão 4: resposta automática por e-mail](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Missão 6: promoção gota a gota ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
