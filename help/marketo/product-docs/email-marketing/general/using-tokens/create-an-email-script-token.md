---
unique-page-id: 1900577
description: Criar um token de script de email - Documentação do Marketo - Documentação do produto
title: Criar um token de script de email
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 4%

---

# Criar um token de script de email {#create-an-email-script-token}

Para desenvolvedores avançados, você pode usar os [scripts do Velocity](https://velocity.apache.org/engine/1.7/user-guide.html) nos seus emails. Veja como fazer isso.

1. Vá para **[!UICONTROL Atividades de marketing]**.

   ![](assets/ma.png)

1. Localize e selecione qualquer programa (Evento, Padrão, Envolvimento etc.).

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Na guia **[!UICONTROL Meus tokens]**, arraste um token de **[!UICONTROL Script de email]**.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Nomeie seu token de script de email e **[!UICONTROL Clique para Editar]** seu conteúdo.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Use a árvore à direita para arrastar os tokens de **[!UICONTROL Pessoa]**, **[!UICONTROL Oportunidade]** ou **[!UICONTROL Objeto Personalizado]**.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Ao acessar uma matriz (oportunidade ou objeto personalizado), você está limitado aos 10 itens mais recentes associados à pessoa.

1. Observe que o token fica marcado/ativo depois de arrastá-lo para o editor de script.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >Se você estiver digitando tokens em formato livre, certifique-se de verificar/ativar todos os tokens correspondentes na árvore, caso contrário eles serão tratados como texto sem formatação e não funcionarão.

1. Escreva seu script no Velocity. Estes são alguns recursos úteis:

   * [Documentação de scripts de email de desenvolvedores do Marketo](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting)
   * [Guia do usuário do Velocity](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Guia de referência do Velocity](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Javadoc de ferramentas do Velocity](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Após concluir o script, clique em **[!UICONTROL Salvar]**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Clique em **[!UICONTROL Salvar]** mais uma vez.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Agora você pode usar esse token em seus emails. Ele executará o script toda vez que um email for enviado.

>[!MORELIKETHIS]
>
>[Adicionar um token de script de email ao seu email](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
