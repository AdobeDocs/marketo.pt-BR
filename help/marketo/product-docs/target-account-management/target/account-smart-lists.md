---
unique-page-id: 11378814
description: Listas inteligentes de conta - Documentação do Marketo - Documentação do produto
title: Listas inteligentes da conta
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
feature: Target Account Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 1%

---

# Listas inteligentes da conta {#account-smart-lists}

Veja como identificar com rapidez e precisão suas contas de alto valor.

>[!NOTE]
>
>Este recurso só está disponível para aqueles com o complemento [!UICONTROL Gerenciamento de Conta de Destino] e um TAM licenciado emitido.

## Criar uma [!UICONTROL Smart List da conta] {#create-an-account-smart-list}

1. No Marketo, vá para **[!UICONTROL Atividades de marketing]**.

   ![](assets/account-smart-lists-1.png)

1. Localize e selecione o programa desejado.

   ![](assets/account-smart-lists-2.png)

1. Clique no menu suspenso **[!UICONTROL Novo]** e selecione **[!UICONTROL Novo ativo local]**.

   ![](assets/account-smart-lists-3.png)

1. Clique em **[!UICONTROL Lista inteligente de contas]**.

   ![](assets/account-smart-lists-4.png)

1. Insira um nome e clique em **[!UICONTROL Criar]** (Descrição e Rótulos são opcionais).

   ![](assets/account-smart-lists-5.png)

Sua [!UICONTROL Lista Inteligente de Conta] foi criada! Consulte as etapas abaixo para definir suas regras.

## Regras da [!UICONTROL Smart List] da conta {#account-smart-list-rules}

[!UICONTROL Smart Lists de Conta] funcionam de forma semelhante às Smart Lists padrão, com uma exceção notável: contêineres.

1. Para definir sua [!UICONTROL Lista inteligente de contas], clique na guia **[!UICONTROL Regras da lista inteligente de contas]**.

   ![](assets/account-smart-lists-6.png)

1. Escolha o(s) filtro(s) de conta desejado(s). Neste exemplo, estamos escolhendo _[!UICONTROL O setor] é [!UICONTROL Saúde]_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

   >[!NOTE]
   >
   >Os dados do indicador ICP que foram usados em sua [Classificação e ajuste de criação de perfil da conta](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md) serão exibidos como Atributos de conta personalizados para uso em sua Smart List Conta. Estes dados de atributos personalizados se baseiam em quando o Modelo de perfil de conta foi criado/atualizado.

1. Escolha o(s) Filtro(s) de pessoa correspondente(s). Neste exemplo, estamos escolhendo _Estado é a Califórnia_.

   ![](assets/account-smart-lists-9.png)

**ETAPA OPCIONAL**: é aqui que entram os contêineres. Se você escolher um Filtro de pessoa correspondente adicional, poderá soltá-lo abaixo do primeiro, ou _in_, criando um contêiner. Neste exemplo, estamos criando um contêiner ao adicionar _O cargo é CFO_.

![](assets/account-smart-lists-10.png)

Aqui está como o contêiner ficará.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>Criar um contêiner de filtros cria uma regra &quot;and&quot;, o que significa que retornará apenas todos os resultados combinados. Neste exemplo, as contas com um setor de serviços de saúde, junto com uma localização na Califórnia _e_ com alguém listado como CFO. Se você não quiser utilizar contêineres, basta soltar o filtro abaixo/acima do filtro existente.

E é isso! Confira a seção abaixo para ver como você pode aproveitar sua [!UICONTROL Lista inteligente de contas].

>[!TIP]
>
>Assim como com as Smart Lists padrão, você pode usar a lógica avançada para refinar ainda mais seus resultados. Você precisa de pelo menos três filtros para fazer isso, e em [!UICONTROL Listas inteligentes de conta], um contêiner (independentemente de quantos filtros ele contém) equivale a um filtro.

## Ações da [!UICONTROL Smart List] da conta {#account-smart-list-actions}

Na guia Visão geral da sua [!UICONTROL Smart List da conta], você verá algumas opções de ação.

**[!UICONTROL Exportar]**: exporta os resultados da sua [!UICONTROL Smart List da conta] como CSV.

**[!UICONTROL Clonar]**: faz uma cópia da sua [!UICONTROL Lista Inteligente de Contas].

**[!UICONTROL Enviar para a Rede de Publicidade]**: Envia a lista para [!DNL LinkedIn] como um novo Público Correspondente.

Você também pode fazer referência à sua [!UICONTROL Lista Inteligente de Conta] em uma Campanha/Lista Inteligente padrão usando o filtro _[!UICONTROL Lista Inteligente de Membro de Conta]_.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>Os resultados da [!UICONTROL Lista Inteligente de Pessoas de Conta] mostrarão cada pessoa na(s) conta(s) identificada(s), não apenas as pessoas que são encontradas por meio dos filtros Pessoa Correspondentes na lista inteligente de contas.

>[!NOTE]
>
>**Definição**
>
>**[!UICONTROL Lista Inteligente de Membro de Conta de Pessoas]**: nesse caso, a palavra &quot;membro&quot; refere-se à própria conta; portanto, &quot;membro de pessoas&quot; significa as pessoas reais (registros Marketo) nessas contas.
