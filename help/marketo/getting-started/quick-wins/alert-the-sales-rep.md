---
unique-page-id: 2359424
description: Alertar o representante de vendas - Documentos da Marketo - Documentação do produto
title: Alertar o representante de vendas
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 28%

---

# Alertar o representante de vendas {#alert-the-sales-rep}

## Missão: Alertar o representante de vendas quando uma pessoa preencher um formulário em seu site {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Para enviar automaticamente e-mails de alerta aos representantes de vendas, você só precisa de um e-mail de alerta e uma campanha de e-mail. Aqui está como fazê-lo.

>[!PREREQUISITES]
>
>[Página com formulário](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

## Etapa 1: Criar um email de alerta {#step-create-an-alert-email}

1. Vá para a área **Marketing Activities**.

   ![](assets/one-5.png)

1. Selecione **My Program** que você criou na [Landing Page com uma vitória rápida Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) e, em **New** clique em **New Local Asset**.

   ![](assets/two-6.png)

1. Clique em **Email**.

   ![](assets/three-5.png)

1. **** Nomeie o email como &quot;Meu alerta de email&quot;, selecione um modelo e clique em  **Criar**.

   ![](assets/four-4.png)

1. Insira o **Do nome**, **Do email**, **Responder para** e **Assunto** que você deseja que a equipe de vendas veja.

   ![](assets/five-5.png)

1. Clique duas vezes para editar o texto do e-mail.

   ![](assets/six-5.png)

1. Digite o conteúdo do email.

   ![](assets/seven-6.png)

1. Coloque o cursor onde deseja inserir as informações de contato da pessoa e clique no ícone **Inserir token**.

   ![](assets/eight-4.png)

1. Localize e selecione o `{{SP_Send_Alert_Info}}` **Token** e clique em **Inserir**.

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} é um token especial para e-mails de alerta. Consulte [Use o token Enviar informações de alerta](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) para saber mais.

1. Clique em **Salvar**.

   ![](assets/ten-5.png)

1. Feche a guia/janela do editor de email.

   ![](assets/eleven-5.png)

1. Em **Ações de email** clique em **Aprovar**.

   ![](assets/twelve-4.png)

## Etapa 2: Criar uma campanha de disparador de alertas {#step-create-an-alert-trigger-campaign}

1. Selecione **Meu Programa** criado anteriormente e, em **Novo** clique em **Nova Campanha Inteligente**.

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **** Nomeie a campanha como &quot;Minha campanha de alerta&quot; e clique em  **Criar**.

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. Na guia **Smart List**, localize e arraste o acionador **Preencha o formulário** para a tela.

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. Selecione o formulário criado anteriormente.

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. Na guia **Fluxo**, localize e arraste a ação de fluxo **Enviar alerta** para a tela.

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. Selecione **My Alert Email** criado anteriormente e deixe **Send To** como **Sales Owner**.

   ![](assets/eighteen-1.png)

1. Digite seu endereço de e-mail no campo **Para outros e-mails.**

   ![](assets/nineteen-2.png)

1. Vá para a guia **Schedule** e clique no botão **Ativate**.

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >Defina as **Regras de qualificação** como **sempre** (editando a Campanha inteligente) para permitir que a mesma pessoa acione alertas várias vezes.

1. Clique em **Ativar** na tela de confirmação.

   ![](assets/twenty-one-1.png)

## Etapa 3: Teste! {#step-test-it-out}

1. Selecione a landing page e clique em **Exibir página aprovada**.

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >Não esqueça de aprovar as páginas, pois elas só são disponibilizadas após a aprovação.

1. Preencha o formulário e clique em **Enviar**.

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. Você deve receber seu e-mail em breve. Depois de verificar se tudo está funcionando como deveria, remova seu endereço de e-mail do fluxo Enviar alerta (veja a etapa 2.7 acima).

   >[!NOTE]
   >
   >Clique na guia **Informações da pessoa** no Marketo para ver as informações de contato.

## Missão cumprida! {#mission-complete}

<br> 

[◄ Missão 7: personalizar um e-mail](personalize-an-email.md)

[Missão 9: atualizar dados de leads ►](update-person-data.md)
