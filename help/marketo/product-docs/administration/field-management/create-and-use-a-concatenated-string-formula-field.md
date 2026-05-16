---
unique-page-id: 2360337
description: Combine valores de vários campos ou crie valores condicionais usando campos de fórmula no Marketo Engage.
title: Criar e usar um campo de string concatenada (fórmula)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
TQID: https://experienceleague.adobe.com/Yk-Xh-WHUE8-GR2KTCxXRSqerdz-JHu2JnzYp8tAq9U
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 148
ht-degree: 10%

---

# Criar e usar um campo de string concatenada (fórmula) {#create-and-use-a-concatenated-string-formula-field}

Você pode combinar valores de vários campos ou criar um valor condicional usando um campo de fórmula do Marketo Engage.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Clique em **[!UICONTROL Gerenciamento de campos]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Clique em **[!UICONTROL Novo Campo Personalizado]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Selecione **[!UICONTROL Fórmula]** para o **[!UICONTROL Tipo]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Insira um **[!UICONTROL Nome]** para o seu campo e clique em **[!UICONTROL Criar]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Localize e selecione o campo de fórmula e clique em **[!UICONTROL Editar Regras]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. Adicione duas opções e as defina como a captura de tela abaixo.

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >Saiba mais sobre [tokens para etapas de fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Agora é possível adicionar o campo da fórmula como um token em um email.

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>Os campos de fórmula podem ser usados em Landing Pages, emails e colunas de Smart List. Emails com campos de fórmula _não_ podem ser enviados usando uma campanha em lote. Use um [token de script de email](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) neste cenário.
