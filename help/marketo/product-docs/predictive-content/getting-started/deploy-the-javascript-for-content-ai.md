---
unique-page-id: 11385053
description: Implantar o JavaScript para IA de conteúdo - Documentação do Marketo - Documentação do produto
title: Implantar o JavaScript para IA de conteúdo
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 1%

---

# Implantar o JavaScript para IA de conteúdo {#deploy-the-javascript-for-content-ai}

Para usar o Predictive Content, você precisa gerar e configurar a tag RTP (Web Personalization).

## Gerar marca {#generate-tag}

1. Faça logon na sua conta de conteúdo preditivo. Ir para **Configurações da conta**.

   ![](assets/settings-dropdown-account-hands.png)

1. Entrada **Configuração de domínio**, localize o domínio relevante e clique em **Gerar tag**.

   ![](assets/generate-tag.png)

1. Copie e cole a tag de Personalização da Web no HTML do seu site.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copie a tag JavaScript da Personalização da Web e cole-a como o primeiro script no cabeçalho de suas páginas, entre o `<head> </head>` específicos. Ver mais detalhes [instruções de implementação aqui](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Verifique se a tag é exibida em todas as páginas, incluindo páginas de aterrissagem e subdomínios. Verifique isso clicando com o botão direito do mouse na página do site. Ir para **Exibir fonte da página** em um navegador da Web. Pesquisa: &quot;RTP&quot;.

1. Confirme se o botão Tag está definido como **LIGADO**.
