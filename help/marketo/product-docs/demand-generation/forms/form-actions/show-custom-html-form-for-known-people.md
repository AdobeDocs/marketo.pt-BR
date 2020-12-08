---
unique-page-id: 2359644
description: Mostrar formulário HTML personalizado para pessoas conhecidas - Documentos do marketing - Documentação do produto
title: Mostrar formulário HTML personalizado para pessoas conhecidas
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# Mostrar formulário HTML personalizado para pessoas conhecidas {#show-custom-html-form-for-known-people}

Se um visitante estiver com cookies (pessoa conhecida que forneceu um endereço de email no passado), então por que se preocupar com o formulário? Dê a eles o botão de download. Veja como.

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

1. Vá para **Marketing** **Atividade**.

   ![](assets/login-marketing-activities-5.png)

1. Em **Marketing** **Atividade**, selecione seu formulário e clique em **Editar** **formulário**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. Em **Configurações de** formulário ****, clique em **Configurações**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Defina Se **Conhecido** O **Visitante, Mostrar**: para **Personalizar** **HTML**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Clique em ![—](assets/image2014-9-25-14-3a1-3a26.png) para editar o **HTML** **personalizado** que será exibido para pessoas conhecidas.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. Há algum conteúdo padrão, mas sinta-se à vontade para alterá-lo.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Tokens disponíveis:

   | Token | Descrição |
   |---|---|
   | `{{lead.FirstName}}` | Isso exibirá o nome da pessoa. |
   | `{{lead.LastName}}` | Isso exibirá o sobrenome da pessoa. |
   | `{{form.Button:default=Download}}` | Isso exibirá o botão de formulário. Substitua a área depois do botão `=` para alterar o texto do botão. |
   | `{{form.NotYou:default=Not you?}}` | Isso exibirá um link caso a pessoa seja outra pessoa. Substitua a área depois do link `=` para alterar o texto do link. |

   >[!CAUTION]
   >
   >Somente os quatro tokens acima podem ser usados. Qualquer outro token não funcionará aqui.

1. Clique em **Concluir**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Clique em **Aprovar e fechar**.

   >[!NOTE]
   >
   >O formulário deve ser aprovado para uso no landing page.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >**Lembrete**
   >
   >
   >Lembre-se de [aprovar o rascunho](../../../../product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) de landing page criado pelas alterações de formulário.

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >É possível direcionar o clique do botão para o ativo definindo a página de acompanhamento do formulário para o URL do arquivo.

Pedaço de bolo! Verifique o que uma pessoa veria se voltasse ao mesmo formulário: