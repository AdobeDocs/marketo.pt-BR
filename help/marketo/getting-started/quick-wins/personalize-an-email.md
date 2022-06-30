---
unique-page-id: 2359422
description: Personalizar um email - Documentos do Marketo - Documentação do produto
title: Personalizar um e-mail
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 30%

---

# Personalizar um e-mail {#personalize-an-email}

## Missão: personalizar seus e-mails adicionando tokens de dados {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configurar e adicionar uma pessoa](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [Enviar uma explosão de email](/help/marketo/getting-started/quick-wins/send-an-email.md){target=&quot;_blank&quot;}
>* [Depuração, Perfuração, Nurtura](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target=&quot;_blank&quot;}


## Etapa 1: selecionar um e-mail para personalizar {#step-select-an-email-to-personalize}

1. Selecione um dos emails de criação criados no [vitória rápida anterior](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target=&quot;_blank&quot;} e clique em **Editar rascunho**.

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >Isso criará uma cópia do e-mail como rascunho. Você deve aprovar o rascunho para que as alterações entrem em vigor.

Se você não tiver ativado um bloqueador de pop-ups, o editor de email será aberto em uma nova guia/janela. Caso contrário, clique em **Editar rascunho** duas vezes.

## Etapa 2: Transformar o Vendedor no Remetente {#step-make-the-salesperson-the-sender}

1. Selecione o **De** campo, destaque e **excluir** o nome atual.

   ![](assets/two-5.png)

1. Clique no botão **Token** à direita do **De** campo.

   ![](assets/three-4.png)

1. Encontre e selecione o **`{{lead.Lead Owner First Name}}`** token.

   ![](assets/four-3.png)

1. Digite o nome da sua empresa e um traço para a **Valor padrão** para garantir que algo seja exibido caso o nome do representante de venda não esteja disponível. Clique em **Inserir**.

   ![](assets/five-4.png)

1. Clique na barra de espaço no **De** , certificando-se de que o cursor esteja piscando um espaço após o token inserido. Em seguida, clique no botão **Token** ícone novamente.

   ![](assets/six-4.png)

1. Encontre e selecione o **`{{lead.Lead Owner Last Name}}`** token.

   ![](assets/seven-5.png)

1. Digite &quot;Vendas&quot; para a **Valor padrão** e clique em **Inserir**.

   ![](assets/eight-3.png)

## Etapa 3: adicionar o nome do lead ao e-mail {#step-add-the-leads-name-to-the-email}

1. Selecione a seção editável superior, clique no ícone de engrenagem e selecione **Editar**.

   ![](assets/nine-2.png)

1. Adicione um espaço depois de &quot;Hello&quot;, coloque o cursor na frente da vírgula e clique no botão **Inserir Token** ícone .

   ![](assets/ten-4.png)

1. Encontre e selecione o **`{{lead.First Name}}`** token.

   ![](assets/eleven-4.png)

1. Insira &quot;Amigo&quot; (ou qualquer rótulo que você desejar) no **Valor padrão** e clique em **Inserir**.

   ![](assets/twelve-3.png)

   >[!TIP]
   >
   >Sempre inclua um valor padrão para os tokens, pois isso garante que o valor padrão seja exibido no e-mail caso faltem algumas das informações pessoais.

1. Clique em **Salvar**.

   ![](assets/thirteen-3.png)

1. Feche a guia/janela do editor de email.

   ![](assets/fourteen-3.png)

1. Em **Ações de email**, selecione **Aprovar rascunho**.

   ![](assets/fifteen-3.png)

>[!TIP]
>
>Precisa de uma dica rápida para lembrar como enviar o e-mail para si mesmo? Consulte [Enviar uma explosão de email](/help/marketo/getting-started/quick-wins/send-an-email.md){target=&quot;_blank&quot;}.

### Missão cumprida {#mission-complete}

Parabéns, você personalizou seu e-mail! 

<br> 

[◄ Missão 6: promoção gota a gota](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Missão 8: alertar o representante de vendas ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
