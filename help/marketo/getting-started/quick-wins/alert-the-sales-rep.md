---
unique-page-id: 2359424
description: Alertar o representante de vendas - Documentos do marketing - Documentação do produto
title: Alertar o representante de vendas
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---


# Alertar o representante de vendas {#alert-the-sales-rep}

## Missão: Alertar o representante de vendas quando uma pessoa preencher um formulário em seu site {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Para enviar emails de alerta automaticamente aos representantes de vendas, basta enviar um email de alerta e uma campanha de email. Aqui está como fazer isso.

>[!PREREQUISITES]
>
>[landing page com um formulário](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

## Etapa 1: Criar um email de alerta {#step-create-an-alert-email}

1. Vá para a área **Marketing Atividade** .

   ![](assets/one-5.png)

1. Selecione **Meu Programa** que você criou na [Landing page com uma vitória rápida de Formulário](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) e, em **Novo** , clique em **Novo ativo** local.

   ![](assets/two-6.png)

1. Clique em **Email**.

   ![](assets/three-5.png)

1. **Nomeie** o e-mail &quot;Meu alerta de e-mail&quot;, selecione um modelo e clique em **Criar**.

   ![](assets/four-4.png)

1. Digite o nome **** de origem, **de e-mail**, **resposta** e **assunto** que deseja que sua equipe de vendas veja.

   ![](assets/five-5.png)

1. Clique com o duplo do mouse para editar o texto do email.

   ![](assets/six-5.png)

1. Digite o conteúdo do email.

   ![](assets/seven-6.png)

1. Posicione o cursor no local em que deseja inserir as informações de contato da pessoa e clique no ícone **Inserir token** .

   ![](assets/eight-4.png)

1. Localize e selecione o `{{SP_Send_Alert_Info}}` Token **e clique em** Inserir ****.

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} é um token especial para emails de alerta. Consulte [Usar o token](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) Enviar informações de alerta para saber mais.

1. Clique em **Salvar**.

   ![](assets/ten-5.png)

1. Feche a guia/janela do editor de email.

   ![](assets/eleven-5.png)

1. Em Ações **de** email, clique em **Aprovar**.

   ![](assets/twelve-4.png)

## Etapa 2: Criar uma Campanha de Acionador de Alerta {#step-create-an-alert-trigger-campaign}

1. Selecione **Meu Programa** criado anteriormente e, em **Nova** , clique em **Nova Campanha** inteligente.

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **Nomeie** a campanha como &quot;Minha Campanha de alerta&quot; e clique em **Criar**.

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. Na guia Lista **** inteligente, localize e arraste o acionador **Preencher formulário** para fora até a tela de desenho.

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. Selecione o formulário criado anteriormente.

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. Na guia **Fluxo** , localize e arraste a ação de fluxo **Enviar alerta** para a tela.

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. Selecione **Meu Email** de Alerta criado anteriormente e deixe **Enviar para** como Proprietário **** de Vendas.

   ![](assets/eighteen-1.png)

1. Digite seu endereço de email no campo **Para outros emails** .

   ![](assets/nineteen-2.png)

1. Vá para a guia **Agendamento** e clique no botão **Ativar** .

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >Defina as Regras **de** qualificação **sempre** (editando a Campanha inteligente) para permitir que a mesma pessoa dispare alertas várias vezes.

1. Clique em **Ativar** na tela de confirmação.

   ![](assets/twenty-one-1.png)

## Etapa 3: Teste-O! {#step-test-it-out}

1. Selecione sua landing page e clique em **Visualização da página** aprovada.

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >Não se esqueça de aprovar landings page; eles não vão ao vivo até serem aprovados.

1. Preencha o formulário e clique em **Enviar**.

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. Você deverá receber seu email em breve. Depois de verificar se tudo funciona como deveria, remova seu endereço de email do fluxo Enviar alerta (consulte a etapa 2.7 acima).

   >[!NOTE]
   >
   >Clique na guia Informações **da** pessoa em Marketo para ver as informações de contato.

## Missão concluída! {#mission-complete}

<br> 

[◄ Missão 7: Personalizar um email](personalize-an-email.md)

[Missão 9: Atualizar dados de cliente potencial ►](update-person-data.md)
