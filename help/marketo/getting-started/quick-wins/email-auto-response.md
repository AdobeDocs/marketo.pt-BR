---
unique-page-id: 2359416
description: Resposta automática de email - Documentos do Marketo - Documentação do produto
title: Resposta automática por e-mail
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
source-git-commit: 1c350eb17992e45b9e0f825e1abd5c86555d0a0a
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 23%

---

# Resposta automática por e-mail {#email-auto-response}

## Missão: Enviar um email de agradecimento quando uma pessoa preencher um formulário {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Configurar e adicionar uma pessoa](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [Página de aterrissagem com um formulário](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}


## Etapa 1: &#x200B;criar um e-mail {#step-create-an-email}

1. Vá para a área Marketing Activities .

   ![](assets/email-auto-response-1.png)

1. Selecione o programa no menu esquerdo e clique no botão **Novo** e selecione **Novo ativo local**.

   ![](assets/email-auto-response-2.png)

1. Selecionar **Email**.

   ![](assets/email-auto-response-3.png)

1. Nomeie seu email como &quot;Email de resposta automática&quot;, escolha um modelo e clique em **Criar**.

   ![](assets/email-auto-response-4.png)

   Um editor de e-mail será aberto em uma nova janela ou guia. Se as janelas pop-ups estiverem bloqueadas, clique em **Editar rascunho** na página de resumo do ativo para acessar o email.

1. Insira uma linha de assunto e clique duas vezes na área editável do email.

   ![](assets/email-auto-response-5.png)

   _Um editor de rich text será aberto em cima do editor de e-mail._

1. Selecione o conteúdo do e-mail existente.

   ![](assets/email-auto-response-6.png)

1. Digite o conteúdo do e-mail. e clique em **Salvar**.

   ![](assets/email-auto-response-7.png)

1. Clique no botão **Ações de email** e selecione **Aprovar e fechar**.

   ![](assets/email-auto-response-8.png)

## Etapa 2: &#x200B;criar uma campanha inteligente {#step-create-a-smart-campaign}

1. Selecione o programa, clique no botão **Novo** e selecione **Nova Campanha Inteligente**.

   ![](assets/email-auto-response-9.png)

1. **Nome** crie a campanha inteligente &quot;Campanha de resposta automática&quot; e clique em **Criar**.

   ![](assets/email-auto-response-10.png)

1. Vá para o **Lista inteligente** guia .

   ![](assets/email-auto-response-11.png)

   Estamos configurando essa campanha para ser executada sempre que uma pessoa preencher o formulário criado em [**Página de aterrissagem com um formulário**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}.

1. Encontre e arraste a **Preenche Formulário** aciona para a tela.

   ![](assets/email-auto-response-12.png)

1. Selecionar **Meu formulário** no menu suspenso . Em seguida, clique no botão **Fluxo** guia .

   ![](assets/email-auto-response-13.png)

1. Arraste o **Enviar Email** fluxo de ação para a tela à esquerda.

   ![](assets/email-auto-response-14.png)

1. Selecione seu **Email de resposta automática**. Em seguida, clique no botão **Agendar** guia .

   ![](assets/email-auto-response-15.png)

1. Clique em **Editar**.

   ![](assets/email-auto-response-16.png)

1. Selecionar **Todas as vezes** e clique em **Salvar**.

   ![](assets/email-auto-response-17.png)

1. Clique em **Ativar**.

   ![](assets/email-auto-response-18.png)

1. Clique em **Ativar** na tela de confirmação.

   ![](assets/email-auto-response-19.png)

>[!NOTE]
>
>Uma vez ativa, essa campanha será executada sempre que uma pessoa preencher o formulário especificado. A campanha continuará em execução até ser desativada.

## Etapa 3: preencher o formulário {#step-fill-out-the-form}

1. Selecionar **Minha página** (isso foi criado no [Página de aterrissagem com um formulário](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} quick win) e clique em **Visualizar**.

   ![](assets/email-auto-response-20.png)

   _Sua página &quot;Avaliação gratuita&quot; será aberta em uma nova guia._

1. Preencha o formulário com seu nome, sobrenome e endereço de email e clique em **Enviar**.

   ![](assets/email-auto-response-21.png)

>[!NOTE]
>
>Use seu endereço de e-mail verdadeiro para poder receber a mensagem de e-mail.

## Missão cumprida {#mission-complete}

Em apenas alguns minutos, você deverá ver o email de resposta automática na sua caixa de entrada. Muito bem!

<br> 

[◄ Missão 3: pontuação simples](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Missão 5: Importar uma lista de pessoas ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
