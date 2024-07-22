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

1. Faça logon na sua conta de conteúdo preditivo. Vá para **Configurações da conta**.

   ![](assets/settings-dropdown-account-hands.png)

1. Em **Configuração de Domínio**, localize o domínio relevante e clique em **Gerar Marca**.

   ![](assets/generate-tag.png)

1. Copie e cole a tag do Web Personalization na HTML do site.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copie a marca JavaScript do Web Personalization e cole-a como o primeiro script no cabeçalho de suas páginas, entre as marcas `<head> </head>`. Veja mais [instruções de implementação detalhadas aqui](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Verifique se a tag é exibida em todas as páginas, incluindo páginas de aterrissagem e subdomínios. Verifique isso clicando com o botão direito do mouse na página do site. Vá para **Exibir Página Source** em um navegador da Web. Pesquisa: &quot;RTP&quot;.

1. Confirme se o botão de alternância de Marca está definido como **ON**.
