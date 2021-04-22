---
unique-page-id: 2359414
description: Pontuação simples - Documentação do Marketo - Documentação do produto
title: Pontuação simples
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 13%

---

# Pontuação simples {#simple-scoring}

>[!PREREQUISITES]
>
>* [Configurar e adicionar uma pessoa](get-set-up-and-add-a-person.md)
>* [Página com formulário](landing-page-with-a-form.md)


## Etapa 1: &#x200B;criar uma campanha de pontuação  {#step-create-a-scoring-campaign}

1. Vá para a área **Marketing Activities**.

   ![](assets/ma-1.png)

1. Clique com o botão direito do mouse na pasta **Learning** e clique em **New Campaign Folder**.

   ![](assets/two-2.png)

1. Nomeie a pasta da campanha como &quot;Pontuação&quot;.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Se você já tiver uma pasta de Pontuação, nomeie essa pasta como algo diferente, como Pontuação 1. Os nomes de pastas devem ser exclusivos.

1. Em seguida, clique com o botão direito do mouse na nova pasta **Scoring** e selecione **New Smart Campaign**.

   ![](assets/four.png)

1. **** Nomeie a campanha como &quot;Alterar pontuação&quot; e clique em  **Criar**.

   ![](assets/five-1.png)

1. Clique na guia **Smart List**.

   ![](assets/six-1.png)

   Queremos que essa campanha seja executada sempre que uma pessoa preencher seu **Formulário de solicitação de avaliação**.

1. Localize e arraste o acionador **Preencha o formulário** para a tela esquerda.

   ![](assets/image2014-9-24-11-3a43-3a35.png)

1. Selecione **Meu formulário**.

   >[!NOTE]
   >
   >Se você concluiu a [Landing Page com um Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) win rápido, você deve ter o formulário. Se você tiver usado um nome diferente para o formulário, selecione esse nome.

   ![](assets/image2014-9-24-11-3a44-3a16.png)

1. Clique na guia **Fluxo**.

   ![](assets/image2014-9-24-11-3a44-3a33.png)

1. Arraste a ação de fluxo **Change Score** para a tela esquerda.

   ![](assets/image2014-9-24-11-3a44-3a45.png)

1. Você pode digitar qualquer valor para adicionar à pontuação da pessoa. Vamos inserir &quot;+5&quot; no campo **Change**.

   ![](assets/eleven-1.png)

   >[!TIP]
   >
   >Boas campanhas de pontuação são fundamentais para fornecer pessoas de alta qualidade para Vendas. Leia [**O Guia Definitivo para Pontuação de Chumbo**](https://www.marketo.com/definitive-guides/lead-scoring/).

1. Clique na guia **Schedule** e no botão **Ativate**.

   ![](assets/twelve-1.png)

1. Clique em **Ativar** na tela de confirmação.

   ![](assets/thirteen-1.png)

>[!NOTE]
>
>Uma vez ativa, essa campanha será executada sempre que uma pessoa preencher o formulário. A campanha continuará em execução até ser desativada.

## Etapa 2: preencher o formulário {#step-fill-out-the-form}

1. Selecione a landing page que você criou na [Landing Page com uma vitória rápida do Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md).

   ![](assets/fourteen-1.png)

1. Clique em **Exibir página aprovada**. A página será aberta em uma nova guia.

   ![](assets/image2014-9-24-11-3a47-3a51.png)

1. Preencha o formulário com seu nome, sobrenome e endereço de email e clique em **Enviar**.

   ![](assets/image2014-9-24-11-3a47-3a59.png)

   >[!NOTE]
   >
   >Use o mesmo nome e endereço de email usado quando você se inseriu como uma pessoa pela primeira vez para aplicar o aumento de pontuação &quot;+5&quot;.

## Etapa 3: Exibir as Informações de pessoa {#step-view-the-person-info}

1. Vá para a área Banco de Dados.

   ![](assets/db-2.png)

1. Procure o endereço de email usado ao preencher o formulário.

   ![](assets/eighteen.png)

1. Clique duas vezes em sua pessoa.

   ![](assets/nineteen.png)

Os detalhes da pessoa serão abertos em uma nova guia ou janela. Veja como sua pontuação aumentou em 5 pontos para preencher o formulário?!

![](assets/twenty.png)

**Parabéns!** Você criou uma campanha de pontuação.
[◄ Missão 2: página com formulário](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[Missão 4: resposta automática por e-mail ►](/help/marketo/getting-started/quick-wins/email-auto-response.md)
