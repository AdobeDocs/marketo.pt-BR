---
unique-page-id: 9437340
description: Implementação da RTP usando o Gerenciador de tag do Tealium - Documentos da Marketo - Documentação do produto
title: Implementando a RTP usando o Gerenciador de tag do Tealium
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Implementando a RTP usando o Gerenciador de tag do Tealium {#implementing-rtp-using-tealium-tag-manager}

Para implementar sua tag RTP, siga as instruções de instalação abaixo.

1. Faça logon em sua conta do Gerenciador de tags do Tealium.

1. Navegue até a guia Tags e adicione a Tag do contêiner personalizado do tealium, localizada na guia Misc do mercado Tags .

1. No campo Título , informe **Marketo RTP** e clique em **Concluir**.

1. Salve as alterações.

   >[!NOTE]
   >
   >Ainda não há necessidade de publicar o novo contêiner.

1. Depois que o perfil for salvo, clique em seu nome/endereço de email no canto superior direito do console do Tealium iQ.

1. No menu Admin, clique em **Gerenciar modelos** em Account Admin.

1. Selecionar **Contêiner personalizado do tealium: Marketo RTP** na lista suspensa para abrir o modelo Tag .

1. Faça logon em sua conta RTP.

1. Vá para Configurações da conta.

   >[!NOTE]
   >
   >Se você já recebeu sua tag JavaScript do Suporte, continue para a Etapa 11.

1. Em Domínio, localize o domínio relevante e clique em **Gerar tag**.

1. Copie a tag do JavaScript RTP e cole-a entre o Código inicial da biblioteca de tags e o Código final da biblioteca de tags no Modelo de perfil do tealium.

   >[!NOTE]
   >
   >**Etapas importantes**
   >
   >Remova o `<!-- RTP tag -->` e `<!-- End of RTP tag -->` tags do código inserido neste arquivo.
   >
   >Remova qualquer `<script type='text/javascript'>` e `</script>` tags do código inserido neste arquivo.

1. **Clique em Salvar modelo de perfil** e publicar seu novo perfil.
