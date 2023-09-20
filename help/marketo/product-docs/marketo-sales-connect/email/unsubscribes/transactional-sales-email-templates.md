---
description: Modelos de e-mail de vendas transacionais - Documentação do Marketo - Documentação do produto
title: Modelos de email de vendas transacionais
hide: true
hidefromtoc: true
feature: Marketo Sales Connect
source-git-commit: d6a3d95ed42d1c08d69014e1aa013e7436bd06c2
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Modelos de email de vendas transacionais {#transactional-sales-email-templates}

Se sua equipe estiver enviando emails transacionais ou não comerciais, você poderá marcar um modelo de email como não comercial para que ele possa ignorar cancelamentos de assinatura.

## Itens a Observar {#things-to-note}

* Emails não comerciais ignorarão cancelamentos de assinatura de vendas e [verificação de cancelamento de inscrição de Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, but will not bypass [blocked domains](/help/marketo/product-docs/marketo-sales-insight/actions/admin/blocked-domains.md){target="_blank"}.

* As mensagens de cancelamento de inscrição não serão anexadas automaticamente a emails não comerciais, mesmo que a variável [configuração anexar administrador de mensagem de cancelamento de inscrição](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} is enabled. However, the `{{team_unsubscribe}}` [dynamic field](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"} ainda preencherá a mensagem de cancelamento de inscrição da equipe.

## Configurar um modelo de email para uso não comercial {#configure-an-email-template-for-non-commercial-use}

1. No cabeçalho, clique em **Modelos**.

PICC

1. Procure o template que deseja atualizar.

PICC

1. Selecione o template.

PICC

1. Ative a opção de email não comercial em Configurações do modelo.

PICC

## Enviar um email não comercial {#send-a-non-commercial-email}

Quando uma pessoa não inscrita for selecionada, ela será realçada em laranja.

1. Na janela de composição, selecione o template não comercial que deseja ver.

PICC

1. Os usuários verão um banner mostrando que selecionaram atualmente um template de email não comercial.

PICC

1. Clique em **Enviar**.

PICC

O email ainda será enviado mesmo se a inscrição da pessoa for cancelada.
