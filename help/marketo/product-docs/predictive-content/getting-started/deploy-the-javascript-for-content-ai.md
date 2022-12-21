---
unique-page-id: 11385053
description: Implante o JavaScript para Content-AI - Documentos do Marketo - Documentação do produto
title: Implantar o JavaScript para Content-AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 1%

---

# Implantar o JavaScript para Content-AI {#deploy-the-javascript-for-content-ai}

Para usar o Conteúdo preditivo, você precisa gerar e configurar a tag RTP (Personalização da Web).

## Gerar marca {#generate-tag}

1. Faça logon na sua conta de Conteúdo preditivo . Ir para **Configurações da conta**.

   ![](assets/settings-dropdown-account-hands.png)

1. Em **Configuração de domínio**, localize o domínio relevante e clique em **Gerar tag**.

   ![](assets/generate-tag.png)

1. Copie e cole a tag Web Personalization no HTML de seu site.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copie a tag JavaScript de personalização da Web e cole-a como o primeiro script no cabeçalho de suas páginas, entre as `<head> </head>` tags. Veja mais detalhes [instruções de implementação aqui](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Verifique se a tag aparece em todas as páginas, incluindo landing pages e subdomínios. Verifique isso clicando com o botão direito do mouse na página do seu site. Ir para **Exibir origem da página** em um navegador da Web. Pesquisar: &quot;RTP&quot;.

1. Confirme se o botão Tag está definido como **ATIVADO**.
