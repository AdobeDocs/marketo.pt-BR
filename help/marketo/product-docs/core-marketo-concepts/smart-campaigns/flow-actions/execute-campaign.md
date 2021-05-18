---
description: Execute Campaign - Marketo Docs - Documentação do produto
title: Executar campanha
source-git-commit: b491f476c4facc6343559a0acf5d5527e9afc618
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 1%

---

# Executar campanha {#execute-campaign}

Uma Campanha Executável, como outras campanhas, contém uma Lista Inteligente, Fluxo e Programação. Ao contrário de outras campanhas, você não a agenda ou ativa. Ele só pode ser chamado por outra campanha através da etapa Executar fluxo da campanha . As etapas de fluxo na Campanha executável são executadas em série com a campanha pai (diferente da Campanha de solicitação, que é executada simultaneamente em uma Campanha de acionador separada).

>[!NOTE]
>
>Campanhas executáveis são sempre filhos da campanha (pai) que as chama.

## Quando usar Executar Campanha {#when-to-use-execute-campaign}

Há muitas coisas que você pode fazer com uma Campanha Executável. Eles foram projetados para facilitar tarefas operacionais comuns, como roteamento de clientes potenciais, gerenciamento de ciclo de vida e pontuação (entre outros), e podem ser usados para executar o mesmo fluxo de trabalho a partir de campanhas em lote ou acionadas.

Você também pode usá-los quando precisar executar um fluxo separado, mas precisar depender dos resultados desse fluxo nas opções de etapas de fluxo subsequentes (ou seja, se isso for necessário).

Executar Campanha é uma melhoria em [Solicitar Campanha](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/request-campaign.md), pois pode ser executada em série ou em paralelo, enquanto a última só é executada em paralelo.

>[!NOTE]
>
>Etapas de espera e Webhooks nunca serão compatíveis com Campanhas executáveis. Para isso, você precisará usar a Campanha de solicitação .

## Como criar uma campanha executável {#how-to-create-an-executable-campaign}

1. Clique com o botão direito do mouse no programa desejado e selecione **New Smart Campaign**.

   ![](assets/execute-campaign-1.png)

1. Dê um nome a ele, marque a caixa de seleção **Executable** e clique em **Create**.

   ![](assets/execute-campaign-2.png)

1. Defina a Lista inteligente e o Fluxo, como qualquer outra Campanha inteligente.

Você também pode clonar uma Campanha inteligente existente. Se clonar uma Campanha Executável existente, ainda será necessário marcar a caixa de seleção **Executable** após nomeá-la.

>[!NOTE]
>
>Não é possível clonar uma campanha que contenha acionadores.

## Usar contexto de token de campanha pai {#use-parent-campaign-token-context}

Quando definido como true, os seguintes contextos de token serão enviados para a campanha filho (aquele que está sendo executado):

* Meus tokens
* Tokens da campanha
* Tokens de programa
* Tokens de Membro
* [Tokens de acionador](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md)  (se forem chamados de uma campanha acionada)

**Interação da API**

Ao usar Schedule ou Request Campaign [na API](https://developers.marketo.com/rest-api/assets/smart-campaigns/#batch), ambos permitem transmitir valores para Meus tokens, que substitui os valores definidos para esses tokens na campanha que você está chamando. Se essa Campanha executar outra campanha e definir &quot;Usar contexto pai para verdadeiro&quot;, ela usará os valores passados pela API, em vez dos valores definidos no aplicativo.

## O que deve ser observado {#things-to-note}

* A Smart List filtrará qualquer pessoa que não se qualificar. Se uma pessoa se qualificar, o registro de atividade de Campanha executada resultante os listará como &quot;Qualificado: TRUE&quot; (e FALSE se não)
* As regras de qualificação de Programação de Campanha se aplicam (Configurações de Campanha Inteligente na guia Programação)
* Campanhas executáveis não podem ser chamadas em espaços de trabalho
* Se você usar a ação de fluxo [Remover do Fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) direcionada a uma Campanha Executável, ela direcionará o filho e o pai
* Aproveitando a herança de token - por exemplo, se você tiver um único fluxo de pontuação comum acionado por vários ativos diferentes, poderá definir uma pontuação de Meu token padrão na campanha filho e na campanha pai, de modo que possa substituir o valor da campanha de pontuação filho para suas campanhas pai (consulte abaixo para obter um exemplo visual)
* O aninhamento de campanhas executáveis não está disponível no momento, mas estará em uma versão futura

>[!CAUTION]
>
>Nunca deixe suas listas inteligentes para campanhas executáveis inválidas, caso contrário, **ninguém** se qualificará para elas. A prática recomendada é criar ativos de lista inteligente separados, defini-los completamente e garantir que sejam válidos. Em seguida, use o filtro &quot;Membro da Smart List&quot; na Campanha Executável para trocar a definição da lista inteligente.

## Exemplo de herança de token {#token-inheritance-example}

Abaixo está um exemplo visual de Herança de tokens em uma Campanha Executável e duas campanhas pai: um com contexto de token definido como **True**, o outro como **False**.

Campanha filho com Pontuação de alteração tokens.

![](assets/execute-campaign-3.png)

A campanha infantil é &quot;Meus Tokens&quot;.

![](assets/execute-campaign-4.png)

**Exemplo um - Verdadeiro**

Na etapa Executar fluxo da campanha da primeira campanha pai, o &quot;Usar contexto de token de campanha pai&quot; é definido como **True**.

![](assets/execute-campaign-5.png)

Os Meus Tokens da campanha principal.

![](assets/execute-campaign-6.png)

Os resultados: pontuação alterada por +10.

![](assets/execute-campaign-7.png)

**Exemplo dois: Falso**

No filtro Executar campanha da segunda campanha pai, o &quot;Usar contexto de token de campanha pai&quot; é definido como **False**.

![](assets/execute-campaign-8.png)

Os Meus Tokens da campanha principal.

![](assets/execute-campaign-9.png)

Os resultados: pontuação inalterada, pois o valor de pontuação da campanha filho, +0, foi usado.

![](assets/execute-campaign-10.png)
