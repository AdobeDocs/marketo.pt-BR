---
unique-page-id: 2359644
description: Mostrar formulário personalizado do HTML para pessoas conhecidas - Documentação do Marketo - Documentação do produto
title: Mostrar formulário HTML personalizado para pessoas conhecidas
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 7%

---

# Mostrar formulário HTML personalizado para pessoas conhecidas {#show-custom-html-form-for-known-people}

Se um visitante tiver fornecido seu nome completo e endereço de email no passado e você não quiser que ele receba o formulário inteiro, saiba como mostrar a ele algum HTML personalizado (por exemplo, apenas um botão de download).

1. Vá para **[!UICONTROL Atividades de marketing]**.

   ![](assets/login-marketing-activities-5.png)

1. Em **[!UICONTROL Atividades de marketing]**, selecione seu formulário e clique em **[!UICONTROL Editar formulário]**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. Em **[!UICONTROL Configurações de Formulário]**, clique em **[!UICONTROL Configurações]**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Defina Se **[!UICONTROL Visitante conhecido, Mostrar]**: como **[!UICONTROL HTML personalizado]**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Clique no ![—](assets/image2014-9-25-14-3a1-3a26.png) para editar o **[!UICONTROL HTML Personalizado]** que será exibido para pessoas conhecidas.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. Há conteúdo padrão, mas fique à vontade para alterá-lo.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Tokens disponíveis:

   | Token | Descrição |
   |---|---|
   | `{{lead.FirstName}}` | Isso exibirá o nome da pessoa. |
   | `{{lead.LastName}}` | Isso exibirá o sobrenome da pessoa. |
   | `{{form.Button:default=Download}}` | Isso exibirá o botão de formulário. Substitua a área após `=` para alterar o texto do botão. |
   | `{{form.NotYou:default=Not you?}}` | Isso exibirá um link caso a pessoa seja outra pessoa. Substitua a área após `=` para alterar o texto do link. |

   >[!CAUTION]
   >
   >Somente os quatro tokens acima podem ser usados. Nenhum outro token funcionará aqui.

1. Clique em **[!UICONTROL Concluir]**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Clique em **[!UICONTROL Aprovar e Fechar]**.

   >[!NOTE]
   >
   >O formulário deve ser aprovado para ser usado em landing pages.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >Lembre-se de [aprovar o rascunho da página de aterrissagem](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) criado pelas alterações de formulário.

   Pedaço de bolo! Confira o que uma pessoa veria se voltasse ao mesmo formulário:

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >Você pode direcionar o clique do botão para o ativo definindo a página de acompanhamento do formulário para o URL do arquivo.
