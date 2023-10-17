---
unique-page-id: 1146995
description: Usar tokens em etapas de fluxo - Documentação do Marketo - Documentação do produto
title: Usar tokens em etapas de fluxo
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 5%

---

# Usar tokens em etapas de fluxo {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[Adicionar uma etapa de fluxo a uma campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

Um token é uma variável. Você o usa em emails, Landing Pages e Campanhas inteligentes para facilitar sua vida. Você pode usar [Meus tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"} (tokens personalizados) em etapas de fluxo, webhooks, emails e landing pages. Você pode usar tokens para incluir conteúdo variável nestas etapas de fluxo:

* Alterar valor dos dados
* Alterar dados dos membros do programa
* Momento interessante
* Etapas da campanha do Salesforce (adicionar, remover, alterar status)
* Criar tarefa
* Enviar alerta (somente em Campanhas de acionamento)

1. Na etapa de fluxo, comece a digitar `{{` para obter categorias de token.

   ![](assets/image2014-9-22-14-3a3-3a17.png)

   >[!NOTE]
   >
   >Confira [Visão geral de tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} para obter uma lista de vários tokens disponíveis.

1. Continue a digitar até encontrar o token que deseja e clique para selecionar.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >Vários tokens podem ser usados nas etapas de fluxo Momento interessante, Criar tarefa e Enviar alerta.

   >[!NOTE]
   >
   >Os tokens de campo personalizado do membro do programa podem ser usados em: Criar tarefa, Criar tarefa no Microsoft, Momentos interessantes, Ações de fluxo Alterar valor de dados e Webhooks.

   Legal! Os dados serão extraídos do token quando a Campanha inteligente for executada.

   >[!MORELIKETHIS]
   >
   >* [Gerenciamento de meus tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
   >* [Compreender meus tokens em um programa](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"}
