---
unique-page-id: 1146958
description: Enviar alerta - Documentação do Marketo - Documentação do produto
title: Enviar alerta
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 3%

---

# Enviar alerta {#send-alert}

## Visão geral {#overview}

A Marketo pode enviar um alerta por email com informações pessoais para qualquer pessoa: o proprietário das vendas, um parceiro ou outra pessoa. Use o **Enviar alerta** etapa do fluxo.

![](assets/one-1.png)

## Uso {#usage}

1. Localize e selecione o email que deseja enviar.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >Seu alerta de email deve conter todas as informações de cabeçalho e estar no estado **Aprovado** estado.

1. Você pode clicar no ícone de visualização para garantir que selecionou o email correto.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Certifique-se de usar o **Enviar informações de alerta** token no email.

1. Selecione o destinatário do alerta. Você pode escolher o Proprietário de Vendas ou o Proprietário da Conta.

   ![](assets/four-2.png)

1. Como opção, adicione outros endereços de email desejados (separados por vírgula ou ponto e vírgula).

   ![](assets/five.png)

   >[!TIP]
   >
   >Em campanhas de acionadores, você pode usar tokens no **Para Outros Emails** como `{{lead.Territory Owner}}` ou `{{my.Alert Recipient}}` desde que os valores sejam endereços de email válidos. Tokens em **Para Outros Emails** não funcionarão em uma campanha em lote.

Pronto! Agora você sabe como usar o **Enviar alerta** etapa do fluxo.

>[!MORELIKETHIS]
>
>[Criar um email](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md)
