---
unique-page-id: 4720151
description: Implementação do RTP em páginas iniciais do Marketo - Documentação do Marketo - Documentação do produto
title: Implementação do RTP em páginas de aterrissagem do Marketo
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Implementação do RTP em páginas de aterrissagem do Marketo {#implementing-rtp-on-marketo-landing-pages}

Para implementar sua tag RTP, siga as instruções de instalação abaixo:

1. Vá para o **Design Studio.** Abra o item que deseja editar. Selecione **Ações do modelo**, selecione **Editar rascunho**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Faça as alterações no modelo na guia **HTML Source**.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Na sua conta RTP, vá para **Configurações da Conta**.

   a. Se você já tiver recebido a tag do JavaScript do suporte, continue para a etapa 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. Em Domínio, localize o domínio relevante e clique em **Gerar Marca**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copie a marca RTP JavaScript e cole-a em todos os modelos de página de aterrissagem entre as marcas **`<head> </head>`**.

1. Clique em **Salvar** e **Fechar** a janela.

1. De volta ao **Design Studio**, aprove a página de aterrissagem de **Ações de Modelo**, clique em **Aprovar**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Finalmente, você precisará **reaprovar** qualquer landing page que use esse template para que as alterações do template entrem em vigor. É possível aprovar novamente todas de uma só vez na seção principal das Páginas de aterrissagem.

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Verifique se ele aparece em todas as páginas, incluindo páginas de aterrissagem e subdomínios.

   Você pode fazer isso clicando com o botão direito do mouse na página do site. Vá para **Exibir Página Source.** Procure por **RTP** para localizar a marca.
