---
unique-page-id: 4720218
description: Implementação do RTP usando o Adobe Tag Manager - Documentação do Marketo - Documentação do produto
title: Implementação do RTP usando o Adobe Tag Manager
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Implementação do RTP usando o Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Para implementar sua tag RTP, siga as instruções de instalação abaixo:

1. Efetue login em sua conta RTP.

1. Ir para **Configurações da conta**.

   a. Se você já tiver recebido a tag JavaScript do Suporte - continue para a etapa 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. Em Domínio, localize o domínio relevante e clique em **Gerar tag**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Faça logon em sua conta do Dynamic Tag Manager ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Ir para **Painel.** Clique em na propriedade da Web relevante.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Ir para **Regras**, clique em **Criar nova regra**.

1. Preencha o seguinte

   1. Nome: **MARKETO RTP**
   1. Condições (recolher): acionar regra em - **Início da página**
   1. Javascript (recolher): clique **Adicionar novo script**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Chame a nova tag: **Tag Marketo RTP**

1. Remova o seguinte código da tag RTP

   * `<script type='text/javascript'>`
   * `</script>`

1. Cole a tag JavaScript do RTP.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Remova todas as tags e deixe apenas o próprio script (não `<script type='text/javascript'>` , `</script>` )

1. Clique em **Salvar código** no editor de scripts e **Salvar regra** no editor de regras.

1. No painel Regras, localize a regra de carregamento de página do Marketo RTP e, na guia **Ações** seleção suspensa **Ativar regras**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **Verificar** que ele aparece em todas as páginas, incluindo páginas de aterrissagem e subdomínios.

   Você pode fazer isso clicando com o botão direito do mouse nas páginas do site. Ir para **Elemento Inspect**, clique em **Rede**, Pesquisar: **RTP**.
