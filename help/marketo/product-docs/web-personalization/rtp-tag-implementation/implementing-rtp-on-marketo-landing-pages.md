---
unique-page-id: 4720151
description: Implementação do RTP em páginas iniciais do Marketo - Documentação do Marketo - Documentação do produto
title: Implementação do RTP em páginas de aterrissagem do Marketo
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Implementação do RTP em páginas de aterrissagem do Marketo {#implementing-rtp-on-marketo-landing-pages}

Para implementar sua [!UICONTROL tag RTP], siga as instruções de instalação abaixo:

1. Vá para o **[!UICONTROL Design Studio].** Abra o item que deseja editar. Selecione **[!UICONTROL Ações do modelo]**, selecione **[!UICONTROL Editar rascunho]**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Faça alterações no modelo na guia **HTML Source**.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Na sua conta RTP, vá para **[!UICONTROL Configurações da Conta]**.

   a. Se você já tiver recebido a tag do JavaScript do suporte, continue para a etapa 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. Em [!UICONTROL Domínio], localize o domínio relevante e clique em **[!UICONTROL Gerar Marca]**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copie a marca RTP JavaScript e cole-a em todos os modelos de página de aterrissagem entre as marcas **`<head> </head>`**.

1. Clique em **[!UICONTROL Salvar]** e **[!UICONTROL Fechar]** a janela.

1. De volta ao **[!UICONTROL Design Studio]**, aprove a página de aterrissagem de **[!UICONTROL Ações de Modelo]**, clique em **[!UICONTROL Aprovar]**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Finalmente, você precisará **reaprovar** qualquer landing page que use esse template para que as alterações do template entrem em vigor. Você pode aprová-las novamente de uma só vez na seção principal de [!UICONTROL Páginas de Aterrissagem].

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Verifique se ele aparece em todas as páginas, incluindo páginas de aterrissagem e subdomínios.

   Você pode fazer isso clicando com o botão direito do mouse na página do site. Vá para **[!UICONTROL Exibir Página Source].** Procure por **[!UICONTROL RTP]** para localizar a marca.
