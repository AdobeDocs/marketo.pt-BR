---
unique-page-id: 1146958
description: Enviar alerta - Documentos do Marketo - Documentação do produto
title: Enviar alerta
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 2%

---

# Enviar alerta {#send-alert}

## Visão geral {#overview}

A Marketo pode enviar um alerta por email com informações pessoais para qualquer pessoa - o proprietário das vendas, um parceiro ou outra pessoa. Use a etapa de fluxo **Enviar alerta** .

![](assets/one-1.png)

## Uso {#usage}

1. Localize e selecione o email que deseja enviar.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >Seu alerta de email deve conter todas as informações do cabeçalho e estar no estado **Approved**.

1. Você pode clicar no ícone de visualização para garantir que selecionou o email correto.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Certifique-se de usar o token **Enviar Informações do Alerta** em seu email.

1. Selecione o recipient do alerta. Você pode selecionar Proprietário de Vendas ou Proprietário da Conta.

   ![](assets/four-2.png)

1. Opcionalmente, adicione quaisquer outros endereços de email desejados (separados por vírgula ou ponto-e-vírgula).

   ![](assets/five.png)

   >[!TIP]
   >
   >Em campanhas acionadoras, você pode usar tokens em **Para outros emails**, como `{{lead.Territory Owner}}` ou `{{my.Alert Recipient}}`, desde que os valores sejam endereços de email válidos. Tokens em **Para Outros Emails** não funcionarão em uma campanha em lote.

Pronto! Agora você sabe como usar a etapa de fluxo **Enviar alerta** .

>[!MORELIKETHIS]
>
>[Criar um email](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md)
