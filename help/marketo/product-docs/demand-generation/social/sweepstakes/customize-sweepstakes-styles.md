---
unique-page-id: 2359807
description: Personalizar estilos de sorteio - Documentos do Marketing - Documentação do produto
title: Personalizar estilos de sorteio
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Personalizar estilos de sorteio {#customize-sweepstakes-styles}

Ao [criar sorteios](create-sweepstakes.md), você pode personalizar a aparência dela na landing page.

>[!NOTE]
>
>**Disponibilidade**
>
>Nem todos os clientes adquiriram essa funcionalidade. Entre em contato com seu representante de vendas para obter detalhes.

1. Vá para Atividades de marketing.

![](assets/login-marketing-activities-1.png)

1. Selecione os sorteios e clique em **Editar** **Rascunho**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. No editor Sorteios, vá para **App** **Configurações** **** **Aparência**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Edite o texto do botão de inscrição e o link de andamento.
1. ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Para cada elemento que você deseja personalizar, insira suas propriedades CSS personalizadas.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Exemplo de CSS para **Botão Enter**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>` Exemplo de imagem para o botão  **Enter**:
   `<pre>background:url(http://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Se você usar uma imagem com texto nela, lembre-se de remover o texto do campo **Enter** **Button **sob Texto acima.

1. À medida que você faz cada alteração, o resultado é exibido na pré-visualização Visualização e edição.

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >**Lembrete**
   >
   >
   >Teste seu botão em vários navegadores diferentes, incluindo versões mais antigas.

   >[!NOTE]
   >
   >**Artigos relacionados**
   >
   >
   >A próxima etapa é adicionar [emails de inscrição e cumprimento aos sorteios](../../../../product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).

