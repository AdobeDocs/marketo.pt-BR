---
unique-page-id: 2359644
description: Mostrar formulário HTML personalizado para pessoas conhecidas - Documentos do marketing - Documentação do produto
title: Mostrar formulário HTML personalizado para pessoas conhecidas
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# Mostrar formulário HTML personalizado para pessoas conhecidas {#show-custom-html-form-for-known-people}

Se um visitante estiver com cookies (pessoa conhecida que forneceu um endereço de email no passado), então por que se preocupar com o formulário? Dê a eles o botão de download. Veja como.

1. Vá para **Atividades de marketing**.

   ![](assets/login-marketing-activities-5.png)

1. Em **Atividades de marketing**, selecione o formulário e clique em **Editar formulário**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. Em **Configurações do formulário**, clique em **Configurações**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Definir se **Visitante conhecido, Mostrar**: para **HTML personalizado**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Clique em ![—](assets/image2014-9-25-14-3a1-3a26.png) para editar o **HTML personalizado** que será mostrado para pessoas conhecidas.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. Há algum conteúdo padrão, mas sinta-se à vontade para alterá-lo.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Tokens disponíveis:

   | Token | Descrição |
   |---|---|
   | `{{lead.FirstName}}` | Isso exibirá o nome da pessoa. |
   | `{{lead.LastName}}` | Isso exibirá o sobrenome da pessoa. |
   | `{{form.Button:default=Download}}` | Isso exibirá o botão de formulário. Substitua a área depois de `=` para alterar o texto do botão. |
   | `{{form.NotYou:default=Not you?}}` | Isso exibirá um link caso a pessoa seja outra pessoa. Substitua a área depois de `=` para alterar o texto do link. |

   >[!CAUTION]
   >
   >Somente os quatro tokens acima podem ser usados. Qualquer outro token não funcionará aqui.

1. Clique em **Concluir**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Clique em **Aprovar e Fechar**.

   >[!NOTE]
   >
   >O formulário deve ser aprovado para uso no landing page.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >Lembre-se de [aprovar o rascunho da landing page](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) criado pelas alterações de formulário.

   Pedaço de bolo! Verifique o que uma pessoa veria se voltasse ao mesmo formulário:

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >É possível direcionar o clique do botão para o ativo definindo a página de acompanhamento do formulário para o URL do arquivo.
