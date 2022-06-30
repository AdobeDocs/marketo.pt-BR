---
unique-page-id: 2359424
description: Alertar o representante de vendas - Documentos da Marketo - Documentação do produto
title: Alertar o representante de vendas
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 23%

---

# Alertar o representante de vendas {#alert-the-sales-rep}

## Missão: Alertar o representante de vendas quando uma pessoa preencher um formulário em seu site {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Para enviar automaticamente e-mails de alerta aos representantes de vendas, você só precisa de um e-mail de alerta e uma campanha de e-mail. Aqui está como fazê-lo.

>[!PREREQUISITES]
>
>[Página de aterrissagem com um formulário](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}

## Etapa 1: Criar um email de alerta {#step-create-an-alert-email}

1. Vá para o **Atividades de marketing** área.

   ![](assets/one-5.png)

1. Selecionar **Meu programa** criado na [Página de aterrissagem com um formulário](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} vitória rápida, em seguida, em **Novo** click **Novo ativo local**.

   ![](assets/two-6.png)

1. Clique em **Email**.

   ![](assets/three-5.png)

1. **Nome** o email &quot;Meu alerta de email&quot;, selecione um modelo e clique em **Criar**.

   ![](assets/four-4.png)

1. Insira o **Nome do formulário**, **Do Email**, **Responder para** e **Assunto** que você deseja que sua equipe de vendas veja.

   ![](assets/five-5.png)

1. Clique duas vezes para editar o texto do e-mail.

   ![](assets/six-5.png)

1. Digite o conteúdo do email.

   ![](assets/seven-6.png)

1. Coloque o cursor onde deseja inserir as informações de contato da pessoa e clique no link **Inserir Token** ícone .

   ![](assets/eight-4.png)

1. Encontre e selecione o `{{SP_Send_Alert_Info}}` **Token** e clique em **Inserir**.

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} O é um token especial para emails de alerta. Consulte [Usar o token Enviar informações do alerta](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;}{target=&quot;_blank&quot;} para saber mais.

1. Clique em **Salvar**.

   ![](assets/ten-5.png)

1. Feche a guia/janela do editor de email.

   ![](assets/eleven-5.png)

1. Em **Ações de email** click **Aprovar**.

   ![](assets/twelve-4.png)

## Etapa 2: Criar uma campanha de alerta e disparador {#step-create-an-alert-trigger-campaign}

1. Selecionar **Meu programa** criado anteriormente, em seguida, em **Novo** click **Nova Campanha Inteligente**.

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **Nome** a campanha &quot;My Alert Campaign&quot; e clique em **Criar**.

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. Em **Lista inteligente** , localize e arraste a **Preenche Formulário** aciona para a tela.

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. Selecione o formulário criado anteriormente.

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. Em **Fluxo** , localize e arraste a **Enviar alerta** fluxo de ação para a tela.

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. Selecionar **Meu Email de Alerta** criado anteriormente e sair **Enviar para** as **Proprietário de Vendas**.

   ![](assets/eighteen-1.png)

1. Digite seu endereço de e-mail no campo **Para outros e-mails.**

   ![](assets/nineteen-2.png)

1. Vá para o **Agendar** e clique na guia **Ativar** botão.

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >Defina as **Regras de qualificação** para **sempre** (ao editar a Campanha inteligente) para permitir que a mesma pessoa acione alertas várias vezes.

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
   >Clique no botão **Informações da pessoa** no Marketo para ver as informações de contato.

## Missão cumprida! {#mission-complete}

<br> 

[◄ Missão 7: personalizar um e-mail](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[Missão 9: Atualizar dados de pessoa ►](/help/marketo/getting-started/quick-wins/update-person-data.md)
