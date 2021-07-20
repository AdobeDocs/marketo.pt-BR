---
unique-page-id: 11378814
description: Listas inteligentes de contas - Documentos do Marketo - Documentação do produto
title: Listas inteligentes de contas
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
source-git-commit: e4d581ab258a875747a6d5323764e8b4a3949cba
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 1%

---

# Listas inteligentes de contas {#account-smart-lists}

Veja como identificar de forma rápida e precisa suas contas de alto valor.

>[!NOTE]
>
>Este recurso só está disponível para aqueles com o complemento Target Account Management e um TAM licenciado emitido.

## Criar uma lista inteligente de contas {#create-an-account-smart-list}

1. No Marketo, vá para **Marketing Activities**.

   ![](assets/account-smart-lists-1.png)

1. Localize e selecione o programa desejado.

   ![](assets/account-smart-lists-2.png)

1. Clique no menu suspenso **New** e selecione **New Local Asset**.

   ![](assets/account-smart-lists-3.png)

1. Clique em **Lista inteligente de contas**.

   ![](assets/account-smart-lists-4.png)

1. Insira um nome e clique em **Create** (Descrição e rótulos são opcionais).

   ![](assets/account-smart-lists-5.png)

Sua lista inteligente de contas foi criada! Consulte abaixo as etapas sobre como definir suas regras.

## Regras da lista inteligente de contas {#account-smart-list-rules}

As Smart Lists de conta funcionam de forma semelhante às Smart Lists padrão, com uma exceção notável: contêineres.

1. Para definir sua Lista inteligente de contas, clique na guia **Regras da lista inteligente de contas**.

   ![](assets/account-smart-lists-6.png)

1. Escolha os Filtros de conta desejados. Neste exemplo, estamos escolhendo _Industry is Healthcare_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

1. Escolha os Filtros de Pessoa Correspondidos. Neste exemplo, estamos escolhendo _State is California_.

   ![](assets/account-smart-lists-9.png)

**Etapa** opcional: Aqui é onde os contêineres entram. Se você escolher um Filtro de Pessoa Correspondente adicional, poderá soltá-lo abaixo do primeiro, ou _em_, criando um contêiner. Neste exemplo, estamos criando um container adicionando _Cargo Título é CFO_.

![](assets/account-smart-lists-10.png)

Veja como será o contêiner.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>A criação de um contêiner de filtros cria uma regra &quot;e&quot;, o que significa que ela só retornará todos os resultados combinados. Neste exemplo, conta com um setor de saúde, juntamente com a localização em California _e_ com alguém listado como CFO. Se você não quiser utilizar contêineres, basta soltar o filtro abaixo/acima do existente.

E é isso! Consulte a seção abaixo para ver como você pode utilizar sua Lista inteligente de contas.

>[!TIP]
>
>Assim como nas Smart Lists padrão, você pode usar a lógica avançada para refinar seus resultados. Você precisa de pelo menos três filtros para fazer isso, e nas Listas inteligentes de contas, um contêiner (independentemente de quantos filtros ele contém) é igual a um filtro.

## Ações de listas inteligentes de contas {#account-smart-list-actions}

Na guia Visão geral da Lista inteligente de contas, você observará algumas opções de ação.

**Exportar**: Isso exporta os resultados de sua Smart List de conta como um CSV.

**Clonar**: Faz uma cópia da sua Lista inteligente de contas.

**Enviar para a rede** de anúncios: Envia a lista para o LinkedIn como um novo público-alvo correspondente.

Também é possível fazer referência à Smart List da conta em uma Campanha/Lista inteligente padrão usando o filtro _People Member of Account Smart List_.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>Os resultados do Membro de Pessoas da Lista Inteligente de Contas mostrarão todas as pessoas na(s) conta(s) identificada(s), não apenas as pessoas encontradas por meio de filtros de Pessoa Correspondente na lista inteligente de contas.

>[!NOTE]
>
>**Definição**
>
>**Membro de Pessoas da Lista** Inteligente de Contas: Nesse caso, a palavra &quot;membro&quot; refere-se à própria conta, de modo que &quot;membro do povo&quot; significa o povo real (registros Marketo) nessas contas.
