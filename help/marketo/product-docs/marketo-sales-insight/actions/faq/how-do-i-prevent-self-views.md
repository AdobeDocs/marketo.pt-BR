---
description: Como impedir autoexibições - Documentos do Marketo - Documentação do produto
title: Como impedir autoexibições
exl-id: 52de102f-6c6c-4663-9725-aae2f620d5bb
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Como Impedir Visualizações Automáticas? {#how-do-i-prevent-self-views}

Obter falsos positivos no rastreamento de visualização pode levar a inconsistências no relatório. Isso geralmente ocorre quando os usuários do Marketo Sales acidentalmente chamam o pixel de rastreamento do cliente de email (chamamos isso de autovisualização). Abaixo estão algumas dicas sobre redução significativa e até mesmo eliminação de autovisões.

## Web (Outlook Web App e Gmail) {#web-outlook-web-app-and-gmail}

O Marketo Sales armazenará um cookie em seu navegador para impedir que as exibições sejam rastreadas ao abrir seus emails do Outlook Web App e Gmail. Se você ainda estiver recebendo autovisualizações, recomendamos fazer o seguinte:

* Verifique se os cookies estão ativados no computador.

* Se estiver usando um novo computador ou dispositivo móvel, verifique se você fez logon no aplicativo da Web. Isso nos permitirá reconhecer seu computador/dispositivo a partir de agora.

## Desktop (Windows) {#desktop-windows}

As exibições são acompanhadas pelo download de um pequeno pixel de imagem invisível no seu cliente de email. Você pode reduzir significativamente a quantidade de autoexibições no Outlook, desativando as imagens a serem baixadas automaticamente. Abaixo estão os passos como.

1. No Outlook, clique em **Arquivo** na barra de menus.

   ![](assets/how-do-i-prevent-self-views-1.png)

1. Clique em **Opções**.

   ![](assets/how-do-i-prevent-self-views-2.png)

1. Na caixa de diálogo Opções do Outlook, clique em **Central de confiança**.

   ![](assets/how-do-i-prevent-self-views-3.png)

1. Em Microsoft Outlook Trust Center, clique em **Configurações da Central de Confiança**.

   ![](assets/how-do-i-prevent-self-views-4.png)

1. Clique em Download automático no menu à esquerda e selecione o **Não faça o download automático de imagens no HTML email ou em itens RSS** caixa de seleção.

   ![](assets/how-do-i-prevent-self-views-5.png)

1. Clique em **OK** na caixa de diálogo Central de Confiança.

   ![](assets/how-do-i-prevent-self-views-6.png)

1. Clique em **OK** na caixa de diálogo Opções do Outlook.

   ![](assets/how-do-i-prevent-self-views-7.png)

## Desktop (Mac) {#desktop-mac}

As exibições são acompanhadas pelo download de um pequeno pixel de imagem invisível no seu cliente de email. Você pode reduzir significativamente a quantidade de autoexibições no Outlook, desativando as imagens a serem baixadas automaticamente. Abaixo estão os passos como.

1. No Outlook, clique em **Outlook** na barra de menus e selecione **Preferências**.

   ![](assets/how-do-i-prevent-self-views-8.png)

1. Em Email, escolha **Leitura**.

   ![](assets/how-do-i-prevent-self-views-9.png)

1. Em Segurança, clique no botão **Nunca** botão de opção.

   ![](assets/how-do-i-prevent-self-views-10.png)
