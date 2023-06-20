---
unique-page-id: 11378814
description: Listas inteligentes de conta - Documentação do Marketo - Documentação do produto
title: Listas inteligentes de conta
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
source-git-commit: 4d88547ecdc25a2a1e0de49fab1493bbefd6800b
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Listas inteligentes de conta {#account-smart-lists}

Veja como identificar com rapidez e precisão suas contas de alto valor.

>[!NOTE]
>
>Esse recurso só está disponível para aqueles com o complemento Gerenciamento de conta do Target e um TAM licenciado e emitido.

## Criar uma lista inteligente de contas {#create-an-account-smart-list}

1. No Marketo, acesse **Atividades de marketing**.

   ![](assets/account-smart-lists-1.png)

1. Localize e selecione o programa desejado.

   ![](assets/account-smart-lists-2.png)

1. Clique em **Novo** e selecione **Novo ativo local**.

   ![](assets/account-smart-lists-3.png)

1. Clique em **Lista inteligente de contas**.

   ![](assets/account-smart-lists-4.png)

1. Insira um nome e clique em **Criar** (Descrição e rótulos são opcionais).

   ![](assets/account-smart-lists-5.png)

Sua lista inteligente de contas foi criada. Consulte as etapas abaixo para definir suas regras.

## Regras da lista inteligente de contas {#account-smart-list-rules}

As Smart Lists da conta funcionam de forma semelhante às Smart Lists padrão, com uma exceção notável: contêineres.

1. Para definir sua lista inteligente de contas, clique no link **Regras de lista inteligente de contas** guia.

   ![](assets/account-smart-lists-6.png)

1. Escolha o(s) filtro(s) de conta desejado(s). Neste exemplo, estamos escolhendo _O setor é da área de saúde_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

   >[!NOTE]
   >
   >Dados do indicador ICP que foram usados em seu [Classificação e ajuste da criação de perfil da conta](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md) serão exibidos como Atributos de conta personalizados para uso na Smart List da conta. Estes dados de atributos personalizados se baseiam em quando o Modelo de perfil de conta foi criado/atualizado.

1. Escolha o(s) Filtro(s) de pessoa correspondente(s). Neste exemplo, estamos escolhendo _Estado é Califórnia_.

   ![](assets/account-smart-lists-9.png)

**ETAPA OPCIONAL**: É aqui que os contêineres entram. Se você escolher um Filtro de pessoa correspondente adicional, poderá soltá-lo abaixo do primeiro, ou _in_ criar um contêiner. Neste exemplo, estamos criando um container adicionando _O cargo é CFO_.

![](assets/account-smart-lists-10.png)

Aqui está como o contêiner ficará.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>Criar um contêiner de filtros cria uma regra &quot;and&quot;, o que significa que retornará apenas todos os resultados combinados. Neste exemplo, as contas com um setor de assistência médica, juntamente com a localização na Califórnia _e_ com alguém listado como CFO. Se você não quiser utilizar contêineres, basta soltar o filtro abaixo/acima do filtro existente.

E é isso! Confira a seção abaixo para ver como você pode aproveitar sua lista inteligente de contas.

>[!TIP]
>
>Assim como com as Smart Lists padrão, você pode usar a lógica avançada para refinar ainda mais seus resultados. São necessários pelo menos três filtros para fazer isso e, nas Smart Lists de conta, um contêiner (independentemente de quantos filtros ele contém) equivale a um filtro.

## Ações de listas inteligentes de contas {#account-smart-list-actions}

Na guia Visão geral da Smart List da conta, você notará algumas opções de ação.

**Exportar**: exporta os resultados da sua lista inteligente de contas como um CSV.

**Clonar**: faz uma cópia da lista inteligente da sua conta.

**Enviar para a rede de publicidade**: envia a lista para a LinkedIn como um novo Público-alvo correspondido.

Você também pode fazer referência à sua lista inteligente de conta em uma campanha/lista inteligente padrão usando o _Membro de Pessoas da Smart List da Conta_ filtro.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>Os resultados do Membro de pessoas da lista inteligente de contas mostrarão cada pessoa na(s) conta(s) identificada(s), não apenas as pessoas que são encontradas por meio dos filtros Pessoa correspondente na lista inteligente de contas.

>[!NOTE]
>
>**Definição**
>
>**Membro de Pessoas da Smart List da Conta**: nesse caso, a palavra &quot;membro&quot; refere-se à própria conta, portanto, &quot;membro de pessoas&quot; significa as pessoas reais (registros do Marketo) nessas contas.
