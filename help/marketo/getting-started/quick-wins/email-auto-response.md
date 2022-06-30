---
unique-page-id: 2359416
description: Resposta automática de email - Documentos do Marketo - Documentação do produto
title: Resposta automática por e-mail
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '392'
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

   ![](assets/one-2.png)

1. Selecione Meu programa no menu esquerdo, clique no menu suspenso Novo e selecione Novo ativo local.

   ![](assets/two-3.png)

1. Clicar em e-mail.

   ![](assets/three-2.png)

1. Nomeie seu email como &quot;Email de resposta automática&quot;, escolha um modelo e clique em Criar.

   ![](assets/four-1.png)

   Um editor de e-mail será aberto em uma nova janela ou guia. Se as janelas pop-ups estiverem bloqueadas, clique em **Editar rascunho** na página de resumo do ativo para acessar o email.

1. Insira uma linha de assunto e clique duas vezes na área editável do email.

   ![](assets/five-2.png)

   _Um editor de rich text será aberto em cima do editor de e-mail._

1. Selecione o conteúdo do e-mail existente.

   ![](assets/six-2.png)

1. Digite o conteúdo do e-mail. e clique em Salvar.

   ![](assets/seven-2.png)

1. Suas alterações são salvas automaticamente. Feche a guia/janela do editor de email.

   ![](assets/eight-1.png)

1. Selecione o novo email. Em Ações de email , clique em Aprovar .

   ![](assets/image2014-9-24-11-3a55-3a16.png)

## Etapa 2: &#x200B;criar uma campanha inteligente {#step-create-a-smart-campaign}

1. Clique com o botão direito do mouse **Meu programa** e clique em **Nova Campanha Inteligente**.

   ![](assets/image2014-9-24-11-3a56-3a13.png)

1. **Nome** crie a campanha inteligente &quot;Campanha de resposta automática&quot; e clique em **Criar**.

   ![](assets/image2014-9-24-11-3a56-3a25.png)

1. Vá para o **Lista inteligente** guia .

   ![](assets/image2014-9-24-11-3a56-3a38.png)

   Estamos configurando essa campanha para ser executada sempre que uma pessoa preencher o formulário criado em [**Página de aterrissagem com um formulário**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}.

1. Encontre e arraste a **Preenche Formulário** aciona a tela à esquerda.

   ![](assets/image2014-9-24-11-3a57-3a18.png)

1. Selecionar **Meu formulário** no menu suspenso . Clique no botão **Fluxo** guia .

   ![](assets/image2014-9-24-11-3a57-3a29.png)

1. Arraste o **Enviar Email** fluxo de ação para a tela à esquerda.

   ![](assets/image2014-9-24-11-3a57-3a41.png)

1. Selecione seu **Email de resposta automática** e vá para o **Agendar** guia .

   ![](assets/image2014-9-24-11-3a57-3a53.png)

1. Clique em **Editar**.

   ![](assets/8.png)

1. Selecionar **sempre** e clique em **Salvar**.

   ![](assets/9.png)

1. Clique em **Ativar**.

   ![](assets/10.png)

1. Clique em **Ativar** na tela de confirmação.

   ![](assets/11.png)

>[!NOTE]
>
>Uma vez ativa, essa campanha será executada sempre que uma pessoa preencher o formulário especificado. A campanha continuará em execução até ser desativada.

## Etapa 3: preencher o formulário {#step-fill-out-the-form}

1. Selecionar **Minha página**. Isso foi criado no [Página de aterrissagem com um formulário](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} vitória rápida.

   ![](assets/image2014-9-24-12-3a0-3a8.png)

1. Clique em **Exibir página aprovada**.

   ![](assets/image2014-9-24-12-3a0-3a18.png)

   Sua página &quot;Avaliação gratuita&quot; será aberta em uma nova guia.

1. Preencha o formulário com seu nome, sobrenome e endereço de email e clique em **Enviar**.

   ![](assets/image2014-9-24-12-3a0-3a28.png)

>[!NOTE]
>
>Use seu endereço de e-mail verdadeiro para poder receber a mensagem de e-mail.

## Missão cumprida {#mission-complete}

Em apenas alguns minutos, você deverá ver o email de resposta automática na sua caixa de entrada. Muito bem!

<br> 

[◄ Missão 3: pontuação simples](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Missão 5: Importar uma lista de pessoas ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
