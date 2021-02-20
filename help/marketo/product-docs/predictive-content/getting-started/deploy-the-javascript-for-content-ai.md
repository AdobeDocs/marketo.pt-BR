---
unique-page-id: 11385053
description: Implantar o JavaScript para o Content-AI - Documentos do Marketing - Documentação do produto
title: Implantar o JavaScript para Content-AI
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---


# Implantar o JavaScript para Content-AI {#deploy-the-javascript-for-content-ai}

Para usar o Conteúdo preditivo, é necessário gerar e configurar a tag RTP (Personalização da Web).

## Gerar tag {#generate-tag}

1. Faça logon em sua conta de Conteúdo previsível. Vá para **Configurações da conta**.

   ![](assets/settings-dropdown-account-hands.png)

1. Em **Configuração de domínio**, localize o domínio relevante e clique em **Gerar tag**.

   ![](assets/generate-tag.png)

1. Copie e cole a tag de Personalização da Web no HTML do seu site.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copie a tag JavaScript de personalização da Web e cole-a como o primeiro script no cabeçalho de suas páginas, entre as tags `<head> </head>`. Consulte [instruções de implementação mais detalhadas aqui](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Verifique se a tag aparece em todas as páginas, incluindo landings page e subdomínios. Verifique isso clicando com o botão direito do mouse na página do seu site. Vá para **Origem da página de Visualização** em um navegador da Web. Pesquisar: &quot;RTP&quot;.

1. Confirme se a opção Tag está definida como **ON**.
