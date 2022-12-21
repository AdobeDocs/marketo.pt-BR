---
unique-page-id: 2360245
description: Remova o texto de cancelamento de inscrição da seção de email do administrador - Documentos do Marketo - Documentação do produto
title: Remova o texto de cancelamento de inscrição da seção Email de administrador
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Remova o texto de cancelamento de inscrição da seção Email de administrador {#remove-unsubscribe-text-from-the-admin-email-section}

O único motivo pelo qual você deve remover completamente o conteúdo de cancelamento de inscrição da área &quot;Admin > Email&quot; é se estiver optando por criar o link de cancelamento de inscrição nos próprios modelos de email. A caixa de texto tem validação que não permite salvar sem conteúdo. Você pode contornar isso adicionando um pequeno comentário de HTML. O comentário do HTML não será exibido no cliente de email, pois ele está renderizando o email no HTML e os comentários são omitidos. Aqui está como fazê-lo.

1. Vá para o **Administrador** área.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Clique em **Email**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Selecione todo o texto e pressione a tecla **Excluir** chave.

   >[!CAUTION]
   >
   >Antes de excluir, copie/cole em um documento de texto como um backup.

1. Digite `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Clique em **Salvar alterações**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>Para o **Cancelar assinatura do texto** é necessário adicionar um único caractere. Use traço ou ponto.
