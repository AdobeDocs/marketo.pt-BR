---
unique-page-id: 4720218
description: Implementação do RTP usando o Adobe Tag Manager - Documentação do Marketo - Documentação do produto
title: Implementação do RTP usando o Adobe Tag Manager
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---

# Implementação do RTP usando o Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Para implementar sua tag RTP, siga as instruções de instalação abaixo:

1. Efetue login em sua conta RTP.

1. Vá para **[!UICONTROL Configurações da conta]**.

   a. Se você já tiver recebido sua tag do JavaScript do suporte, continue para a etapa 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. Em [!UICONTROL Domínio], localize o domínio relevante e clique em **[!UICONTROL Gerar Marca]**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Faça logon em sua conta do [!DNL Dynamic Tag Manager] ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Ir para **[!UICONTROL Painel].** Clique na propriedade da Web relevante.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Vá para **[!UICONTROL Regras]**, clique em **[!UICONTROL Criar nova regra]**.

1. Preencha o seguinte

   1. [!UICONTROL Nome]: **Marketo RTP**
   1. [!UICONTROL Condições] (recolher): regra de gatilho em - **[!UICONTROL Início da Página]**
   1. [!UICONTROL Javascript] (recolher): clique em **[!UICONTROL Adicionar novo script]**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Chame a nova marca: **Marca RTP do Marketo**

1. Remova o seguinte código da [!UICONTROL marca RTP]

   * `<script type='text/javascript'>`
   * `</script>`

1. Cole a tag RTP JavaScript.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Remova todas as marcas e deixe apenas o próprio script (sem `<script type='text/javascript'>` , `</script>` )

1. Clique em **[!UICONTROL Salvar Código]** no editor de scripts e em **[!UICONTROL Salvar Regra]** no editor de regras.

1. No painel Regras, localize a regra de carregamento de página do Marketo RTP e, na lista suspensa **[!UICONTROL Ações]**, selecione **[!UICONTROL Ativar regras]**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **[!UICONTROL Verifique]** se ele aparece em todas as páginas, incluindo páginas de aterrissagem e subdomínios.

   Você pode fazer isso clicando com o botão direito do mouse nas páginas do site. Vá para **[!UICONTROL Inspecionar Elemento]**, clique em **[!UICONTROL Rede]**, Pesquisar: **RTP**.
