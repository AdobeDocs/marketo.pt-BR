---
unique-page-id: 2359807
description: Personalizar estilos de sorteios - Documentação do Marketo - Documentação do produto
title: Personalizar estilos de sorteios
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 1%

---

# Personalizar estilos de sorteios {#customize-sweepstakes-styles}

Ao [criar um sorteio](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), você pode personalizar sua aparência na página de aterrissagem.

>[!IMPORTANT]
>
>Em 31 de julho de 2024, iniciamos o processo de desativação desse recurso. Você não poderá criar novos ativos. Os ativos existentes continuarão a funcionar até 31 de janeiro de 2025. [Saiba mais](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>Nem todos os usuários do Marketo Engage compraram essa funcionalidade. Entre em contato com a equipe de conta do Adobe (seu gerente de conta) para obter mais detalhes.

1. Vá para **Atividades de marketing**.

![](assets/login-marketing-activities-1.png)

1. Selecione o sorteio e clique em **Editar Rascunho**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. No editor de Sorteios, vá para **Configurações do Aplicativo** > **Aparência**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Edite o texto do botão de inscrição e o link de progresso.

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Para cada elemento que deseja personalizar, insira suas propriedades de CSS personalizadas.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Exemplo de CSS para o **Botão Enter**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   Exemplo de imagem para o **Botão Enter**:
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Se você usar uma imagem com texto, lembre-se de remover o texto do campo **Botão Enter** em Texto acima.

1. À medida que você faz cada alteração, o resultado é exibido na pré-visualização Exibir e editar.

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >Teste seu botão em vários navegadores diferentes, incluindo versões mais antigas.

   >[!MORELIKETHIS]
   >
   >A próxima etapa é adicionar [emails de inscrição e preenchimento ao sorteio](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
