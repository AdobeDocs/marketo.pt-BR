---
unique-page-id: 4720215
description: Implementação da RTP no Wordpress Enterprise - Documentos do Marketo - Documentação do produto
title: Implementação da RTP na Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---

# Implementação da RTP na Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Para implementar sua tag RTP, siga as instruções de instalação abaixo:

1. Ir para **Configurações da conta**.

   a. Se você já recebeu sua tag JavaScript do Suporte - continue para a etapa 3.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. Em Domínio, localize o domínio relevante e clique em **Gerar tag**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Copie a tag do JavaScript RTP.

1. Faça logon em sua conta do WordPress como usuário administrador

   a. Em **Aparência**, vá para **JavaScript personalizado**.
b. Cole a tag do Javascript RTP logo após o código existente.

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
