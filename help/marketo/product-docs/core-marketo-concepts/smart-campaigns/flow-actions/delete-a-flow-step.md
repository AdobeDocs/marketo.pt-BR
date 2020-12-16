---
unique-page-id: 1146987
description: Excluir uma etapa de fluxo - Documentos do marketing - Documentação do produto
title: Excluir uma Etapa de Fluxo
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Excluir uma Etapa de Fluxo {#delete-a-flow-step}

>[!CAUTION]
>
>A remoção de etapas de fluxo, *especialmente etapas* de espera de campanhas inteligentes ativas, pode ter resultados inesperados. **Leia este artigo cuidadosamente.**

Primeiro vamos fazer o básico. Veja como remover um passo de fluxo indesejado de uma campanha inteligente. 1. No Fluxo de campanha inteligente, clique no ícone X para excluir qualquer etapa de fluxo.

![](assets/image2014-9-22-13-3a52-3a20.png)

1. Clique em **Excluir**.

   ![](assets/image2014-9-22-13-3a55-3a25.png)

   Simples e fácil, certo? Na maioria das vezes...

   >[!CAUTION]
   >
   >Excluir, adicionar e mover etapas dentro de uma campanha **ativa** pode ter resultados inesperados. Considere a criação de uma nova campanha, o teste e a troca.

   As alterações podem ser feitas em uma campanha ativa, mas podem ter consequências imprevistas. Estes são os detalhes:

   **Campanhas inteligentes em lote**

   Se sua campanha:

   1. **Nunca corri.** Faça todas as alterações desejadas. Não afetará ninguém até que você administre essa campanha.
   1. **É uma campanha inteligente recorrente.** As mudanças afetarão as pessoas nas execuções futuras, não nas execuções anteriores.
   1. **Já foi executado SEM passos de espera.** Nenhuma pessoa será afetada porque a campanha está inativa depois de correr.
   1. **Está correndo agora.** As alterações podem causar comportamento inesperado, dependendo do tempo e dos detalhes da exclusão. Recomendamos NÃO editar uma campanha em lote que esteja sendo executada ativamente. Para casos de emergência, aprenda a [abortar uma campanha](../../../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md)inteligente em andamento.

   1. **Já executou COM passos de espera.** Vários detalhes sobre este.\
      Quando uma pessoa entra em uma etapa de espera, ela diminui a duração e a ETAPA NÚMERO para voltar. Consulte o exemplo abaixo.

   **Acionar Campanhas inteligentes**

   1. **Sem passos de espera.** Se você excluir uma etapa normal, somente as pessoas que passarem pela campanha no futuro serão afetadas.
   1. **Com etapas de espera.** Consulte o exemplo abaixo para campanhas em lote. A mesma lógica se aplica.

   >[!NOTE]
   >
   >**Exemplo**
   >
   >    
   >    
   >1. Uma campanha inteligente tem três etapas.
   >
   >   * ETAPA 1. Enviar email nº 1
   >   * ETAPA 2. Aguardar 1 semana
   >   * ETAPA 3. Enviar email nº 2
   >
   >1. As pessoas que acessaram a **Etapa 2** esperarão 1 semana antes de seguir para a **Etapa 3**.
   >1. Você exclui a **Etapa 2** durante a semana.
   >1. As pessoas continuarão esperando a primeira semana. (Eles não voltam automaticamente para o fluxo.)
   >1. Quando eles finalmente retornarem, eles tentarão ir para a **Etapa 3**. Eles não vão encontrá-lo.
   >1. **IMPORTANTE:** Como agora existem apenas 2 etapas, as *pessoas não receberão o email nº 2.*


Fazendo alterações em uma Campanha ativa

Entenda este recurso e você principal campanhas inteligentes. Uau!
