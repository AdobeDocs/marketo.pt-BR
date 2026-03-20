---
unique-page-id: 4720149
description: Saiba mais sobre a implementação de rtp no wordpress no Marketo Engage, incluindo a implementação de rtp no dnl wordpress. Use este guia para concluir a próxima etapa.
title: Implementação do RTP no Wordpress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 50befbf7339cd7a8b25b0942515497f6acc8f9ab
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 2%

---

# Implementando RTP em [!DNL Wordpress] {#implementing-rtp-on-wordpress}

Para implementar sua [!UICONTROL tag RTP], siga as instruções de instalação abaixo:

1. Abra o arquivo **header.php** do seu **[!DNL WordPress]tema**.

   Você pode usar um cliente FTP para acessar seu servidor ou editar seus arquivos de tema diretamente do painel do [!DNL WordPress]. O editor de arquivos está localizado na guia **[!UICONTROL Aparência]** do menu da barra lateral.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. Na lista de arquivos de modelo à direita do editor de texto, encontre **header.php** e abra-o.

1. Vá para **[!UICONTROL Configurações da conta]**.

   a. Se você já tiver recebido a tag do JavaScript do suporte, continue para a etapa 5.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. Em [!UICONTROL Domínio], localize o domínio relevante e clique em **[!UICONTROL Gerar Marca]**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Copie a tag RTP JavaScript e cole-a nos modelos do site.

   a. Verifique se esse é o primeiro script no cabeçalho da página - entre as tags **`<head> </head>`**.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Clique em **[!UICONTROL Atualizar arquivo]** para o arquivo header.php.

1. Verifique se ele aparece em todas as páginas, incluindo páginas de aterrissagem e subdomínios.

   a. Você pode fazer isso clicando com o botão direito do mouse na página do site. Vá para **[!UICONTROL Exibir Página Source].** Procure por **RTP** para localizar a marca.
