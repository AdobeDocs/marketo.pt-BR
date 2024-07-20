---
unique-page-id: 8159286
description: Filtros e acionadores da oportunidade - Documentação do Marketo - Documentação do produto
title: Filtros e acionadores da oportunidade
exl-id: 5b372c00-1553-4ac3-a495-53e208371d8d
feature: Smart Lists
source-git-commit: ac7d6b222ca561c88e0bf10aba7736c1b2eee3f7
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 5%

---

# Filtros e acionadores da oportunidade {#opportunity-filters-and-triggers}

Os filtros e acionadores de oportunidade permitem rastrear eventos de oportunidade do Salesforce. Eles são um pouco diferentes se comparados a outros filtros e acionadores.

## Filtros de oportunidade {#opportunity-filters}

Os filtros de oportunidade permitem que você se aprofunde em seus clientes potenciais do Salesforce que têm oportunidades. Você pode encontrá-las na pasta Oportunidades da Paleta ao editar uma Smart List. Eles vêm em alguns sabores.

* Número de oport
* Valor total da oport.
* Receita total esperada da oport.
* Possui oportunidade
* A oportunidade foi adicionada
* A oportunidade foi removida
* A oportunidade foi atualizada

Se estiver procurando seus campos de Oportunidade (personalizados ou padrão), use o filtro **Tem Oportunidade** ou **A oportunidade tinha`[Added/Removed/Updated]`** filtros ou acionadores.

**Número de Opções, Valor Total da Opção, Receita Total Esperada da Opção**

Com esses filtros, você pode encontrar leads com base no número total, na quantia ou na receita esperada de todas as suas oportunidades.

![](assets/opportunity-filters-and-triggers-1.png)

**Possui uma oportunidade, Foi adicionada à oportunidade, Foi removida da oportunidade**

Se você estiver procurando clientes potenciais que têm oportunidades com base em uma combinação de critérios, use o filtro **Tem Oportunidade**, **Foi Adicionada à Oportunidade** ou **Foi Removida da Oportunidade**. Eles lhe dizem:

* **Tem Oportunidade**: se este cliente em potencial tiver alguma oportunidade correspondente no momento
* **Foi Adicionado à Oportunidade**: se este cliente em potencial já foi adicionado a uma oportunidade correspondente
* **Foi Removido da Oportunidade**: se este cliente em potencial já foi removido de uma oportunidade correspondente

Adicione os critérios de pesquisa como **Restrições** no filtro. As restrições incluem os campos padrão de oportunidade e personalizados:

![](assets/opportunity-filters-and-triggers-2.png)

![](assets/opportunity-filters-and-triggers-3.png)

Por exemplo, digamos que você queira encontrar leads com oportunidades abertas de pelo menos US$ 5.000. Arraste no filtro **Tem Oportunidade** e use as restrições **Está Fechado** e **Valor**:

![](assets/opportunity-filters-and-triggers-4.png)

>[!NOTE]
>
>Ao usar vários filtros de Oportunidade, você pode obter respostas incorretas. Se você criou o exemplo acima com dois filtros Oportunidade, obterá uma lista de clientes potenciais que têm qualquer oportunidade de pelo menos US$ 5.000 e qualquer oportunidade que esteja fechada, mesmo que sejam oportunidades separadas.

**A oportunidade foi atualizada**

O filtro **Oportunidade Atualizada** procura qualquer oportunidade quando um campo de oportunidade específico é atualizado. Selecione o campo a ser verificado com o menu suspenso Acionador de atributo, em seguida, use as restrições para restringir o conjunto de alterações.

Por exemplo, este filtro mostrará todos os clientes em potencial que tiveram sua data de fechamento alterada nos últimos 30 dias:

![](assets/opportunity-filters-and-triggers-5.png)

## Acionadores da oportunidade {#opportunity-triggers}

Os acionadores de oportunidade a seguir estão disponíveis. Eles funcionam exatamente como os filtros correspondentes (descritos anteriormente), exceto que podem acionar campanhas logo quando o evento ocorre:

* A oportunidade é atualizada
* Adicionado à oportunidade
* Removido da oportunidade

Por exemplo, você pode usar essa lista inteligente para acionar quando qualquer cliente em potencial for adicionado a qualquer oportunidade. No fluxo, você pode adicioná-los à lista de Marketing suspenso ou enviar a eles um email direcionado.

![](assets/opportunity-filters-and-triggers-6.png)

Para acionar campos personalizados de oportunidade, use o acionador **Oportunidade atualizada** e escolha o campo na lista suspensa:

![](assets/opportunity-filters-and-triggers-7.png)
