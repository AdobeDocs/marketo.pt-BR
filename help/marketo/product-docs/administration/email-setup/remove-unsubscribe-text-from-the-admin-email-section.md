---
unique-page-id: 2360245
description: Remova o texto de cancelamento de inscrição da seção de email do administrador - Documentos do Marketo - Documentação do produto
title: Remova o texto de cancelamento de inscrição da seção Email de administrador
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# Remova o texto de cancelamento de inscrição da seção de email do administrador {#remove-unsubscribe-text-from-the-admin-email-section}

O único motivo pelo qual você deve remover completamente o conteúdo de cancelamento de inscrição da área &quot;Admin > Email&quot; é se estiver optando por criar o link de cancelamento de inscrição nos próprios modelos de email. A caixa de texto tem validação que não permite salvar sem conteúdo. Você pode contornar isso adicionando um pequeno comentário em HTML. O comentário HTML não será exibido no cliente de email, porque ele está renderizando o email em HTML e os comentários são omitidos. Aqui está como fazê-lo.

1. Vá para **Admin** e clique em **Email**.

   ![](assets/image2016-8-26-13-3a57-3a9.png)

1. Selecione todo o texto e pressione a tecla **Delete**.

   >[!CAUTION]
   >
   >Antes de excluir, copie/cole em um documento de texto como um backup.

1. Digite `<!--This is a comment -->`.

   ![](assets/image2016-8-26-13-3a53-3a15.png)

1. Clique em **Salvar alterações**.

   ![](assets/image2016-8-26-13-3a59-3a40.png)

>[!NOTE]
>
>Para o **Cancelar inscrição do texto** é necessário adicionar um único caractere. Use traço ou ponto.
