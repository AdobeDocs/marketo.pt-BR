---
description: Noções básicas sobre as opções de envio do Sales Campaign para as etapas de e-mail - Documentação do Marketo - Documentação do produto
title: Noções básicas sobre as opções de envio do Sales Campaign para etapas de email
feature: Sales Insight Actions
exl-id: 775c6401-efb2-4940-a81c-be5d2759c7bd
source-git-commit: 3e1db4c113df7278eadcf1b61ee225989e70452b
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 2%

---

# Noções básicas sobre as opções de envio do Sales Campaign para etapas de email {#understanding-sales-campaign-send-options-for-email-steps}

Ao criar uma Campanha de vendas, você tem várias opções sobre como as etapas de email são criadas em Ações de insight de vendas. E, dependendo de onde seu email se encaixa em sua Campanha de vendas, suas opções também diferem.

## Opções de envio da primeira etapa {#first-step-send-options}

Se for a primeira etapa e o primeiro dia na Campanha de vendas, você terá as seguintes opções:

![](assets/understanding-sales-campaign-send-options-for-email-steps-1.png)

### Escolherei quando enviar este email {#first-step-i-will-choose}

* Essa opção permite escolher a hora &quot;enviar em&quot; para o primeiro email na Campanha de vendas quando você iniciar a Campanha de vendas adicionando pessoas.

### Enviar este email no seguinte horário {#first-step-following-time}

* Quando você inicia sua Campanha de vendas adicionando pessoas a ela, agendamos o email para este horário.
* Você sempre tem a opção de escolher um novo &quot;enviar em&quot; momento quando estiver iniciando sua Campanha de vendas.

### Criar uma tarefa; eu mesmo vou enviar este e-mail {#first-step-create-a-task}

* Esta opção criará uma Tarefa de email (e a sincronizará com o Salesforce) que você poderá enviar quando desejar.
* Depois de fazer essa seleção, ao iniciar sua Campanha de vendas, colocaremos essas tarefas na fila do Centro de comando e do Feed ao vivo. Em seguida, você pode personalizar e enviar (ou agendar) cada email antes que ele seja enviado.

   * Se você abrir essa tarefa em nosso aplicativo web, ela abrirá uma janela de composição com o endereço de email do seu contato, a linha de assunto do seu email e o modelo escolhido.
   * Se você abrir essa tarefa no Gmail ou Outlook, ela abrirá uma janela de composição nativa e preencherá dinamicamente o endereço de email do seu contato, a linha de assunto do seu email e o modelo escolhido.

## Opções de envio da etapa subsequente {#subsequent-step-send-options}

Para qualquer dia/etapa subsequente em sua Campanha de vendas, você terá as seguintes opções:

### Enviar este email ao mesmo tempo que o email anterior nesta Campanha de vendas {#subsequent-send-at-same-time}

* Essa opção enviará o email ao mesmo tempo que o email diretamente antes dele.
* Ele ainda será enviado no dia em que estiver associado.

### Enviar este email no seguinte horário {#subsequent-send-at-following-time}

* Quando você inicia sua Campanha de vendas adicionando pessoas a ela, agendamos o email para este horário.
* Você sempre tem a opção de escolher um novo &quot;enviar em&quot; momento quando estiver iniciando sua Campanha de vendas.

### Criar uma tarefa; eu mesmo vou enviar este e-mail {#subsequent-create-a-task}

* Esta opção criará uma Tarefa de email (e a sincronizará com o Salesforce) que você poderá enviar quando desejar.
* Depois de fazer essa seleção, ao iniciar sua Campanha de vendas, as Ações do Sales Insight enfileirarão essas tarefas no Command Center e no Feed ativo. Em seguida, você pode personalizar e enviar (ou agendar) cada email antes que ele seja enviado.

   * Se você abrir essa tarefa em nosso aplicativo web, ela abrirá uma janela de composição com o endereço de email do seu contato, a linha de assunto do seu email e o modelo escolhido.
   * Se você abrir essa tarefa no Gmail ou Outlook, ela abrirá uma janela de composição nativa e preencherá dinamicamente o endereço de email do seu contato, a linha de assunto do seu email e o modelo escolhido.

### Criar este email como um acompanhamento do email anterior nesta campanha {#subsequent-create-this-email}

* Ative essa caixa de seleção se desejar que o email anterior da campanha de vendas seja anexado ao próximo email enviado pela campanha de vendas.
* Para a cópia anexada do email, o template do email em sua campanha de vendas sempre será enviado. As edições que o usuário tiver feito antes de ser enviado não serão incluídas no envio.

>[!NOTE]
>
>Essa opção para criar um email como acompanhamento só estará disponível em uma etapa de email, quando a etapa anterior também for um email. Se a etapa anterior for Chamar, InMail ou Personalizar, a opção para criar um acompanhamento não será exibida.

>[!MORELIKETHIS]
>
>[Criar uma campanha de vendas](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/create-a-sales-campaign.md){target="_blank"}
>[Tipos de Etapa de Campanha de Vendas e Tarefas de Lembrete](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-step-types-and-reminder-tasks.md){target="_blank"}
>[Configurações da campanha de vendas](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-settings.md){target="_blank"}
