---
unique-page-id: 4720145
description: Implementação da RTP usando o Google Tag Manager - Documentos da Marketo - Documentação do produto
title: Implementar a RTP usando o Gerenciador de tags da Google
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---

# Implementar a RTP usando o Gerenciador de tags da Google {#implementing-rtp-using-google-tag-manager}

Para implementar sua tag RTP, siga as instruções de instalação abaixo.

1. Faça logon em sua conta do Gerenciador de tags da Google.

1. Adicione uma nova tag > Configurações de tag > Tag HTML personalizada**.** Chame **RTP**.

1. Faça logon em sua conta RTP**.**

1. Ir para **Configurações da conta**.

   a. Se você já recebeu sua tag JavaScript do Suporte, continue para a Etapa 6.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. Em Domínio, localize o domínio relevante e clique em **Gerar tag**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Copie a tag do JavaScript RTP e cole-a no novo **Tag HTML personalizada** criado (Etapa 1).

1. Clique em **+Adicionar regra para acionar tag**. Selecionar **Todas as páginas**.

1. Clique em **Salvar** e [publicar a nova versão](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Verifique se ele aparece em todas as páginas, incluindo landing pages e subdomínios.

   a. Você pode fazer isso clicando com o botão direito do mouse na página do seu site. Ir para **Elemento do Inspect**, Pesquisar por **RTP** para localizar a tag.
