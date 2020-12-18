---
unique-page-id: 9437340
description: Implementação da RTP usando o Gerenciador de tags do Tealium - Documentos do Marketing - Documentação do produto
title: Implementação do RTP usando o Gerenciador de tags do Tealium
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Implementação do RTP usando o Gerenciador de tags do Tealium {#implementing-rtp-using-tealium-tag-manager}

Para implementar sua tag RTP, siga as instruções de instalação abaixo.

1. Faça logon em sua conta do Gerenciador de tags do Tealium.
1. Navegue até a guia Tags e adicione a Tag de Container personalizada do Tealium, localizada na guia Diversos do mercado de Tags.
1. No campo Título, digite **Marketo RTP** e clique em **Concluir**.
1. Salve as alterações.

   >[!NOTE]
   >
   >Ainda não há necessidade de publicar o novo container.

1. Depois que o perfil for salvo, clique no seu nome/endereço de email no canto superior direito do console do Tealium iQ.
1. No menu Admin, clique em **Gerenciar modelos** em Administrador de contas.
1. Selecione **Container Personalizado do Tealium: Marque para RTP** da lista suspensa para abrir o modelo de tag.
1. Faça logon na sua conta RTP.
1. Vá para Configurações da conta.

   >[!NOTE]
   >
   >Se você já tiver recebido sua tag JavaScript do Suporte, continue com a Etapa 11.

1. Em Domínio, localize o domínio relevante e clique em **Gerar tag**.
1. Copie a tag do JavaScript RTP e cole-a entre o Código da biblioteca de tags do Start e o Código da biblioteca de tags final no Modelo de Perfil do Tealium.

   >[!NOTE]
   >
   >**Etapas importantes**
   >
   >Remova as tags `<!-- RTP tag -->` e `<!-- End of RTP tag -->` do código inserido neste arquivo.
   >
   >Remova as tags `<script type='text/javascript'>` e `</script>` do código inserido neste arquivo.

1. **Clique em Salvar** modelo de Perfil e publique seu novo perfil.

