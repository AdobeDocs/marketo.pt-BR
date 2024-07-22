---
description: Configuração Da Mensagem De Cancelamento De Inscrição De Anexação Automática - Documentação Do Marketo - Documentação Do Produto
title: Configuração de Mensagem de Cancelamento de Inscrição de Anexação Automática
feature: Marketo Sales Connect
exl-id: 8aa75123-f6b5-4dfe-8fa7-f764620c04e8
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Configuração de Mensagem de Cancelamento de Inscrição de Anexação Automática {#auto-append-unsubscribe-message-setting}

Certifique-se de que cada email enviado inclua uma mensagem de cancelamento de inscrição para que os recipients tenham uma opção fácil de não se comunicar. Quando a opção anexar mensagem de cancelamento de inscrição estiver habilitada, todas as comunicações que sua equipe envia do Marketo Sales incluirão uma mensagem de cancelamento de inscrição, incluindo emails enviados do aplicativo web, do Salesforce, do plug-in do Gmail e do plug-in do Outlook.

## Itens a Observar {#things-to-note}

* Para emails enviados de plug-ins, o cancelamento de inscrição só será anexado quando um modelo for usado.

* Se você usar o campo dinâmico `{{team_unsubscribe}}` em um modelo de email e a configuração de acréscimo da mensagem de cancelamento de inscrição estiver habilitada, o campo dinâmico de cancelamento de inscrição da equipe preencherá a mensagem de cancelamento de inscrição _em vez de_.

## Habilitar/Desabilitar Anexar Cancelamento de Inscrição {#enable-disable-unsubscribe-append}

1. Clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. Em Configurações De Administração, Clique Em **Cancelar Assinaturas**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. Na guia Mensagens, em Anexar mensagem de cancelamento de inscrição, mova o controle deslizante para o estado desejado.

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>Se você desativar a configuração Anexar mensagem de cancelamento de inscrição, recomendamos adicionar um rodapé de cancelamento de inscrição aos modelos para garantir que a comunicação tenha uma opção de recusa. Você pode fazer isso adicionando sua própria mensagem personalizada a cada modelo, ou usando o `{{team_unsubscribe}}` [campo dinâmico](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"}.
