---
unique-page-id: 1900577
description: Criar um token de script de e-mail - Documentos do Marketo - Documentação do produto
title: Criar um token de script de email
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---


# Criar um token de script de email {#create-an-email-script-token}

Para desenvolvedores avançados, você pode usar scripts [](http://velocity.apache.org/engine/1.7/user-guide.html) Velocity em seus emails. Aqui está como fazer isso.

1. Vá para **Marketing Atividade**.

   ![](assets/ma.png)

1. Localize e selecione qualquer programa (Evento, Padrão ou Envolvimento, etc.).

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Na guia **Meus tokens** , arraste um token de script **de** email.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Nomeie seu token de script de email e **clique para editar** seu conteúdo.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Use a árvore à direita para arrastar os tokens **Pessoa, Oportunidade** ou Objeto **** personalizado.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Ao acessar uma matriz (oportunidade ou objeto personalizado), você está limitado aos 10 itens mais recentes associados à pessoa.

1. Observe que o token fica marcado/ativo depois de arrastá-lo para o editor de scripts.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >**Lembrete**
   >
   >
   >Se você estiver digitando tokens de forma livre, verifique/ative todos os tokens correspondentes na árvore ou eles serão tratados como texto sem formatação e não funcionarão.

1. Escreva seu script no Velocity. Estes são alguns recursos úteis:

   * [Documentação de scripts de e-mail para desenvolvedores de marketing](http://developers.marketo.com/email-scripting/)
   * [Guia do usuário Velocity](http://velocity.apache.org/engine/devel/user-guide.html)
   * [Guia de referência de velocidade](http://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity Tools Javadoc](http://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Quando o script for concluído, clique em **Salvar**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Clique em **Salvar** mais uma vez.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Agora você pode usar este token em seus emails. Ele executará o script sempre que um email for enviado.

>[!MORELIKETHIS]
>
>* [Adicionar um token de script de email ao seu email](add-an-email-script-token-to-your-email.md)

>



