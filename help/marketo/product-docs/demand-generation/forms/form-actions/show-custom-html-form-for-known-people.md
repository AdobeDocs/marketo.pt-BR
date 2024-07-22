---
unique-page-id: 2359644
description: Mostrar formulário de HTML personalizado para pessoas conhecidas - Documentação do Marketo - Documentação do produto
title: Mostrar formulário de HTML personalizado para pessoas conhecidas
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 1%

---

# Mostrar formulário de HTML personalizado para pessoas conhecidas {#show-custom-html-form-for-known-people}

Se um visitante é diagnosticado (pessoa conhecida que forneceu um endereço de email no passado), por que se preocupar com o formulário? Dê a eles o botão de download. Veja como.

1. Vá para **Atividades de marketing**.

   ![](assets/login-marketing-activities-5.png)

1. Em **Atividades de marketing**, selecione seu formulário e clique em **Editar formulário**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. Em **Configurações de Formulário**, clique em **Configurações**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Defina Se **Visitante conhecido, Mostrar**: como **HTML personalizado**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Clique no ![—](assets/image2014-9-25-14-3a1-3a26.png) para editar o **HTML personalizado** que será exibido para pessoas conhecidas.

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

1. Clique em **Concluir**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Clique em **Aprovar e Fechar**.

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
