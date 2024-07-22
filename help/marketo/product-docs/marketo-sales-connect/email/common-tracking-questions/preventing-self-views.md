---
unique-page-id: 14352540
description: Como evitar autovisualizações - Documentação do Marketo - Documentação do produto
title: Como evitar as auto visualizações
exl-id: c18715fc-4ca2-4a6b-8f63-a9406f30c0d8
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---

# Como evitar as auto visualizações {#preventing-self-views}

## Visão geral {#overview}

Obter falsos positivos no rastreamento de visualização pode gerar inconsistências de relatório. Isso geralmente ocorre quando os usuários do MSC invocam acidentalmente o pixel de rastreamento do cliente de email (chamamos isso de visualização automática). Abaixo estão algumas dicas sobre como reduzir significativamente e até mesmo eliminar as autovisualizações.

## Web (Outlook Web App e Gmail) {#web-outlook-web-app-and-gmail}

O Sales Connect armazenará um cookie em seu navegador para impedir que as exibições sejam rastreadas ao abrir seus emails do Outlook Web App e do Gmail. Se você ainda estiver recebendo visualizações pessoais, recomendamos fazer o seguinte:

* Verifique se os cookies estão ativados no computador.

* Se estiver usando um novo computador ou dispositivo móvel, verifique se você fez logon no aplicativo web. Isso nos permitirá reconhecer seu computador/dispositivo a partir de agora.

## Área de trabalho (Windows) {#desktop-windows}

As visualizações são rastreadas baixando um pequeno pixel de imagem invisível em seu cliente de email. Você pode reduzir significativamente a quantidade de visualizações automáticas no Outlook ao desabilitar o download automático de imagens. Abaixo estão as etapas como.

1. No Outlook, clique em **Arquivo** na barra de menus.

   ![](assets/win-1.png)

1. Clique em **Opções**.

   ![](assets/win-2.png)

1. Na caixa de diálogo Opções do Outlook, clique em **Central de Confiabilidade**.

   ![](assets/win-3.png)

1. Em Central de Confiabilidade do Microsoft Outlook, clique em **Configurações da Central de Confiabilidade**.

   ![](assets/win-4.png)

1. Clique em Download Automático no menu à esquerda e marque a caixa de seleção **Não baixar imagens automaticamente no email HTML ou em itens RSS**.

   ![](assets/win-5.png)

1. Clique em **OK** na caixa de diálogo Central de Confiabilidade.

   ![](assets/win-6.png)

1. Clique em **OK** na caixa de diálogo Opções do Outlook.

   ![](assets/win-6.png)

## Desktop (Mac) {#desktop-mac}

As visualizações são rastreadas baixando um pequeno pixel de imagem invisível em seu cliente de email. Você pode reduzir significativamente a quantidade de visualizações automáticas no Outlook ao desabilitar o download automático de imagens. Abaixo estão as etapas como.

1. No Outlook, clique em **Outlook** na barra de menus e selecione **Preferências**.

   ![](assets/mac-1.png)

1. Em Email, escolha **Leitura**.

   ![](assets/mac-2.png)

1. Em Segurança, clique no botão de opção **Nunca**.

   ![](assets/mac-3.png)
