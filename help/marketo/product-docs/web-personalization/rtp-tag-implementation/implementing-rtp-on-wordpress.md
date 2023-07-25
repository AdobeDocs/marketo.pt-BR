---
unique-page-id: 4720149
description: Implementação do RTP no Wordpress - Documentação do Marketo - Documentação do produto
title: Implementação de RTP no Wordpress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# Implementação de RTP no Wordpress {#implementing-rtp-on-wordpress}

Para implementar sua tag RTP, siga as instruções de instalação abaixo:

1. Abra o **header.php** arquivo de seu **Tema do WordPress**.

   Você pode usar um cliente FTP para acessar seu servidor ou editar seus arquivos de tema diretamente do painel do WordPress. O editor de arquivos está localizado no **Aparência** no menu da barra lateral.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. Na lista de arquivos de modelo à direita do editor de texto, localize **header.php** e abra-o.

1. Ir para **Configurações da conta**.

   a. Se você já tiver recebido a tag JavaScript do Suporte - continue para a etapa 5.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. Em Domínio, localize o domínio relevante e clique em **Gerar tag**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Copie a tag JavaScript do RTP e cole-a nos modelos do site.

   a. Certifique-se de que seja o primeiro script no cabeçalho da página - entre a tag **`<head> </head>`** específicos.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Clique em **Atualizar arquivo** para o arquivo header.php.

1. Verifique se ele aparece em todas as páginas, incluindo páginas de aterrissagem e subdomínios.

   a. Você pode fazer isso clicando com o botão direito do mouse na página do site. Ir para **Exibir fonte da página.** Pesquisar por **RTP** para localizar a tag.
