---
unique-page-id: 4720151
description: Implementação do RTP em páginas iniciais do Marketo - Documentação do Marketo - Documentação do produto
title: Implementação do RTP em páginas de aterrissagem do Marketo
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Implementação do RTP em páginas de aterrissagem do Marketo {#implementing-rtp-on-marketo-landing-pages}

Para implementar sua tag RTP, siga as instruções de instalação abaixo:

1. Vá para a **Design Studio.** Abra o item que deseja editar. Selecionar **Ações do modelo**, selecione **Editar rascunho**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Faça as alterações no modelo no **Origem do HTML** guia.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Na sua conta RTP, acesse **Configurações da conta**.

   a. Se você já tiver recebido a tag JavaScript do Suporte - continue para a etapa 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. Em Domínio, localize o domínio relevante e clique em **Gerar tag**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copie a tag RTP JavaScript e cole-a em todos os templates de landing page entre a tag **`<head> </head>`** específicos.

1. Clique em **Salvar** e **Fechar** a janela.

1. De volta ao **Design Studio**, aprove a landing page de **Ações do modelo**, clique em **Aprovar**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Por fim, será necessário **reaprovar** as landing pages que usam esse template para que as alterações no template entrem em vigor. É possível aprovar novamente todas de uma só vez na seção principal das Páginas de aterrissagem.

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Verifique se ele aparece em todas as páginas, incluindo páginas de aterrissagem e subdomínios.

   Você pode fazer isso clicando com o botão direito do mouse na página do site. Ir para **Exibir fonte da página.** Pesquisar por **RTP** para localizar a tag.
