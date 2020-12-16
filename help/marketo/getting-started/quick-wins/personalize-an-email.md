---
unique-page-id: 2359422
description: Personalizar um e-mail - Documentos do Marketing - Documentação do produto
title: Personalizar um email
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---


# Personalizar um email {#personalize-an-email}

## Missão: Torne seus emails pessoais adicionando tokens de dados {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configurar e adicionar uma pessoa](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)
>* [Enviar uma Explosão de Email](/help/marketo/getting-started/quick-wins/send-an-email.md)
>* [Derramamento, Derramamento, Enfermeira](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)


## Etapa 1: Selecione um email para personalizar {#step-select-an-email-to-personalize}

1. Selecione um dos emails de criação criados na vitória [rápida](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md) anterior e clique em **Editar rascunho**.

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >Isso cria uma cópia do email como rascunho. Você deve aprovar o rascunho para que as alterações entrem em vigor.

Se você não tiver ativado um bloqueador de pop-ups, o editor de e-mail será aberto em uma nova guia/janela. Caso contrário, clique duas vezes em **Editar rascunho** .

## Etapa 2: Transformar o vendedor no remetente {#step-make-the-salesperson-the-sender}

1. Selecione o campo **De** , realce e **exclua** o nome atual.

   ![](assets/two-5.png)

1. Clique no ícone **Token** à direita do campo **De** .

   ![](assets/three-4.png)

1. Localize e selecione o **`{{lead.Lead Owner First Name}}`** token.

   ![](assets/four-3.png)

1. Digite o nome da empresa e um traço para o Valor **** padrão para garantir que algo seja exibido caso o nome do representante de vendas não esteja disponível. Clique em **Inserir**.

   ![](assets/five-4.png)

1. Pressione a barra de espaço no campo **De** , certificando-se de que o cursor esteja piscando um espaço após o token inserido. Em seguida, clique novamente no ícone **Token** .

   ![](assets/six-4.png)

1. Localize e selecione o **`{{lead.Lead Owner Last Name}}`** token.

   ![](assets/seven-5.png)

1. Digite &quot;Sales&quot; para o Valor **** padrão e clique em **Insert**.

   ![](assets/eight-3.png)

## Etapa 3: Adicione o nome do cliente potencial ao email {#step-add-the-leads-name-to-the-email}

1. Selecione a seção editável superior, clique no ícone de engrenagem e selecione **Editar**.

   ![](assets/nine-2.png)

1. Adicione um espaço depois de &quot;Hello&quot;, posicione o cursor na frente da vírgula e clique no ícone **Inserir token** .

   ![](assets/ten-4.png)

1. Localize e selecione o **`{{lead.First Name}}`** token.

   ![](assets/eleven-4.png)

1. Digite &quot;Friend&quot; (ou qualquer rótulo que você gostaria) no campo Valor **** padrão e clique em **Inserir**.

   ![](assets/twelve-3.png)

   >[!TIP]
   >
   >Sempre incluir um valor padrão para tokens; isso garante que o valor padrão será exibido no email se alguma parte das informações pessoais estiver ausente.

1. Clique em **Salvar**.

   ![](assets/thirteen-3.png)

1. Feche a guia/janela do editor de email.

   ![](assets/fourteen-3.png)

1. Em Ações **de** email, selecione **Aprovar rascunho**.

   ![](assets/fifteen-3.png)

>[!TIP]
>
>Precisa de uma atualização rápida sobre como enviar o e-mail para você mesmo? Consulte [Enviar uma explosão](/help/marketo/getting-started/quick-wins/send-an-email.md)de email.

### Missão concluída {#mission-complete}

Parabéns, você personalizou seu email!

<br> 

[◄ Missão 6: Derramamento, Derramamento, Enfermeira](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Missão 8: Alerte o representante de vendas ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
