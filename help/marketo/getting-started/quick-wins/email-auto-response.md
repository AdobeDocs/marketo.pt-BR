---
unique-page-id: 2359416
description: Resposta automática por email - Documentos do Marketo - Documentação do produto
title: Resposta automática por email
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '380'
ht-degree: 100%

---

# Resposta automática por email {#email-auto-response}

## Missão: enviar um email de agradecimento quando uma pessoa preencher um formulário {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Configurar e adicionar uma pessoa](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Página com formulário](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Etapa 1: &#x200B;criar um e-mail {#step-create-an-email}

1. Acesse a área [!UICONTROL Atividades de marketing].

   ![](assets/email-auto-response-1.png)

1. Selecione seu programa no menu esquerdo, clique no menu suspenso **[!UICONTROL Novo]** e selecione **[!UICONTROL Novo ativo local]**.

   ![](assets/email-auto-response-2.png)

1. Selecione **[!UICONTROL Email]**.

   ![](assets/email-auto-response-3.png)

1. Nomeie seu email como “Email de resposta automática”, escolha um modelo e clique em **[!UICONTROL Criar]**.

   ![](assets/email-auto-response-4.png)

   O editor de email será aberto em uma nova janela ou guia. Se os pop-ups estiverem bloqueados, clique em **[!UICONTROL Editar rascunho]** na página de resumo do ativo para acessar o email.

1. Insira uma linha de assunto e clique duas vezes na área editável do email.

   ![](assets/email-auto-response-5.png)

   _Um editor de rich text será aberto sobre o editor de email._

1. Selecione o conteúdo do email existente.

   ![](assets/email-auto-response-6.png)

1. Digite seu conteúdo de email e clique em **[!UICONTROL Salvar]**.

   ![](assets/email-auto-response-7.png)

1. Clique no menu suspenso **[!UICONTROL Ações de email]** e selecione **[!UICONTROL Aprovar e fechar]**.

   ![](assets/email-auto-response-8.png)

## Etapa 2: criar uma campanha inteligente {#step-create-a-smart-campaign}

1. Selecione seu programa, clique no menu suspenso **[!UICONTROL Novo]** e selecione **[!UICONTROL Nova campanha inteligente]**.

   ![](assets/email-auto-response-9.png)

1. **Nomeie** a campanha inteligente como “Campanha de resposta automática” e clique em **[!UICONTROL Criar]**.

   ![](assets/email-auto-response-10.png)

1. Acesse a guia **[!UICONTROL Lista inteligente]**.

   ![](assets/email-auto-response-11.png)

   Estamos configurando esta campanha para ser executada sempre que uma pessoa preencher o formulário que você criou em [**Página de destino com um formulário**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}.

1. Localize e arraste o acionador **[!UICONTROL Preencheu o formulário]** para a tela.

   ![](assets/email-auto-response-12.png)

1. Selecione **[!UICONTROL Meu formulário]** no menu suspenso. Em seguida, clique na guia **[!UICONTROL Fluxo]**.

   ![](assets/email-auto-response-13.png)

1. Arraste a ação de fluxo **[!UICONTROL Enviar email]** para a tela esquerda.

   ![](assets/email-auto-response-14.png)

1. Selecione o **Email de resposta automática**. Em seguida, clique na guia **[!UICONTROL Cronograma]**.

   ![](assets/email-auto-response-15.png)

1. Clique em **[!UICONTROL Editar]**.

   ![](assets/email-auto-response-16.png)

1. Selecione **[!UICONTROL Toda vez]** e clique em **[!UICONTROL Salvar]**.

   ![](assets/email-auto-response-17.png)

1. Clique em **[!UICONTROL Ativar]**.

   ![](assets/email-auto-response-18.png)

1. Clique em **[!UICONTROL Ativar]** na tela de confirmação.

   ![](assets/email-auto-response-19.png)

>[!NOTE]
>
>Uma vez ativa, esta campanha será executada sempre que uma pessoa preencher o formulário especificado. A campanha continuará em execução até ser desativada.

## Etapa 3: preencher o formulário {#step-fill-out-the-form}

1. Selecione **Minha página** (isso foi criado na missão rápida [Página de destino com um formulário](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}) e clique em **[!UICONTROL Pré-visualizar]**.

   ![](assets/email-auto-response-20.png)

   _A página de destino “Teste gratuito” será aberta em uma nova guia._

1. Preencha o formulário com seu nome, sobrenome, endereço de email e clique em **[!UICONTROL Enviar]**.

   ![](assets/email-auto-response-21.png)

>[!NOTE]
>
>Use seu endereço de e-mail verdadeiro para poder receber a mensagem de e-mail.

## Missão cumprida {#mission-complete}

Em apenas alguns minutos, você deverá ver o email de resposta automática na sua caixa de entrada.

[◄ Missão 3: pontuação simples](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Missão 5: importar uma lista de pessoas ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
