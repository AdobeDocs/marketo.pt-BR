---
unique-page-id: 1146987
description: Excluir uma etapa do fluxo - Documentação do Marketo - Documentação do produto
title: Excluir uma etapa do fluxo
exl-id: 039a1e80-48cc-47f9-9e1a-459f89bf0730
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Excluir uma etapa do fluxo {#delete-a-flow-step}

>[!CAUTION]
>
>Remoção de etapas de fluxo, _especialmente as etapas de espera_ em campanhas inteligentes ativas, pode ter resultados inesperados. **Leia este artigo cuidadosamente.**

Primeiro, vamos fazer o básico. Veja como remover uma etapa de fluxo indesejada de uma campanha inteligente. 1. No Fluxo da campanha inteligente, clique no ícone X para excluir qualquer etapa do fluxo.

![](assets/image2014-9-22-13-3a52-3a20.png)

1. Clique em **Excluir**.

   ![](assets/image2014-9-22-13-3a55-3a25.png)

   Simples e fácil, certo? Na maioria das vezes...

   >[!CAUTION]
   >
   >Excluir, adicionar e mover etapas dentro de um **ativo** a campanha pode definitivamente ter resultados inesperados. Considere criar uma nova campanha, testá-la e depois alternar.

   As alterações podem ser feitas em uma campanha ativa, mas podem ter consequências imprevistas. Veja os detalhes:

   **Campanhas inteligentes em lote**

   Se sua campanha:

   1. **Nunca corri.** Faça todas as alterações desejadas. Não afetará ninguém até você dirigir essa campanha.
   1. **É uma campanha inteligente recorrente.** As alterações afetarão as pessoas nas execuções futuras, não nas execuções anteriores.
   1. **Já executado SEM etapas de espera.** Nenhuma pessoa será afetada porque a campanha está inativa após a execução.
   1. **O está em execução agora.** As alterações podem causar comportamento inesperado, dependendo do tempo e dos detalhes da exclusão. Recomendamos NÃO editar uma campanha em lote que esteja em execução ativamente. Para casos de emergência, saiba como [abortar uma campanha inteligente em execução](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md).

   1. **Já executado COM etapas de espera.** Vários detalhes sobre este.\
      Quando uma pessoa insere uma etapa de espera, ela anota a duração e a QUAL ETAPA NUMÉRICA retornar. Veja o exemplo abaixo.

   **Acionar campanhas inteligentes**

   1. **Nenhuma etapa de espera.** Se você excluir uma etapa normal, somente as pessoas que executarão a campanha no futuro serão afetadas.
   1. **Com passos de espera.** Consulte o exemplo abaixo para campanhas em lote. A mesma lógica se aplica.

   >[!NOTE]
   >
   >**Exemplo**
   >
   >1. Uma campanha inteligente tem 3 etapas.
   >    * ETAPA 1. Enviar e-mail #1
   >    * ETAPA 2. Aguardar 1 semana
   >    * ETAPA 3. Enviar e-mail #2
   >
   >1. Pessoas que atingiram **Etapa 2** aguardará 1 semana antes de passar para a **Etapa 3**.
   >1. Você exclui **Etapa 2** durante a semana.
   >1. As pessoas continuarão a esperar a 1 semana. (Eles não voltam automaticamente ao fluxo.)
   >1. Quando eles finalmente voltarem, eles tentarão ir para **Etapa 3**. Eles não vão encontrá-lo.
   >1. **IMPORTANTE:** Uma vez que agora existem apenas 2 etapas, a *as pessoas não receberão o email #2.*

Fazer alterações em uma campanha ativa

Entenda esse recurso e você principal campanhas inteligentes.
