---
unique-page-id: 4720151
description: Implementação da RTP em Landings page de marketing - Documentos de marketing - Documentação do produto
title: Implementação da RTP em Landings page de marketing
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---


# Implementação do RTP em Landings page de marketing {#implementing-rtp-on-marketo-landing-pages}

Para implementar sua tag RTP, siga as instruções de instalação abaixo:

1. Vá para o **Design Studio.** Abra o item que deseja editar. Selecione **Ações do modelo**, selecione **Editar rascunho**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Faça as alterações no modelo na guia **HTML Source**.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Na sua conta RTP, vá para **Configurações da conta**.

   a. Se você já recebeu sua tag JavaScript do Suporte - continue com a etapa 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. Em Domínio, localize o domínio relevante e clique em **Gerar tag**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copie a tag RTP JavaScript e cole-a em todos os seus modelos de landing page entre as tags **`<head> </head>`**.

1. Clique em **Salvar** e **Fechar** na janela.

1. De volta ao **Design Studio**, aprove a landing page de **Ações de Modelo**, clique em **Aprovar**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Por fim, você precisará **reaprovar** todas as landings page que usam esse modelo para que as alterações de modelo entrem em vigor. Você pode aprová-los novamente de uma só vez na seção Landings page principal.

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Verifique se ele aparece em todas as páginas, incluindo landings page e subdomínios.

   Você pode fazer isso clicando com o botão direito do mouse na página do seu site. Vá para **Fonte de página de Visualização.** Procure  **** RTP para localizar a tag.
