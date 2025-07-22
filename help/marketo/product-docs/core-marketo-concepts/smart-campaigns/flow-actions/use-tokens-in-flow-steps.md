---
unique-page-id: 1146995
description: Usar tokens em etapas de fluxo - Documentação do Marketo - Documentação do produto
title: Usar tokens em etapas de fluxo
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
feature: Smart Campaigns
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 5%

---

# Usar tokens em etapas de fluxo {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[Adicionar uma Etapa de Fluxo a uma Campanha Inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

Um token é uma variável. Você o usa em emails, Landing Pages e Campanhas inteligentes para facilitar sua vida. Você pode usar [Meus tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"} (tokens personalizados) em etapas de fluxo, webhooks, emails e páginas de aterrissagem. Você pode usar tokens para incluir conteúdo variável nestas etapas de fluxo:

* Alterar valor dos dados
* Alterar dados dos membros do programa
* Momento interessante
* [!DNL Salesforce] Etapas da campanha (adicionar, remover, alterar status)
* Criar tarefa
* Enviar alerta (somente em Campanhas de acionamento)

1. Na etapa de fluxo, comece digitando `{{` para obter categorias de token.

   ![](assets/use-tokens-in-flow-steps-1.png)

   >[!NOTE]
   >
   >Confira a [Visão geral dos tokens](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} para obter uma lista de vários tokens disponíveis.

1. Continue a digitar até encontrar o token que deseja e clique para selecionar.

   ![](assets/use-tokens-in-flow-steps-2.png)

   >[!TIP]
   >
   >Vários tokens podem ser usados nas etapas de fluxo Momento interessante, Criar tarefa e Enviar alerta.

   >[!NOTE]
   >
   >Os tokens de campo personalizado do membro do programa podem ser usados em: Criar tarefa, Criar tarefa no Microsoft, Momentos interessantes, Ações de fluxo Alterar valor de dados e Webhooks.

   Legal! Os dados serão extraídos do token quando a Campanha inteligente for executada.

   >[!MORELIKETHIS]
   >
   >* [Gerenciando Meus Tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
   >* [Compreendendo Meus Tokens em um Programa](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"}
