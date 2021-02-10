---
unique-page-id: 1900577
description: Criar um token de script de e-mail - Documentos do Marketo - Documentação do produto
title: Criar um token de script de email
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---


# Criar um token de script de email {#create-an-email-script-token}

Para desenvolvedores avançados, você pode usar [scripts Velocity](https://velocity.apache.org/engine/1.7/user-guide.html) em seus emails. Aqui está como fazer isso.

1. Vá para **Atividades de marketing**.

   ![](assets/ma.png)

1. Localize e selecione qualquer programa (Evento, Padrão ou Envolvimento, etc.).

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Na guia **Meus tokens**, arraste um token **Script de e-mail**.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Nomeie seu token de script de email e **clique para editar** seu conteúdo.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Use a árvore à direita para arrastar os tokens **Pessoa, Oportunidade** ou **Objeto Personalizado**.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Ao acessar uma matriz (oportunidade ou objeto personalizado), você está limitado aos 10 itens mais recentes associados à pessoa.

1. Observe que o token fica marcado/ativo depois de arrastá-lo para o editor de scripts.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >Se você estiver digitando tokens de forma livre, verifique/ative todos os tokens correspondentes na árvore ou eles serão tratados como texto sem formatação e não funcionarão.

1. Escreva seu script no Velocity. Estes são alguns recursos úteis:

   * [Documentação de scripts de e-mail para desenvolvedores de marketing](https://developers.marketo.com/email-scripting/)
   * [Guia do usuário Velocity](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Guia de referência de velocidade](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity Tools Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Depois que o script for concluído, clique em **Salvar**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Clique em **Salvar** mais uma vez.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Agora você pode usar este token em seus emails. Ele executará o script sempre que um email for enviado.

>[!MORELIKETHIS]
>
>[Adicionar um token de script de email ao seu email](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
