---
unique-page-id: 2360337
description: Criar e usar um campo de string concatenada (fórmula) - Documentos do Marketo - Documentação do produto
title: Criar e usar um campo de string concatenada (fórmula)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
source-git-commit: b13360b009aea869bbd96a9cd0888bb121afdcd2
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# Criar e usar um campo de string concatenada (fórmula) {#create-and-use-a-concatenated-string-formula-field}

É possível combinar valores de vários campos ou criar um valor condicional usando um campo Fórmula do Marketo .

1. Vá para o **Administrador** área.

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Clique em **Gerenciamento de campos**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Clique em **Novo campo personalizado**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Selecionar **Fórmula** para **Tipo**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Insira um **Nome** no seu campo e clique em **Criar**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Encontre e selecione seu campo de fórmula e clique em **Editar regras**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. Adicione duas opções e defina-as como a captura de tela abaixo.

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >Saiba mais sobre [tokens para etapas de fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Agora é possível adicionar o campo de fórmula como um token em um email.

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>Os campos de fórmula podem ser usados em landing pages, emails e colunas de lista inteligente (não são exportados). Emails com campos de fórmula podem **not** ser enviada usando uma campanha em lote. Use um [token de script de email](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) neste cenário.

Bom trabalho! Agora você tem um campo inteligente que sabe qual saudação incluir com base no sexo. Divirta-se com isso e seja criativo.
