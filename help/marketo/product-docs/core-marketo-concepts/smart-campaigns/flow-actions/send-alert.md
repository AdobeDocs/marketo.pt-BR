---
unique-page-id: 1146958
description: Enviar alerta - Documentos do marketing - Documentação do produto
title: Enviar alerta
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# Enviar alerta {#send-alert}

## Visão geral {#overview}

O Marketo pode enviar um alerta por e-mail com informações pessoais para qualquer pessoa - o proprietário da venda, um parceiro ou outra pessoa. Use a etapa de fluxo **Enviar alerta**.

![](assets/one-1.png)

## Uso {#usage}

1. Localize e selecione o email que deseja enviar.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >Seu alerta de email deve conter todas as informações do cabeçalho e estar no estado **Aprovado**.

1. Você pode clicar no ícone pré-visualização para garantir que selecionou o email correto.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Certifique-se de usar o token **Enviar informações de alerta** no seu email.

1. Selecione o recipient de alerta. Você pode selecionar Proprietário de Vendas ou Proprietário de Conta.

   ![](assets/four-2.png)

1. Como opção, adicione quaisquer outros endereços de email que desejar (separados por vírgula ou ponto-e-vírgula).

   ![](assets/five.png)

   >[!TIP]
   >
   >Nas campanhas de disparo, você pode usar tokens em **Para outros e-mails**, como `{{lead.Territory Owner}}` ou `{{my.Alert Recipient}}`, desde que os valores sejam endereços de e-mail válidos. Os tokens em **Para outros e-mails** não funcionarão em uma campanha em lote.

É isso! Agora você sabe como usar a etapa de fluxo **Enviar alerta**.

>[!MORELIKETHIS]
>
>[Criar um email](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md)
