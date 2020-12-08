---
unique-page-id: 1146958
description: Enviar alerta - Documentos do marketing - Documentação do produto
title: Enviar alerta
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---


# Enviar alerta {#send-alert}

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Visão geral {#overview}

O Marketo pode enviar um alerta por e-mail com informações pessoais para qualquer pessoa - o proprietário da venda, um parceiro ou outra pessoa. Use a etapa de fluxo **Enviar alerta** .

![](assets/one-1.png)

## Uso {#usage}

1. Localize e selecione o email que deseja enviar.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >**Lembrete**
   >
   >Seu alerta de email deve conter todas as informações do cabeçalho e estar no estado **Aprovado** .

1. Você pode clicar no ícone pré-visualização para garantir que selecionou o email correto.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >**Lembrete**
   >
   >Certifique-se de usar o token **Enviar informações** de alerta em seu email.

1. Selecione o recipient de alerta. Você pode selecionar Proprietário de Vendas ou Proprietário de Conta.

   ![](assets/four-2.png)

1. Como opção, adicione quaisquer outros endereços de email que desejar (separados por vírgula ou ponto-e-vírgula).

   ![](assets/five.png)

   >[!TIP]
   >
   >Em campanhas de disparo, você pode usar tokens em **Para outros e-mails** , como `{{lead.Territory Owner}}` ou `{{my.Alert Recipient}}` desde que os valores sejam endereços de e-mail válidos. Os tokens em **Para outros e-mails** não funcionarão em uma campanha em lote.

É isso! Agora você sabe como usar a etapa de fluxo **Enviar alerta** .

>[!NOTE]
>
>**Artigos relacionados**
>
>[Criar um email](../../../../product-docs/email-marketing/general/creating-an-email/create-an-email.md)

