---
unique-page-id: 4720218
description: Implementação do RTP usando o Adobe Tag Manager - Documentos do Marketing - Documentação do produto
title: Implementação do RTP usando o Adobe Tag Manager
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# Implementação do RTP usando Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Para implementar sua tag RTP, siga as instruções de instalação abaixo:

1. Faça logon na sua conta RTP.
1. Vá para **Configurações da conta.**

   Se você já tiver recebido sua tag JavaScript do Suporte - continue com a etapa 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. Em Domínio, localize o domínio relevante e clique em **Gerar tag**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Faça logon em sua conta do Gerenciador dinâmico de tags ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).
1. Vá para **Painel.** Clique na propriedade da Web relevante.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Vá para **Regras,** clique em **Criar Nova Regra.**

1. Preencha o seguinte

   1. Nome: **Marketo RTP**
   1. Condições (recolher): Disparar regra em - **Parte superior da página**
   1. Javascript (recolher): clique em **Adicionar Novo Script**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Chame a nova tag: **Tag RTP do Marketo**
1. Remova o seguinte código da tag RTP

   * `<script type='text/javascript'>`
   * `</script>`

1. Cole a tag RTP JavaScript.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Certifique-se de remover todas as tags e deixar somente o próprio script (não `<script type='text/javascript'>` , `</script>` )

1. Clique em **Salvar código** no editor de scripts e **Salvar regra** no editor de regras.

1. No painel Regras, localize a regra de carregamento da página RTP do Marketo e, na lista suspensa **Ações**, selecione **Ativar regras**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **Verifique** se ele aparece em todas as páginas, incluindo landings page e subdomínios.

   Você pode fazer isso clicando com o botão direito do mouse nas páginas de seu site. Vá para **Elemento Inspect**, clique em **Rede, **Pesquisar: **RTP**.
