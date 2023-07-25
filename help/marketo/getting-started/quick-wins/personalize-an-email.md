---
unique-page-id: 2359422
description: Personalizar um email - Documentação do Marketo - Documentação do produto
title: Personalizar um e-mail
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 30%

---

# Personalizar um e-mail {#personalize-an-email}

## Missão: personalizar seus e-mails adicionando tokens de dados {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configurar e adicionar uma pessoa](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Enviar e-mail por meio de programa de envio](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [Promoção gota a gota](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}

## Etapa 1: selecionar um e-mail para personalizar {#step-select-an-email-to-personalize}

1. Selecione um dos emails de criação criados na [vitória rápida anterior](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"} e clique em **[!UICONTROL Criar rascunho]**.

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >Isso criará uma cópia do e-mail como rascunho. Lembre-se de aprovar o rascunho para que as alterações entrem em vigor.

Se você não tiver ativado um bloqueador de pop-ups, o editor de email será aberto em uma nova guia/janela. Caso contrário, clique **[!UICONTROL Criar rascunho]** duas vezes.

## Etapa 2: Transformar o Vendedor no Remetente {#step-make-the-salesperson-the-sender}

1. Selecione o **[!UICONTROL De]** campo, destaque e **excluir** o nome atual.

   ![](assets/personalize-an-email-2.png)

1. Clique em **Token** ícone à direita do **[!UICONTROL De]** campo.

   ![](assets/personalize-an-email-3.png)

1. Localize e selecione o **`{{lead.Lead Owner First Name}}`** token.

   ![](assets/personalize-an-email-4.png)

1. Digite o nome da sua empresa e um traço para a **Valor padrão** para garantir que algo seja exibido caso o nome do representante de venda não esteja disponível. Clique em **Inserir**.

   ![](assets/personalize-an-email-5.png)

1. Aperte a barra de espaço no **[!UICONTROL De]** , certificando-se de que o cursor pisca um espaço após o token que você acabou de inserir. Em seguida, clique no link **Token** ícone novamente.

   ![](assets/personalize-an-email-6.png)

1. Localize e selecione o **`{{lead.Lead Owner Last Name}}`** token.

   ![](assets/personalize-an-email-7.png)

1. Digite &quot;Vendas&quot; para o **Valor padrão** e clique em **Inserir**.

   ![](assets/personalize-an-email-8.png)

## Etapa 3: adicionar o nome do lead ao e-mail {#step-add-the-leads-name-to-the-email}

1. Selecione a seção editável superior, clique no ícone de engrenagem e selecione **[!UICONTROL Editar]**.

   ![](assets/personalize-an-email-9.png)

1. Adicione um espaço após &quot;Hello&quot;, coloque o cursor na frente da vírgula e clique no botão **Inserir token** ícone.

   ![](assets/personalize-an-email-10.png)

1. Localize e selecione o **`{{lead.First Name}}`** token.

   ![](assets/personalize-an-email-11.png)

1. Insira &quot;Friend&quot; (ou qualquer rótulo que desejar) na **[!UICONTROL Valor padrão]** e clique em **[!UICONTROL Inserir]**.

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >Sempre inclua um valor padrão para os tokens, pois isso garante que o valor padrão seja exibido no e-mail caso faltem algumas das informações pessoais.

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/personalize-an-email-13.png)

1. Em **[!UICONTROL Ações de email]** e selecione **[!UICONTROL Aprovar e fechar]**.

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>Precisa de uma dica rápida para lembrar como enviar o e-mail para si mesmo? Consulte [Enviar uma explosão de e-mail](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}.

### Missão cumprida {#mission-complete}

Parabéns, você personalizou seu e-mail! 

<br> 

[◄ Missão 6: promoção gota a gota](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Missão 8: alertar o representante de vendas ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
