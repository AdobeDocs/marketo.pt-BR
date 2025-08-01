---
unique-page-id: 14352621
description: Noções básicas sobre as opções de envio - Documentação do Marketo - Documentação do produto
title: Noções básicas sobre as opções de envio
exl-id: acdee691-478e-4ffe-90e2-54cf559fa38d
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# Noções básicas sobre as opções de envio {#understanding-send-options}

Ao criar uma Campanha, você tem várias opções sobre como as etapas de email são criadas no [!DNL Sales Connect]. E, dependendo de onde seu email se encaixa no Campaign, suas opções também diferem.

Se for o primeiro passo e o primeiro dia do Campaign, você terá as seguintes opções:

![](assets/image2019-10-25-10-43-19.png)

**Escolherei quando enviar este email**

* Essa opção permite escolher a hora &quot;enviar em&quot; para o primeiro email do Campaign quando você inicia o Campaign adicionando pessoas.

**Enviar este email no seguinte horário**

* Quando você inicia sua campanha adicionando pessoas a ela, nós agendamos o email para este horário.
* Você sempre tem a opção de escolher um novo &quot;enviar em&quot; momento em que inicia sua campanha.

**Criar uma tarefa; eu mesmo enviarei este email**

* Esta opção criará uma [!UICONTROL Tarefa de email] (e sincronizará com [!DNL Salesforce]) que você poderá enviar quando desejar.
* Depois de fazer essa seleção, quando você iniciar sua campanha, colocaremos essas tarefas na fila do Command Center e do Feed ativo. Em seguida, você pode personalizar e enviar (ou agendar) cada email antes que ele seja enviado.

   * Se você abrir essa tarefa em nosso aplicativo web, ela abrirá uma janela de composição com o endereço de email do seu contato, a linha de assunto do seu email e o modelo escolhido.
   * Se você abrir esta tarefa em [!DNL Gmail] ou [!DNL Outlook], ela abrirá uma janela de composição nativa e preencherá dinamicamente o endereço de email do seu contato, a linha de assunto do seu email e o modelo escolhido.

Para quaisquer dias/etapas subsequentes do Campaign, você terá as seguintes opções:

**Enviar este email ao mesmo tempo que o email anterior nesta Campanha**

* Essa opção enviará o email ao mesmo tempo que o email diretamente antes dele.
* Ele ainda será enviado no dia em que estiver associado.

>[!IMPORTANT]
>
>Enviar um email ao mesmo tempo que o email anterior não é suportado para emails enviados no mesmo dia. Em vez disso, o email será enviado no horário do email enviado do dia anterior. Se essa opção estiver selecionada para um email no primeiro dia da campanha (não recomendado), esse email será enviado imediatamente no início da campanha.

**Enviar este email no seguinte horário**

* Quando você inicia sua campanha adicionando pessoas a ela, nós agendamos o email para este horário.
* Você sempre tem a opção de escolher um novo &quot;enviar em&quot; momento em que inicia sua campanha.

**Criar uma tarefa; eu mesmo enviarei este email**

* Esta opção criará uma [!UICONTROL Tarefa de email] (e sincronizará com [!DNL Salesforce]) que você poderá enviar quando desejar.
* Depois de fazer essa seleção, quando você iniciar sua campanha, o Tout enfileirará essas tarefas para você no Command Center e no Feed ativo. Em seguida, você pode personalizar e enviar (ou agendar) cada email antes que ele seja enviado.

   * Se você abrir essa tarefa em nosso aplicativo web, ela abrirá uma janela de composição com o endereço de email do seu contato, a linha de assunto do seu email e o modelo escolhido.
   * Se você abrir esta tarefa em [!DNL Gmail] ou [!DNL Outlook], ela abrirá uma janela de composição nativa e preencherá dinamicamente o endereço de email do seu contato, a linha de assunto do seu email e o modelo escolhido.

**Encadear este email no email anterior**

* Essa opção de envio será um acompanhamento do email anterior e anexará o corpo do email anterior à parte inferior desse email.

