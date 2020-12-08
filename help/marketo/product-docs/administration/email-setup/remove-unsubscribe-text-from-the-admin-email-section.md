---
unique-page-id: 2360245
description: Remova o texto de cancelamento de assinatura da seção "Admin -> Email" - Documentos do Marketing - Documentação do produto
title: Remova o texto de cancelamento de assinatura da seção "Admin -> Email"
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# Remova o texto de cancelamento de assinatura da seção &quot;Admin -> Email&quot; {#remove-unsubscribe-text-from-the-admin-email-section}

A única razão pela qual você deve remover completamente o conteúdo de cancelamento de inscrição da área &quot;Admin > Email&quot; é se estiver optando por criar o link de cancelamento de inscrição nos próprios modelos de email. A caixa de texto tem uma validação que não permite salvar sem nenhum conteúdo. Você pode contornar isso adicionando um pequeno comentário HTML. O comentário HTML não será exibido no cliente de email, pois ele está renderizando o email em HTML e os comentários são omitidos. Aqui está como fazer isso.

1. Vá para **Admin** e clique em **Email**.

   ![](assets/image2016-8-26-13-3a57-3a9.png)

1. Selecione todo o texto e pressione a tecla **Delete **key.

   >[!CAUTION]
   >
   >Antes de excluir, copie/cole em um documento de texto como backup.

1. Digite **<!--This is a comment -->**.

   ![](assets/image2016-8-26-13-3a53-3a15.png)

1. Clique em **Salvar alterações**.

   ![](assets/image2016-8-26-13-3a59-3a40.png)

>[!NOTE]
>
>Para **Cancelar inscrição de texto **é necessário adicionar um único caractere. Use um traço ou ponto final.

