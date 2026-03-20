---
unique-page-id: 4720215
description: Saiba mais sobre como implementar o rtp no wordpress enterprise no Marketo Engage, incluindo como implementar o rtp no wordpress. Use este guia para concluir a próxima etapa.
title: Implementação do RTP no Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
source-git-commit: 50befbf7339cd7a8b25b0942515497f6acc8f9ab
workflow-type: tm+mt
source-wordcount: '120'
ht-degree: 10%

---

# Implementação do RTP no Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Para implementar sua [!UICONTROL tag RTP], siga as instruções de instalação abaixo:

1. Vá para **[!UICONTROL Configurações da conta]**.

   a. Se você já tiver recebido sua tag do JavaScript do suporte, continue para a etapa 3.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. Em [!UICONTROL Domínio], localize o domínio relevante e clique em **[!UICONTROL Gerar Marca]**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Copie a tag RTP JavaScript.

1. Faça logon na sua conta [!DNL WordPress] como usuário administrador

   a. Em **[!UICONTROL Aparência]**, vá para **[!UICONTROL JavaScript Personalizado]**.
b. Cole a tag RTP Javascript logo após o código existente.

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >Ao colar o código, EXCLUA as seguintes tags:
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`
   >
   >Insira SOMENTE o próprio script.

1. Clique **[!UICONTROL Atualizar]**.
