---
unique-page-id: 2360337
description: Criar e usar um campo de string concatenada (fórmula) - Documentos do Marketo - Documentação do produto
title: Criar e usar um campo de string concatenada (fórmula)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Criar e usar um campo de string concatenada (fórmula) {#create-and-use-a-concatenated-string-formula-field}

É possível combinar valores de vários campos ou criar um valor condicional usando um campo Fórmula do Marketo .

1. Ir para **Administrador** e clique em **Gerenciamento de campos**.

   ![](assets/image2014-9-19-9-3a44-3a58.png)

1. Clique em **Novo campo personalizado**.

   ![](assets/image2014-9-19-9-3a45-3a8.png)

1. Selecionar **Fórmula** para **Tipo**.

   ![](assets/image2014-9-19-9-3a45-3a17.png)

1. Insira um **Nome** no seu campo e clique em **Criar**.

   ![](assets/image2014-9-19-9-3a46-3a0.png)

1. Encontre e selecione seu campo de fórmula e clique em **Editar regras**.

   ![](assets/image2014-9-19-9-3a46-3a13.png)

1. Adicione duas opções e defina-as como a captura de tela abaixo.

   ![](assets/image2014-9-19-9-3a46-3a25.png)

   >[!TIP]
   >
   >Saiba mais sobre [tokens para etapas de fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Agora é possível adicionar o campo de fórmula como um token em um email.

   ![](assets/seven.png)

>[!NOTE]
>
>Os campos de fórmula podem ser usados em landing pages, emails e colunas de lista inteligente (não são exportados). Emails com campos de fórmula podem **not** ser enviada usando uma campanha em lote. Use um [token de script de email](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) neste cenário.

Bom trabalho! Agora você tem um campo inteligente que sabe qual saudação incluir com base no sexo. Divirta-se com isso e seja criativo.
