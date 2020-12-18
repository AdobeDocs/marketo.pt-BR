---
unique-page-id: 4720149
description: Implementação da RTP no Wordpress - Documentos do Marketing - Documentação do produto
title: Implementação da RTP no Wordpress
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---


# Implementação do RTP no Wordpress {#implementing-rtp-on-wordpress}

Para implementar sua tag RTP, siga as instruções de instalação abaixo:

1. Abra o arquivo **header.php** do tema do WordPress **.**

   Você pode usar um cliente FTP para acessar seu servidor ou editar seus arquivos de tema diretamente do painel do WordPress. Seu editor de arquivos está localizado na guia **Aparência** no menu da barra lateral.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. Na lista de arquivos de modelo à direita do editor de texto, localize **header.php** e abra-o.
1. Vá para **Configurações da conta.**

   Se você já recebeu sua tag JavaScript do Suporte - continue com a etapa 5.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. Em Domínio, localize o domínio relevante e clique em **Gerar tag**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Copie a tag RTP do JavaScript e cole-a nos modelos do site.

   Verifique se é o primeiro script no cabeçalho da página - entre as tags **`<head> </head>`**.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Clique em **Atualizar arquivo** para o arquivo header.php.
1. Verifique se ele aparece em todas as landings page e subdomínios `pages including`.

   Você pode fazer isso clicando com o botão direito do mouse na sua página `website’s`. Vá para **Fonte de página de Visualização.** Procure  **** RTP para localizar a tag.
