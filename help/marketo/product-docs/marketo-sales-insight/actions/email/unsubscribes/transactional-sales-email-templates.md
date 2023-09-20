---
description: Modelos de e-mail de vendas transacionais - Documentação do Marketo - Documentação do produto
title: Modelos de email de vendas transacionais
hide: true
hidefromtoc: true
feature: Sales Insight Actions
source-git-commit: f11e455196cdfb7a6c1054df40344cab5b06772b
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# Modelos de email de vendas transacionais {#transactional-sales-email-templates}

Se sua equipe estiver enviando emails transacionais ou não comerciais, você poderá marcar um modelo de email como não comercial para que ele possa ignorar cancelamentos de assinatura.

## Itens a Observar {#things-to-note}

* Emails não comerciais ignorarão cancelamentos de assinatura de vendas e [verificação de cancelamento de inscrição de Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, but will not bypass [blocked domains](/help/marketo/product-docs/marketo-sales-insight/actions/admin/blocked-domains.md){target="_blank"}.

* As mensagens de cancelamento de inscrição não serão anexadas automaticamente a emails não comerciais, mesmo que a variável [configuração anexar administrador de mensagem de cancelamento de inscrição](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} is enabled. However, the `{{team_unsubscribe}}`[dynamic field](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"} ainda preencherá a mensagem de cancelamento de inscrição da equipe.

## Configurar um modelo de email para uso não comercial {#configure-an-email-template-for-non-commercial-use}

Navegue até a seção modelo.

Procure o template que deseja atualizar.

Selecione o template.

Ative a opção de email não comercial em Configurações do modelo.

Enviar um email não comercial

Quando uma pessoa não inscrita é selecionada, ela é realçada em laranja.

Na janela de composição, selecione o modelo não comercial que deseja ver.

Os usuários verão um banner mostrando que selecionaram atualmente um template de email não comercial.

Clique em enviar e o email ainda será enviado mesmo se a inscrição da pessoa for cancelada.
