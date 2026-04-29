---
unique-page-id: 2360245
description: Remova o conteúdo padrão para cancelar a inscrição do email do administrador usando um comentário do HTML ao criar o link em modelos.
title: Remover texto de cancelamento de inscrição
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
source-git-commit: 9c4f0d0a43d3ef06132d827b605b9e42de712e22
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 7%

---

# Remover texto de cancelamento de inscrição {#remove-unsubscribe-text}

A única razão pela qual você deve remover completamente o conteúdo de cancelamento de inscrição da área **[!UICONTROL Administrador]** > **[!UICONTROL Email]** é se você optar por criar o link de cancelamento de inscrição nos próprios modelos de email. A caixa de texto tem uma validação que não permite salvar sem conteúdo. Você pode contornar isso adicionando um pequeno comentário do HTML. O comentário do HTML não será exibido no cliente de email, pois está renderizando o email no HTML e os comentários são omitidos.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Clique em **[!UICONTROL Email]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Selecione todo o texto e pressione a tecla **[!UICONTROL Delete]**.

   >[!CAUTION]
   >
   >Antes de excluir, copie/cole em um documento de texto como backup.

1. Digite em `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Clique em **[!UICONTROL Salvar alterações]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>Para o **Texto de Cancelamento de Inscrição**, é necessário adicionar um único caractere. Use um traço ou ponto.
