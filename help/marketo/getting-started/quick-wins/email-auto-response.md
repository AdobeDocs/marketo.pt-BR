---
unique-page-id: 2359416
description: Resposta automática de email - Documentação do Marketo - Documentação do produto
title: Resposta automática por e-mail
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
feature: Getting Started
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 14%

---

# Resposta automática por e-mail {#email-auto-response}

## Missão: Enviar um e-mail de agradecimento quando uma pessoa preencher um formulário {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Configure e adicione uma pessoa](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Página com formulário](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Etapa 1: &#x200B;criar um e-mail {#step-create-an-email}

1. Vá para a área [!UICONTROL Atividades de marketing].

   ![](assets/email-auto-response-1.png)

1. Selecione seu programa no menu esquerdo, clique no menu suspenso **[!UICONTROL Novo]** e selecione **[!UICONTROL Novo ativo local]**.

   ![](assets/email-auto-response-2.png)

1. Selecione **[!UICONTROL Email]**.

   ![](assets/email-auto-response-3.png)

1. Nomeie seu email como &quot;Email de resposta automática&quot;, escolha um modelo e clique em **[!UICONTROL Criar]**.

   ![](assets/email-auto-response-4.png)

   Um editor de email será aberto em uma nova janela ou guia. Se os pop-ups estiverem bloqueados, clique em **[!UICONTROL Editar rascunho]** na página de resumo do ativo para acessar o email.

1. Insira uma linha de assunto e clique duas vezes na área editável do email.

   ![](assets/email-auto-response-5.png)

   _Um editor de rich text será aberto na parte superior do editor de email._

1. Selecione o conteúdo do e-mail existente.

   ![](assets/email-auto-response-6.png)

1. Digite seu conteúdo de email e clique em **[!UICONTROL Salvar]**.

   ![](assets/email-auto-response-7.png)

1. Clique no menu suspenso **[!UICONTROL Ações de email]** e selecione **[!UICONTROL Aprovar e Fechar]**.

   ![](assets/email-auto-response-8.png)

## Etapa 2: &#x200B;criar uma campanha inteligente {#step-create-a-smart-campaign}

1. Selecione seu programa, clique no menu suspenso **[!UICONTROL Novo]** e selecione **[!UICONTROL Nova Campanha Inteligente]**.

   ![](assets/email-auto-response-9.png)

1. **Nomeie** a campanha inteligente &quot;Campanha de Resposta Automática&quot; e clique em **[!UICONTROL Criar]**.

   ![](assets/email-auto-response-10.png)

1. Vá para a guia **[!UICONTROL Smart List]**.

   ![](assets/email-auto-response-11.png)

   Estamos configurando esta campanha para ser executada sempre que uma pessoa preencher o formulário criado na [**Página de Aterrissagem com um Formulário**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}.

1. Localize e arraste o acionador **[!UICONTROL Preencher formulário]** para a tela.

   ![](assets/email-auto-response-12.png)

1. Selecione **[!UICONTROL Meu formulário]** no menu suspenso. Em seguida, clique na guia **[!UICONTROL Fluxo]**.

   ![](assets/email-auto-response-13.png)

1. Arraste a ação de fluxo **[!UICONTROL Enviar Email]** para a tela à esquerda.

   ![](assets/email-auto-response-14.png)

1. Selecione seu **Email de Resposta Automática**. Em seguida, clique na guia **[!UICONTROL Agendar]**.

   ![](assets/email-auto-response-15.png)

1. Clique em **[!UICONTROL Editar]**.

   ![](assets/email-auto-response-16.png)

1. Selecione **[!UICONTROL toda vez]** e clique em **[!UICONTROL Salvar]**.

   ![](assets/email-auto-response-17.png)

1. Clique em **[!UICONTROL Ativar]**.

   ![](assets/email-auto-response-18.png)

1. Clique em **[!UICONTROL Ativar]** na tela de confirmação.

   ![](assets/email-auto-response-19.png)

>[!NOTE]
>
>Uma vez ativa, essa campanha será executada sempre que uma pessoa preencher o formulário especificado. A campanha continuará em execução até ser desativada.

## Etapa 3: preencher o formulário {#step-fill-out-the-form}

1. Selecione **Minha Página** (isso foi criado na [Página de Aterrissagem com um Formulário](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} quick win) e clique em **[!UICONTROL Visualizar]**.

   ![](assets/email-auto-response-20.png)

   _A página de aterrissagem de &quot;Avaliação Gratuita&quot; será aberta em uma nova guia._

1. Preencha o formulário com seu nome, sobrenome e endereço de email e clique em **[!UICONTROL Enviar]**.

   ![](assets/email-auto-response-21.png)

>[!NOTE]
>
>Use seu endereço de e-mail verdadeiro para poder receber a mensagem de e-mail.

## Missão cumprida {#mission-complete}

Em apenas alguns minutos, você deve ver o email de resposta automática em sua caixa de entrada.

[◄ Missão 3: Pontuação simples](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Missão 5: Importar uma Lista de Pessoas ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
