---
unique-page-id: 2360337
description: Criar e usar um campo de string concatenada (fórmula) - Documentação do Marketo - Documentação do produto
title: Criar e usar um campo de string concatenada (fórmula)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
source-git-commit: 20c41143d1e7839352dddbfea0951c2633987692
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# Criar e usar um campo de string concatenada (fórmula) {#create-and-use-a-concatenated-string-formula-field}

Você pode combinar valores de vários campos ou criar um valor condicional usando um campo Fórmula do Marketo.

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Clique em **[!UICONTROL Gerenciamento de campo]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Clique em **[!UICONTROL Novo campo personalizado]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Selecionar **[!UICONTROL Fórmula]** para o **[!UICONTROL Tipo]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Insira um **[!UICONTROL Nome]** para o campo e clique em **[!UICONTROL Criar]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Localize e selecione o campo de fórmula e clique em **[!UICONTROL Editar regras]**.

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
>Os campos de fórmula podem ser usados em páginas iniciais, emails e colunas de smart list (eles não são exportados). Os emails com campos de fórmula podem _não_ ser enviado usando uma campanha em lote. Use um [token de script de email](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) neste cenário.

Bom trabalho! Agora você tem um campo inteligente que sabe que saudação incluir com base no gênero. Divirta-se com isso e seja criativo.
