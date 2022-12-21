---
unique-page-id: 4720151
description: Implementação da RTP em páginas de aterrissagem do Marketo - Documentos do Marketo - Documentação do produto
title: Implementação da RTP em páginas de aterrissagem do Marketo
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Implementação da RTP em páginas de aterrissagem do Marketo {#implementing-rtp-on-marketo-landing-pages}

Para implementar sua tag RTP, siga as instruções de instalação abaixo:

1. Vá para o **Design Studio.** Abra o item que deseja editar. Selecionar **Ações do modelo**, selecione **Editar rascunho**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Faça alterações no modelo na **Origem HTML** guia .

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Na sua conta RTP, acesse **Configurações da conta**.

   a. Se você já recebeu sua tag JavaScript do Suporte - continue para a etapa 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. Em Domínio, localize o domínio relevante e clique em **Gerar tag**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copie a tag do JavaScript RTP e cole-a em todos os modelos de landing page entre a **`<head> </head>`** tags.

1. Clique em **Salvar** e **Fechar** a janela .

1. De volta ao **Design Studio**, aprove a landing page de **Ações do modelo**, clique em **Aprovar**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Por fim, você precisará **aprovar novamente** todas as landing pages que usam esse template para que o modelo tenha efeito. Você pode aprovar novamente todas de uma vez na seção Páginas de aterrissagem principal.

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Verifique se ele aparece em todas as páginas, incluindo landing pages e subdomínios.

   Você pode fazer isso clicando com o botão direito do mouse na página do seu site. Ir para **Exibir fonte da página.** Procurar por **RTP** para localizar a tag.
