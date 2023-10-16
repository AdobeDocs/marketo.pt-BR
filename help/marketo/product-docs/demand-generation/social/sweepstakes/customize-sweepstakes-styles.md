---
unique-page-id: 2359807
description: Personalizar estilos de sorteios - Documentação do Marketo - Documentação do produto
title: Personalizar estilos de sorteios
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Personalizar estilos de sorteios {#customize-sweepstakes-styles}

Quando você [criar um sorteio](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), você pode personalizar a aparência na sua landing page.

>[!AVAILABILITY]
>
>Nem todos os usuários do Marketo Engage compraram essa funcionalidade. Entre em contato com a equipe de conta do Adobe (seu gerente de conta) para obter mais detalhes.

1. Ir para **Atividades de marketing**.

![](assets/login-marketing-activities-1.png)

1. Selecione o sorteio e clique em **Editar rascunho**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. No editor do Sweepstakes, acesse **Configurações do aplicativo** > **Aparência**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Edite o texto do botão de inscrição e o link de progresso.

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Para cada elemento que deseja personalizar, insira suas propriedades de CSS personalizadas.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Exemplo de CSS para **Botão Enter**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   Exemplo de imagem para **Botão Enter**:
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Se você usar uma imagem com texto, lembre-se de remover o texto da tag **Botão Enter** em Texto acima.

1. À medida que você faz cada alteração, o resultado é exibido na pré-visualização Exibir e editar.

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >Teste seu botão em vários navegadores diferentes, incluindo versões mais antigas.

   >[!MORELIKETHIS]
   >
   >A próxima etapa é adicionar [emails de inscrição e preenchimento para o sorteio](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
