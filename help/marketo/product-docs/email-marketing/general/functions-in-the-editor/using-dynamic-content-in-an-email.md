---
unique-page-id: 2950617
description: Saiba como usar conteúdo dinâmico em um email. Mostre conteúdo diferente para segmentos diferentes com base em regras e atributos.
title: Usar conteúdo dinâmico em um email
exl-id: a1178f76-6760-4a4a-9510-f129ee6a9032
feature: Email Editor
TQID: https://experienceleague.adobe.com/NzTat-p-dgq9wtHv-hyJJzAwud27aOBvVTIS1Tn0lnc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 271
ht-degree: 5%

---

# Usar conteúdo dinâmico em um email {#using-dynamic-content-in-an-email}

>[!PREREQUISITES]
>
>[Criar uma segmentação](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

Use o Conteúdo dinâmico em emails para enviar informações direcionadas aos seus clientes potenciais.

>[!NOTE]
>
>O uso de variáveis no conteúdo dinâmico em um email só é compatível com o uso de Campanhas de acionador. **Não** suportado ao usar Campanhas em Lote.

## Adicionar segmentação {#add-segmentation}

1. Acesse **[!UICONTROL Atividades de marketing]**.

   ![](assets/login-marketing-activities.png)

1. Selecione seu email e clique em **[!UICONTROL Editar Rascunho]**.

   ![](assets/1.2.png)

1. Neste exemplo, estamos tornando a Linha de assunto dinâmica. Clique no campo [!UICONTROL Assunto] e no botão **Tornar dinâmico**.

   ![](assets/1.3.png)

   >[!NOTE]
   >
   >Você também pode tornar um elemento dentro do email dinâmico. Para fazer isso, selecione a área, clique no ícone de engrenagem e selecione **Tornar dinâmico** (ou [Substituir pelo trecho](/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md), dependendo do que você estiver fazendo).

1. Insira o nome da Segmentação, selecione-o e clique em **[!UICONTROL Salvar]**.

   ![](assets/1.4.png)

   Sua segmentação e seus segmentos aparecem na guia [!UICONTROL Dinâmico] à direita.

   ![](assets/1.5.png)

## Aplicar conteúdo dinâmico {#apply-dynamic-content}

>[!CAUTION]
>
>O número de elementos de conteúdo dinâmico permitidos não é ilimitado. Embora não haja um limite de número específico (pode variar com base na combinação de conteúdo), o uso excessivo de conteúdo dinâmico pode afetar negativamente o desempenho do email. Recomendamos manter a quantidade de elementos de conteúdo dinâmico usados para menos de 20 por email.

1. Clique nos segmentos e adicione a linha de assunto.

![](assets/2.1.png)

1. Repita o procedimento para cada segmento.

   ![](assets/2.2.png)

>[!TIP]
>
>Crie um email padrão antes de aplicar conteúdo aos vários segmentos.

>[!CAUTION]
>
>As alterações no bloco de conteúdo Segmento padrão são aplicadas a todos os segmentos.

Doce! Agora você pode enviar emails flexíveis para seu público-alvo.

>[!MORELIKETHIS]
>
>* [Visualizar um Email com Conteúdo Dinâmico](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)
>* [Usar Conteúdo Dinâmico em uma Página de Aterrissagem](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/use-dynamic-content-in-a-free-form-landing-page.md)
