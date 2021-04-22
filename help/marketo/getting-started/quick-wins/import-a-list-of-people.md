---
unique-page-id: 2359418
description: Importar uma lista de pessoas - Documentos do Marketo - Documentação do produto
title: Importar uma lista de pessoas
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 19%

---

# Importar uma Lista de Pessoas {#import-a-list-of-people}

## Missão: importar a lista de uma planilha de participantes de um evento comercial para seu banco de dados {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Configurar e adicionar uma pessoa](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

Neste tutorial, você aprenderá a importar pessoas de um arquivo de planilha para o Marketo.

## Etapa 1: baixar e editar uma planilha {#step-download-and-edit-a-spreadsheet}

1. Para iniciar, baixe nosso arquivo de planilha de práticas ([**tradeshow-atenudees.csv**](https://docs.marketo.com/display/docs/assets/tradeshow-attendees.csv)) no seu computador.

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >Ao importar uma data, use este formato: **9/21/20** (Mês/Dia/Ano).

   >[!NOTE]
   >
   >Todos os campos de data/hora que estão sendo importados são tratados como Hora central. Se você tiver campos de data/hora em um fuso horário diferente, poderá usar uma fórmula do Excel para transformá-la em Hora Central (América/Chicago).

1. Adicione seu nome, sobrenome, endereço de e-mail e cargo e, em seguida, salve o arquivo em seu computador.

   ![](assets/image2014-9-24-12-3a5-3a30.png)

>[!NOTE]
>
>Insira seu endereço de email real no arquivo CSV para que você possa receber os emails de preparação que enviará na próxima missão.

## Etapa 2: &#x200B;criar um programa {#step-create-a-program}

1. Vá para a área **Marketing Activities**.

   ![](assets/ma-2.png)

1. Selecione a pasta **Aprendizagem** e, em **Novo** clique em **Novo Programa**.

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **** Nomeie o programa como &quot;Meu programa de shows de vendas&quot; e selecione &quot;Evento&quot; para o tipo de  **programa**.

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. Selecione **Transmissão** para o **Canal** e clique em **Criar**.

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>Os programas de eventos ocorrem em datas específicas. Saiba mais sobre [**Eventos**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md).

## Etapa 3: importar sua planilha para o Marketo {#step-import-your-spreadsheet-into-marketo}

1. Em **Meu Programa de Apresentação de Marcas**, clique em **Novo** e selecione **Novo Ativo Local**.

   ![](assets/seven-3.png)

1. Clique em **List**.

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **** Nomeie a lista como &quot;Participantes de shows de vendas&quot; e clique em  **Criar**.

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. Em sua lista **Participantes de shows de vendas**, clique em **Listar ações** e selecione **Importar lista**.

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >Se você estiver usando seu próprio arquivo CSV, verifique se ele está codificado em UTF-8, UTF-16, Shift-JIS ou EUC-JP.

   >[!NOTE]
   >
   >O limite de tamanho para arquivos CSV é de 100 MB.

1. **** Navegue até o arquivo  **tradeshow-ants.** csvspreadsheet no seu computador e clique em  **Next**.

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >No Modo de importação de lista, escolher **Ignorar novas pessoas e atualizações** significa que você não afetará os registros de pessoas existentes ou registrará quaisquer atividades. Use esse modo se desejar uma lista estática rápida e pré-filtrada de pessoas existentes para uso em suas atividades de marketing. Selecionar este modo irá:
   >
   > * Ignorar a criação de nova pessoa
   > * Ignorar atualizações de campos de pessoas
   > * Ignorar registro de atividade


1. Mapeie os campos de Coluna de lista para o respectivo Campo Marketo e clique em **Próximo**.

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >Os cabeçalhos de coluna devem sempre corresponder exatamente ao campo (diferencia maiúsculas de minúsculas) para obter os melhores resultados de mapeamento automático. Se você estiver usando campos personalizados e não os vir no menu suspenso, volte e [crie-os](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) para que possam se tornar opções.

   >[!NOTE]
   >
   >Se houver campos que não deseja importar, selecione **Ignorar** no menu suspenso Campo do Marketo.

1. Selecione **My Tradeshow Program** para o **Acquisition Program** e clique em **Import**.

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. Aguarde a importação das pessoas e feche a janela pop-up de progresso da importação.

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. De volta a **My Tradeshow Program**, clique na guia **Members**. Você verá todas as pessoas que acabou de importar.

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>Para analisar o sucesso de seu programa, acompanhe os membros a ele associados. Saiba mais sobre [**Programas**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md).

## Missão cumprida {#mission-complete}

Agora os participantes de seu evento comercial são membros de seu programa do Marketo!

<br> 

[◄ Missão 4: resposta automática por e-mail](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Missão 6: promoção gota a gota ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
