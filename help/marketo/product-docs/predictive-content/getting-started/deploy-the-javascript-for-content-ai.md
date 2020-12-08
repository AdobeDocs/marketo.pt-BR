---
unique-page-id: 11385053
description: Implantar o JavaScript para o Content-AI - Documentos do Marketing - Documentação do produto
title: Implantar o JavaScript para Content-AI
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# Implantar o JavaScript para Content-AI {#deploy-the-javascript-for-content-ai}

>[!NOTE]
>
>Dependendo da data de compra, sua subscrição de marketing pode incluir Conteúdo preditivo de marketing ou Conteúdo`<sup>AI</sup>`. Para os usuários do Predictive Content, o Marketo está habilitando os recursos do Content`<sup>AI</sup>` Analytics até 30 de abril de 2018. Para manter esses recursos além dessa data, entre em contato com o Gerente de sucesso do cliente do Marketo para atualizar para o Conteúdo`<sup>AI</sup>`do Marketing.

Para usar o Conteúdo preditivo, é necessário gerar e configurar o RTP (Personalização da Web) `tag.`

## Gerar tag {#generate-tag}

1. Faça logon em sua conta de Conteúdo previsível. Vá para Configurações **da** conta.

   ![](assets/settings-dropdown-account-hands.png)

1. Em Configuração **de** domínio, localize o domínio relevante e clique em **Gerar tag.**

   ![](assets/generate-tag.png)

1. Copie e cole a tag de Personalização da Web no HTML do seu site.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Copie a tag JavaScript de personalização da Web e cole-a como o primeiro script no cabeçalho de suas páginas, entre as `<head> </head>` tags. Consulte instruções de [implementação mais detalhadas aqui](http://docs.marketo.com/display/docs/rtp+tag+implementation) [.](http://pages2.marketo.com/rtp-implementation.html)

1. Verifique se a tag aparece em todas as páginas, incluindo landings page e subdomínios. Verifique isso clicando com o botão direito do mouse na sua `website’s` página. Vá para Fonte **da página de** Visualização em um navegador da Web. Pesquisar: &quot;RTP&quot;.
1. Confirme se a opção Tag está definida como **ON (Ativado)**.

