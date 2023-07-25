---
unique-page-id: 9437340
description: Implementação do RTP usando o Tealium Tag Manager - Documentação do Marketo - Documentação do produto
title: Implementação do RTP usando o Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Implementação do RTP usando o Tealium Tag Manager {#implementing-rtp-using-tealium-tag-manager}

Para implementar sua tag RTP, siga as instruções de instalação abaixo.

1. Faça logon na sua conta do Tealium Tag Manager.

1. Navegue até a guia Tags e adicione a Tag de contêiner personalizado Tealium, localizada na guia Diversos do marketplace Tags.

1. No campo Título, informe **MARKETO RTP** e clique em **Concluir**.

1. Salve as alterações.

   >[!NOTE]
   >
   >Não há necessidade de publicar o novo contêiner ainda.

1. Depois que o perfil for salvo, clique em seu nome/endereço de email no canto superior direito do console iQ do Tealium.

1. No menu Admin, clique em **Gerenciar modelos** em Administrador da conta.

1. Selecionar **Contêiner personalizado Tealium: Marketo RTP** na lista suspensa para abrir o Modelo de tag.

1. Efetue login em sua conta RTP.

1. Vá para Configurações da conta.

   >[!NOTE]
   >
   >Se você já recebeu a tag JavaScript do suporte, continue para a Etapa 11.

1. Em Domínio, localize o domínio relevante e clique em **Gerar tag**.

1. Copie a tag JavaScript RTP e cole-a entre Iniciar código da biblioteca de tags e Encerrar código da biblioteca de tags no modelo de perfil do Tálium.

   >[!NOTE]
   >
   >**Etapas importantes**
   >
   >Remova o `<!-- RTP tag -->` e `<!-- End of RTP tag -->` do código que você insere nesse arquivo.
   >
   >Remover qualquer `<script type='text/javascript'>` e `</script>` do código que você insere nesse arquivo.

1. **Clique em Salvar modelo de perfil** e publique seu novo perfil.
