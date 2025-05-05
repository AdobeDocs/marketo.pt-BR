---
unique-page-id: 4720145
description: Implementação do RTP usando o Google Tag Manager - Documentação do Marketo - Documentação do produto
title: Implementação do RTP usando o Google Tag Manager
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# Implementação do RTP usando o Google Tag Manager {#implementing-rtp-using-google-tag-manager}

Para implementar sua tag RTP, siga as instruções de instalação abaixo.

1. Faça logon em sua conta do Google Tag Manager.

1. Adicione uma nova tag > Configurações de tag > Tag de HTML personalizada&#x200B;**.** Chame de **RTP**.

1. Faça logon em sua conta RTP&#x200B;**.**

1. Vá para **Configurações da conta**.

   a. Se você já tiver recebido sua tag do JavaScript do Suporte, continue para a Etapa 6.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. Em Domínio, localize o domínio relevante e clique em **Gerar Marca**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Copie a tag RTP JavaScript e cole-a na nova **Tag HTML personalizada** que você criou (Etapa 1).

1. Clique em **+Adicionar Regra para Acionar Marca**. Selecione **Todas as páginas**.

1. Clique em **Salvar** e [publicar a nova versão](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Verifique se ele aparece em todas as páginas, incluindo páginas de aterrissagem e subdomínios.

   a. Para fazer isso, clique com o botão direito do mouse na página do site. Vá para **Inspect Element**, Pesquise por **RTP** para localizar a marca.
