---
unique-page-id: 14352540
description: Como evitar autovisualizações - Documentação do Marketo - Documentação do produto
title: Prevenção de autovisualizações
exl-id: c18715fc-4ca2-4a6b-8f63-a9406f30c0d8
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 2%

---

# Prevenção de autovisualizações {#preventing-self-views}

## Visão geral {#overview}

Obter falsos positivos no rastreamento de visualização pode gerar inconsistências de relatório. Isso geralmente ocorre quando os usuários do MSC invocam acidentalmente o pixel de rastreamento do cliente de email (chamamos isso de visualização automática). Abaixo estão algumas dicas sobre como reduzir significativamente e até mesmo eliminar as autovisualizações.

## Web ([!DNL Outlook Web App] e Gmail) {#web-outlook-web-app-and-gmail}

O [!DNL Sales Connect] armazenará um cookie em seu navegador para impedir que os modos de exibição sejam rastreados ao abrir seus emails do Outlook Web App e do Gmail. Se você ainda estiver recebendo visualizações pessoais, recomendamos fazer o seguinte:

* Verifique se os cookies estão ativados no computador.

* Se estiver usando um novo computador ou dispositivo móvel, verifique se você fez logon no aplicativo web. Isso nos permitirá reconhecer seu computador/dispositivo a partir de agora.

## Área de trabalho (Windows) {#desktop-windows}

As visualizações são rastreadas baixando um pequeno pixel de imagem invisível em seu cliente de email. Você pode reduzir significativamente a quantidade de visualizações automáticas em [!DNL Outlook] desabilitando imagens para download automático. Abaixo estão as etapas como.

1. Em [!DNL Outlook], clique em **[!UICONTROL Arquivo]** na barra de menus.

   ![](assets/win-1.png)

1. Clique em **[!UICONTROL Opções]**.

   ![](assets/win-2.png)

1. Na caixa de diálogo [!DNL Outlook] Opções, clique em **[!UICONTROL Central de Confiabilidade]**.

   ![](assets/win-3.png)

1. Em [!UICONTROL Central de Confiabilidade do Microsoft Outlook], clique em **[!UICONTROL Configurações da Central de Confiabilidade]**.

   ![](assets/win-4.png)

1. Clique em [!UICONTROL Download Automático] no menu à esquerda e marque a caixa de seleção **[!UICONTROL Não baixar imagens automaticamente em emails do HTML ou itens RSS]**.

   ![](assets/win-5.png)

1. Clique em **[!UICONTROL OK]** na caixa de diálogo [!UICONTROL Central de Confiabilidade].

   ![](assets/win-6.png)

1. Clique em **[!UICONTROL OK]** na caixa de diálogo [!DNL Outlook] Opções.

   ![](assets/win-6.png)

## Desktop (Mac) {#desktop-mac}

As visualizações são rastreadas baixando um pequeno pixel de imagem invisível em seu cliente de email. Você pode reduzir significativamente a quantidade de visualizações automáticas em [!DNL Outlook] desabilitando imagens para download automático. Abaixo estão as etapas como.

1. Em [!DNL Outlook], clique em **[!UICONTROL Outlook]** na barra de menus e selecione **[!UICONTROL Preferências]**.

   ![](assets/mac-1.png)

1. Em [!UICONTROL Email], escolha **[!UICONTROL Leitura]**.

   ![](assets/mac-2.png)

1. Em [!UICONTROL Segurança], clique no botão de opção **[!UICONTROL Nunca]**.

   ![](assets/mac-3.png)
