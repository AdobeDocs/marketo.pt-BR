---
unique-page-id: 2359418
description: Importar uma lista de pessoas - Documentos do Marketo - Documentação do produto
title: Importar uma lista de pessoas
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 14%

---

# Importar uma lista de pessoas {#import-a-list-of-people}

## Missão: importar a lista de uma planilha de participantes de um evento comercial para seu banco de dados {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Configurar e adicionar uma pessoa](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}

Neste tutorial, você aprenderá a importar pessoas de um arquivo de planilha para o Marketo.

## Etapa 1: baixar e editar uma planilha {#step-download-and-edit-a-spreadsheet}

1. Para iniciar, baixe nosso arquivo de planilha de práticas ([**tradeshow-ants.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target=&quot;_blank&quot;}) para seu computador.

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >Ao importar uma data, use este formato: **21/9/20** (Mês/Dia/Ano).

   >[!NOTE]
   >
   >Todos os campos de data/hora que estão sendo importados são tratados como Hora central. Se você tiver campos de data/hora em um fuso horário diferente, poderá usar uma fórmula do Excel para transformá-la em Hora Central (América/Chicago).

1. Adicione seu próprio nome, sobrenome, endereço de email real (para que você possa receber os emails de preparação que enviará na próxima missão) e o cargo. Salve o arquivo em seu computador.

   ![](assets/image2014-9-24-12-3a5-3a30.png)

   >[!CAUTION]
   >
   >A Marketo faz **not** são compatíveis com endereços de email que contêm emojis.

## Etapa 2: &#x200B;criar um programa {#step-create-a-program}

1. Vá para o **Atividades de marketing** área.

   ![](assets/ma-2.png)

1. Selecione seu **Aprendizagem** , em seguida, em **Novo** click **Novo programa**.

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **Nome** o programa &quot;Meu programa de feiras&quot; e selecione &quot;Evento&quot; para o **Tipo de programa**.

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. Selecionar **Dosagem** para **Canal** e clique em **Criar**.

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>Os programas de eventos ocorrem em datas específicas. Saiba mais sobre [**Eventos**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target=&quot;_blank&quot;}.

## Etapa 3: importar sua planilha para o Marketo {#step-import-your-spreadsheet-into-marketo}

1. Em **Meu programa de shows de vendas**, clique em **Novo** e selecione **Novo ativo local**.

   ![](assets/seven-3.png)

1. Clique em **Lista**.

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **Nome** na lista &quot;Participantes de shows de vendas&quot; e clique em **Criar**.

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. Em seu **Participantes de shows de vendas** listar, clique em **Ações de lista** e selecione **Importar Lista**.

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >Se você estiver usando seu próprio arquivo CSV, verifique se ele está codificado em UTF-8, UTF-16, Shift-JIS ou EUC-JP.

   >[!NOTE]
   >
   >O limite de tamanho para arquivos CSV é de 100 MB.

1. **Procurar** para **tradeshow-ants.csv** arquivo de planilha no seu computador e clique em **Próximo**.

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >No Modo de Importação de Lista, escolhendo **Ignorar novas pessoas e atualizações** significa que você não afetará os registros de pessoas existentes ou registrará quaisquer atividades. Use esse modo se desejar uma lista estática rápida e pré-filtrada de pessoas existentes para uso em suas atividades de marketing. Selecionar este modo irá:
   >
   > * Ignorar a criação de nova pessoa
   > * Ignorar atualizações de campos de pessoas
   > * Ignorar registro de atividade


1. Mapeie os campos da Coluna de lista para os respectivos campos do Marketo e clique em **Próximo**.

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >Os cabeçalhos de coluna devem sempre corresponder exatamente ao campo (diferencia maiúsculas de minúsculas) para obter os melhores resultados de mapeamento automático. Se você estiver usando campos personalizados e não os vir no menu suspenso, volte e [criá-los](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target=&quot;_blank&quot;} para que possam se tornar opções.

   >[!NOTE]
   >
   >Se houver campos que você não queira importar, selecione **Ignorar** no menu suspenso Campo do Marketo .

1. Selecionar **Meu programa de shows de vendas** para **Programa de aquisição**, depois clique em **Importar**.

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. Aguarde a importação das pessoas e feche a janela pop-up de progresso da importação.

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. Voltar a **Meu programa de shows de vendas**, clique no botão **Membros** guia . Você verá todas as pessoas que acabou de importar.

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>Para analisar o sucesso de seu programa, acompanhe os membros a ele associados. Saiba mais sobre [**Programas**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target=&quot;_blank&quot;}.

## Missão cumprida {#mission-complete}

Agora os participantes de seu evento comercial são membros de seu programa do Marketo!

<br> 

[◄ Missão 4: resposta automática por e-mail](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Missão 6: promoção gota a gota ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
