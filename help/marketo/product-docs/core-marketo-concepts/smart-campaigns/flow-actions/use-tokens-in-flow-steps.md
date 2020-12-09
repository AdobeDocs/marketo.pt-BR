---
unique-page-id: 1146995
description: Usar tokens em etapas de fluxo - Documentos do marketing - Documentação do produto
title: Usar tokens em Etapas de Fluxo
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---


# Usar tokens em Etapas de Fluxo {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>* [Adicionar uma Etapa de fluxo a uma Campanha inteligente](add-a-flow-step-to-a-smart-campaign.md)


Um token é uma variável. Você o usa em [emails](https://docs.marketo.com/pages/viewpage.action?pageId=557076), [landings page](https://docs.marketo.com/pages/viewpage.action?pageId=2359689)e campanhas [](https://docs.marketo.com/display/DOCS/Smart+Lists+and+Lists) inteligentes para facilitar sua vida. Você pode usar [Meus tokens](../../../../product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) (tokens personalizados) em etapas de fluxo, webhooks, e-mails e landings page.  Você pode usar tokens para incluir conteúdo variável nessas etapas de fluxo:

* Alterar valor de dados
* Momento interessante
* Etapas de Campanha do Salesforce (adicionar, remover, alterar status)
* Criar Tarefa
* Enviar alerta (somente em campanhas de acionamento)

>[!NOTE]
>
>**Disponibilidade**
>
>Nem todos os clientes adquiriram essa funcionalidade. Entre em contato com seu representante de vendas para obter detalhes.

1. Na etapa de fluxo, digite o start `{{` para obter categorias de token. ![](assets/image2014-9-22-14-3a3-3a17.png)>

   >[!NOTE]
   >
   >**Mergulho profundo**
   >
   >Consulte Visão geral [dos](../../../../product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) tokens para obter uma lista de vários tokens disponíveis.

1. Continue digitando até encontrar o token desejado e clique para selecionar.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >Vários tokens podem ser usados em etapas interessantes de Momento, Criar Tarefa e Enviar alerta.

   >[!NOTE]
   >
   >**Artigos relacionados**
   >
   >* [Gerenciando Meus Tokens](../../../../product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [Como entender meus tokens em um Programa](../../../../product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)


Legal! Os dados serão obtidos do token quando a campanha inteligente for executada.