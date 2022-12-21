---
unique-page-id: 14352540
description: Evitando autoexibições - Documentos do Marketo - Documentação do produto
title: Evitando autoexibições
exl-id: c18715fc-4ca2-4a6b-8f63-a9406f30c0d8
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---

# Evitando autoexibições {#preventing-self-views}

## Visão geral {#overview}

Obter falsos positivos no rastreamento de visualização pode levar a inconsistências no relatório. Isso geralmente ocorre quando os usuários do MSC chamam acidentalmente o pixel de rastreamento do cliente de email (chamamos isso de autovisualização). Abaixo estão algumas dicas sobre redução significativa e até mesmo eliminação de autovisões.

## Web (Outlook Web App e Gmail) {#web-outlook-web-app-and-gmail}

O Sales Connect armazenará um cookie em seu navegador para impedir que as exibições sejam rastreadas ao abrir seus emails do Outlook Web App e do Gmail. Se você ainda estiver recebendo autovisualizações, recomendamos fazer o seguinte:

* Verifique se os cookies estão ativados no computador.

* Se estiver usando um novo computador ou dispositivo móvel, verifique se você fez logon no aplicativo da Web. Isso nos permitirá reconhecer seu computador/dispositivo a partir de agora.

## Desktop (Windows) {#desktop-windows}

As exibições são acompanhadas pelo download de um pequeno pixel de imagem invisível no seu cliente de email. Você pode reduzir significativamente a quantidade de autoexibições no Outlook, desativando as imagens a serem baixadas automaticamente. Abaixo estão os passos como.

1. No Outlook, clique em **Arquivo** na barra de menus.

   ![](assets/win-1.png)

1. Clique em **Opções**.

   ![](assets/win-2.png)

1. Na caixa de diálogo Opções do Outlook, clique em **Central de confiança**.

   ![](assets/win-3.png)

1. Em Microsoft Outlook Trust Center, clique em **Configurações da Central de Confiança**.

   ![](assets/win-4.png)

1. Clique em Download automático no menu à esquerda e selecione o **Não faça o download automático de imagens no HTML email ou em itens RSS** caixa de seleção.

   ![](assets/win-5.png)

1. Clique em **OK** na caixa de diálogo Central de Confiança.

   ![](assets/win-6.png)

1. Clique em **OK** na caixa de diálogo Opções do Outlook.

   ![](assets/win-6.png)

## Desktop (Mac) {#desktop-mac}

As exibições são acompanhadas pelo download de um pequeno pixel de imagem invisível no seu cliente de email. Você pode reduzir significativamente a quantidade de autoexibições no Outlook, desativando as imagens a serem baixadas automaticamente. Abaixo estão os passos como.

1. No Outlook, clique em **Outlook** na barra de menus e selecione **Preferências**.

   ![](assets/mac-1.png)

1. Em Email, escolha **Leitura**.

   ![](assets/mac-2.png)

1. Em Segurança, clique no botão **Nunca** botão de opção.

   ![](assets/mac-3.png)
