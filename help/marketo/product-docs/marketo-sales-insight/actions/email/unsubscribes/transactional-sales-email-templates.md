---
description: Modelos de e-mail de vendas transacionais - Documentação do Marketo - Documentação do produto
title: Modelos de email de vendas transacionais
feature: Sales Insight Actions
exl-id: 0178155e-f01c-449f-b510-40adf718e177
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# Modelos de email de vendas transacionais {#transactional-sales-email-templates}

Se sua equipe estiver enviando emails transacionais ou não comerciais, você poderá marcar um modelo de email como não comercial para que ele possa ignorar cancelamentos de assinatura.

## Itens a Observar {#things-to-note}

* Emails não comerciais ignorarão cancelamentos de assinatura de vendas e [verificação de cancelamento de assinatura de Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, mas não ignorarão [domínios bloqueados](/help/marketo/product-docs/marketo-sales-insight/actions/admin/blocked-domains.md){target="_blank"}.

* As mensagens de cancelamento de inscrição não serão anexadas automaticamente a emails não comerciais, mesmo que a [configuração de administração de mensagens de cancelamento de inscrição de anexação](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} esteja habilitada. No entanto, o `{{team_unsubscribe}}` [campo dinâmico](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"} ainda preencherá a mensagem de cancelamento de inscrição da sua equipe.

## Configurar um modelo de email para uso não comercial {#configure-an-email-template-for-non-commercial-use}

1. No cabeçalho, clique em **Modelos**.

   ![](assets/transactional-sales-email-templates-1.png)

1. Localize e selecione o template que deseja atualizar.

   ![](assets/transactional-sales-email-templates-2.png)

1. Ative a opção de email não comercial em Configurações do modelo.

   ![](assets/transactional-sales-email-templates-3.png)

## Enviar um email não comercial {#send-a-non-commercial-email}

>[!NOTE]
>
>Quando uma pessoa não inscrita for selecionada, ela será realçada em laranja.

1. No cabeçalho, clique em **Compor**. Localize e selecione o modelo não comercial desejado.

   ![](assets/transactional-sales-email-templates-4.png)

1. Os usuários verão um banner mostrando que selecionaram um template de email não comercial.

   ![](assets/transactional-sales-email-templates-5.png)

1. Clique em **Enviar**.

   ![](assets/transactional-sales-email-templates-6.png)

O email ainda será enviado mesmo se a inscrição da pessoa for cancelada.
