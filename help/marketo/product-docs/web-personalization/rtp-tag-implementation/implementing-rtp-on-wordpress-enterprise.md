---
unique-page-id: 4720215
description: Implementação do RTP no Wordpress Enterprise - Documentação do Marketo - Documentação do produto
title: Implementação do RTP no Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Implementação do RTP no Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Para implementar sua tag RTP, siga as instruções de instalação abaixo:

1. Vá para **Configurações da conta**.

   a. Se você já tiver recebido sua tag do JavaScript do suporte, continue para a etapa 3.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. Em Domínio, localize o domínio relevante e clique em **Gerar Marca**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Copie a tag RTP JavaScript.

1. Faça logon na sua conta do WordPress como usuário administrador

   a. Em **Aparência**, vá para **JavaScript Personalizado**.
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

1. Clique em **Atualizar**.
