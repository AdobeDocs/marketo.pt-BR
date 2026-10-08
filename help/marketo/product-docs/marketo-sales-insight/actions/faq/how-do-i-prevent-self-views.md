---
description: Saiba como evitar que as autovisualizações contem no rastreamento de email. Evite aumentar as estatísticas abertas ao visualizar seus próprios emails.
title: Como evitar auto visualizações
exl-id: 52de102f-6c6c-4663-9725-aae2f620d5bb
feature: Sales Insight Actions
TQID: 'https://experienceleague.adobe.com/6AN3CB0CoDTRPBerpKPzg94dpsvbsk5-r-DRhdePvMo'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
    internal-label: Reporting
  - id: 412786a7-b8da-5b9d-8c3f-2539a3faad9f
    internal-label: Sales Insight Actions
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 1%
---
# Como impedir as autovisualizações? {#how-do-i-prevent-self-views}

Obter falsos positivos no rastreamento de visualização pode gerar inconsistências de relatório. Isso geralmente ocorre quando usuários do [!DNL Marketo Sales] invocam acidentalmente o pixel de rastreamento do cliente de email (chamamos isso de visualização automática). Abaixo estão algumas dicas sobre como reduzir significativamente e até mesmo eliminar as autovisualizações.

## Web ([!DNL Outlook] aplicativo da Web e Gmail) {#web-outlook-web-app-and-gmail}

O [!DNL Marketo Sales] armazenará um cookie em seu navegador para impedir que os modos de exibição sejam rastreados ao abrir seus emails do [!DNL Outlook] Web App e do Gmail. Se você ainda estiver recebendo visualizações pessoais, recomendamos fazer o seguinte:

* Verifique se os cookies estão ativados no computador.

* Se estiver usando um novo computador ou dispositivo móvel, verifique se você fez logon no aplicativo web. Isso nos permitirá reconhecer seu computador/dispositivo a partir de agora.

## Área de trabalho (Windows) {#desktop-windows}

As visualizações são rastreadas baixando um pequeno pixel de imagem invisível em seu cliente de email. Você pode reduzir significativamente a quantidade de visualizações automáticas em [!DNL Outlook] desabilitando imagens para download automático. Abaixo estão as etapas como.

1. No Outlook, clique em **[!UICONTROL Arquivo]** na barra de menus.

   ![](assets/how-do-i-prevent-self-views-1.png)

1. Clique em **[!UICONTROL Opções]**.

   ![](assets/how-do-i-prevent-self-views-2.png)

1. Na caixa de diálogo [!DNL Outlook] Opções, clique em **[!UICONTROL Central de Confiabilidade]**.

   ![](assets/how-do-i-prevent-self-views-3.png)

1. Em Central de Confiabilidade do Microsoft [!DNL Outlook], clique em **[!UICONTROL Configurações da Central de Confiabilidade]**.

   ![](assets/how-do-i-prevent-self-views-4.png)

1. Clique em [!UICONTROL Download Automático] no menu à esquerda e marque a caixa de seleção **[!UICONTROL Não baixar imagens automaticamente em emails do HTML ou itens RSS]**.

   ![](assets/how-do-i-prevent-self-views-5.png)

1. Clique em **[!UICONTROL OK]** na caixa de diálogo [!UICONTROL Central de Confiabilidade].

   ![](assets/how-do-i-prevent-self-views-6.png)

1. Clique em **[!UICONTROL OK]** na caixa de diálogo [!DNL Outlook] Opções.

   ![](assets/how-do-i-prevent-self-views-7.png)

## Desktop (Mac) {#desktop-mac}

As visualizações são rastreadas baixando um pequeno pixel de imagem invisível em seu cliente de email. Você pode reduzir significativamente a quantidade de visualizações automáticas em [!DNL Outlook] desabilitando imagens para download automático. Abaixo estão as etapas como.

1. Em [!DNL Outlook], clique em **[!UICONTROL Outlook]** na barra de menus e selecione **[!UICONTROL Preferências]**.

   ![](assets/how-do-i-prevent-self-views-8.png)

1. Em [!UICONTROL Email], escolha **[!UICONTROL Leitura]**.

   ![](assets/how-do-i-prevent-self-views-9.png)

1. Em [!UICONTROL Segurança], clique no botão de opção **[!UICONTROL Nunca]**.

   ![](assets/how-do-i-prevent-self-views-10.png)
