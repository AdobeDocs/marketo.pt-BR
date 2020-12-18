---
unique-page-id: 4720215
description: Implementação da RTP no Wordpress Enterprise - Documentos do Marketing - Documentação do produto
title: Implementação da RTP na Wordpress Enterprise
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---


# Implementando RTP no Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Para implementar sua tag RTP, siga as instruções de instalação abaixo:

1. Vá para** Configurações da conta.**

   1. Se você já tiver recebido sua tag JavaScript do Suporte - continue com a etapa 3.\
      ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. Em Domínio, localize o domínio relevante e clique em **Gerar tag**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Copie a tag RTP JavaScript.
1. Faça logon na sua conta do WordPress como Usuário administrador

   1. Em **Aparência**, vá para **JavaScript personalizado**.
   1. Cole a tag RTP Javascript logo após o código existente.

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
   >Insira o script SOMENTE.

1. Clique em **Atualizar**.
