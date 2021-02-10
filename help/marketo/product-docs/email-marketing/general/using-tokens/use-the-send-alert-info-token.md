---
unique-page-id: 2952678
description: Usar o token Enviar informações de alerta {{SP_Send_Alert_Info}} - Documentos de marketing - Documentação do produto
title: Usar o token Enviar informações de alerta
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---


# Usar o token Enviar informações de alerta {#use-the-send-alert-info-token-sp-send-alert-info}

O token `{{SP_Send_Alert_Info}}` é um token especial a ser usado ao criar emails de alerta para sua equipe de vendas.

>[!TIP]
>
>Este token só funciona como esperado ao enviar o email que o contém com a etapa de fluxo [Enviar alerta](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md). Ele não funcionará quando usado em uma etapa de fluxo Enviar e-mail.

Exemplo de alerta:

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>Atenção! Os URLs em alertas têm datas de expiração, portanto, verifique se eles têm uma cadência compatível com esses tipos de mensagens. As datas de expiração são [configuradas por um Admin](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

As seguintes informações estão incluídas como parte do `{{SP_Send_Alert_Info}}`:

* Nome e sobrenome como um link para os detalhes da pessoa no Marketo
* Um link para a pessoa em seu CRM
* O nome da campanha no Marketo que enviou o alerta
* A hora em que o alerta foi enviado

>[!NOTE]
>
>O link para o CRM só será exibido se a pessoa estiver no sistema CRM (atualmente não disponível no Dynamics CRM). O link pode ser acessado por usuários do Marketing e não do Marketing.

## Adicione o token SP_Send_Alert_Info a um email {#add-the-sp-send-alert-info-token-to-an-email}

1. Selecione o email e clique em **Editar rascunho**.

   ![](assets/one-3.png)

1. Clique com o duplo na área editável à qual deseja adicionar o token.

   ![](assets/two-3.png)

1. Posicione o cursor no local desejado para o token e clique no botão **Inserir token**.

   ![](assets/three-3.png)

1. Localize e selecione o token **`{{SP_Send_Alert_Info}}`** e clique em **Inserir**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Clique em **Salvar**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>Não se esqueça de aprovar seu email.

Que coisa boa! Esse token é muito útil e você deve usá-lo em todos os alertas criados para sua equipe de vendas.
