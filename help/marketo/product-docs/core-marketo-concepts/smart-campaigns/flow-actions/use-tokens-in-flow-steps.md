---
unique-page-id: 1146995
description: Usar tokens nas etapas do fluxo - Documentos do Marketo - Documentação do produto
title: Usar tokens em etapas do fluxo
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
source-git-commit: 46812deb41ed56328a4a64fbd36340d13c50dde4
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 5%

---

# Usar tokens em etapas do fluxo {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[Adicionar uma etapa de fluxo a uma campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

Um token é uma variável. Você o usa em emails, landing pages e campanhas inteligentes para facilitar a vida. Você pode usar [Meus tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) (tokens personalizados) em etapas de fluxo, webhooks, emails e landing pages. Você pode usar tokens para incluir conteúdo variável nessas etapas de fluxo:

* Alterar valor dos dados
* Alterar dados dos membros do programa
* Momento interessante
* Etapas da campanha do Salesforce (adicionar, remover, alterar status)
* Criar tarefa
* Enviar alerta (somente em campanhas acionadoras)

1. Na etapa do fluxo, comece a digitar `{{` para obter categorias de token.

   ![](assets/image2014-9-22-14-3a3-3a17.png)

   >[!NOTE]
   >
   >Confira [Visão geral de tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) para obter uma lista de vários tokens disponíveis.

1. Continue digitando até encontrar o token desejado e clique para selecionar.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >Vários tokens podem ser usados nas etapas do fluxo Momento interessante, Criar tarefa e Enviar alerta .

   >[!NOTE]
   >
   >Tokens de campo personalizado de membro do programa podem ser usados em: Criar tarefa, Criar tarefa na Microsoft, Momentos interessantes, Alterar ações de fluxo do valor de dados e Webhooks.

   Legal! Os dados serão obtidos do token quando a campanha inteligente for executada.

   >[!MORELIKETHIS]
   >
   >* [Gerenciar meus tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [Noções básicas sobre meus tokens em um programa](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)

