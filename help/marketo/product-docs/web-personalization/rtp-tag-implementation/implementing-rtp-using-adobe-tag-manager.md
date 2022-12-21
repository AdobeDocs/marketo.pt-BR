---
unique-page-id: 4720218
description: Implementação da RTP usando Adobe Tag Manager - Marketo Docs - Documentação do produto
title: Implementação de RTP usando Adobe Tag Manager
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Implementação de RTP usando Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Para implementar sua tag RTP, siga as instruções de instalação abaixo:

1. Faça logon em sua conta RTP.

1. Ir para **Configurações da conta**.

   a. Se você já recebeu sua tag JavaScript do Suporte - continue para a etapa 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. Em Domínio, localize o domínio relevante e clique em **Gerar tag**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Faça logon em sua conta do Gerenciador dinâmico de tags ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Ir para **Painel.** Clique na propriedade da Web relevante.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Ir para **Regras**, clique em **Criar nova regra**.

1. Preencha o seguinte

   1. Nome: **Marketo RTP**
   1. Condições (recolher) : Acionar regra em - **Parte superior da página**
   1. Javascript (recolher): click **Adicionar novo script**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Chame a nova tag : **Tag Marketo RTP**

1. Remova o seguinte código da tag RTP

   * `<script type='text/javascript'>`
   * `</script>`

1. Cole a tag do JavaScript RTP.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Certifique-se de remover todas as tags e deixar somente o próprio script (não `<script type='text/javascript'>` , `</script>` )

1. Clique em **Salvar código** no editor de scripts e **Salvar regra** no editor de regras.

1. No painel Regras , localize a regra de carregamento da página RTP do Marketo e no **Ações** seleção suspensa **Ativar regras**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **Verificar** que aparece em todas as páginas, incluindo landing pages e subdomínios.

   Você pode fazer isso clicando com o botão direito do mouse nas páginas de seu site. Ir para **Elemento do Inspect**, clique em **Rede**, Pesquisa: **RTP**.
