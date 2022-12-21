---
unique-page-id: 1146987
description: Excluir uma etapa do fluxo - Documentos do Marketo - Documentação do produto
title: Excluir uma etapa do fluxo
exl-id: 039a1e80-48cc-47f9-9e1a-459f89bf0730
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Excluir uma etapa do fluxo {#delete-a-flow-step}

>[!CAUTION]
>
>Remoção das etapas do fluxo, _especialmente etapas de espera_ de campanhas inteligentes ativas, pode ter resultados inesperados. **Leia este artigo cuidadosamente.**

Primeiro vamos fazer o básico. Veja como remover uma etapa de fluxo indesejado de uma campanha inteligente. 1. No Fluxo da campanha inteligente, clique no ícone X para excluir qualquer etapa do fluxo.

![](assets/image2014-9-22-13-3a52-3a20.png)

1. Clique em **Excluir**.

   ![](assets/image2014-9-22-13-3a55-3a25.png)

   Simples e fácil, certo? Bem, na maioria das vezes...

   >[!CAUTION]
   >
   >Como excluir, adicionar e mover etapas dentro de um **ative** campanha pode definitivamente ter resultados inesperados. Considere a criação de uma nova campanha, o teste e a troca.

   As alterações podem ser feitas em uma campanha ativa, mas podem ter consequências imprevistas. Veja os detalhes:

   **Campanhas inteligentes em lote**

   Se sua campanha:

   1. **Nunca fugiu.** Faça todas as alterações desejadas. Não afetará ninguém até que você execute essa campanha.
   1. **É uma campanha inteligente recorrente.** As alterações afetarão as pessoas nas execuções futuras, e não nas execuções anteriores.
   1. **Já executou SEM etapas de espera.** Nenhuma pessoa será afetada porque a campanha está inativa após a execução.
   1. **Está funcionando agora.** As alterações podem causar comportamento inesperado, dependendo do tempo e dos detalhes da exclusão. É altamente recomendável NÃO editar uma campanha em lote que esteja sendo executada ativamente. Para casos de emergência, saiba como [suspender uma campanha inteligente em execução](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md).

   1. **Já executou COM etapas de espera.** Vários detalhes sobre este.\
      Quando uma pessoa insere uma etapa de espera, a pessoa se une à duração e a qual ETAPA NÚMERO retornar. Consulte o exemplo abaixo.

   **Acionar campanhas inteligentes**

   1. **Sem etapas de espera.** Se você excluir uma etapa normal, somente as pessoas que executarem a campanha no futuro serão afetadas.
   1. **Com etapas de espera.** Consulte o exemplo abaixo para campanhas em lote. Aplica-se a mesma lógica.

   >[!NOTE]
   >
   >**Exemplo**
   >
   >1. Uma campanha inteligente tem 3 etapas.
      >    * ETAPA 1. Enviar Email nº 1
      >    * ETAPA 2. Aguardar 1 semana
      >    * ETAPA 3. Enviar Email nº 2
   >
   >1. Pessoas que acessaram **Etapa 2** esperará 1 semana antes de passar para o **Etapa 3**.
   >1. Você exclui **Etapa 2** durante a semana.
   >1. As pessoas continuarão esperando a 1 semana. (Elas não retornam automaticamente ao fluxo.)
   >1. Quando finalmente voltarem, tentarão ir para **Etapa 3**. Eles não vão encontrá-lo.
   >1. **IMPORTANTE:** Como agora há apenas 2 etapas, a variável *as pessoas não receberão o Email nº 2.*


Fazendo alterações em uma campanha ativa

Entenda este recurso e você principal campanhas inteligentes.
