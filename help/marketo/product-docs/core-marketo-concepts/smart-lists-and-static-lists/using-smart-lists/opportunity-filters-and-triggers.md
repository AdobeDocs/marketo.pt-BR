---
unique-page-id: 8159286
description: Filtros e acionadores da oportunidade - Documentos do Marketo - Documentação do produto
title: Filtros e acionadores da oportunidade
exl-id: 5b372c00-1553-4ac3-a495-53e208371d8d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 5%

---

# Filtros e acionadores da oportunidade {#opportunity-filters-and-triggers}

Os filtros e acionadores de oportunidade permitem rastrear eventos de oportunidade do Salesforce. Elas são um pouco diferentes em comparação com outros filtros e acionadores.

## Filtros de Oportunidade {#opportunity-filters}

Os filtros de oportunidade permitem detalhar os leads do Salesforce que têm oportunidades. Você pode encontrá-las na pasta Oportunidades da Paleta ao editar uma lista inteligente. Eles vêm em alguns sabores.

* Número de oport
* Valor total da oport.
* Receita total esperada da oport.
* Possui oportunidade
* Oportunidade adicionada
* Oportunidade removida
* A oportunidade foi atualizada

Se estiver procurando seus campos de Oportunidade (personalizados ou padrão), use a variável **Tem oportunidade** filtrar ou **A oportunidade foi`[Added/Removed/Updated]`** filtros ou acionadores.

**Número de opções, Valor total da opção, Receita total esperada da opção**

Com esses filtros, você pode encontrar leads com base no número total, na quantidade ou na receita esperada de todas as suas oportunidades.

![](assets/image2015-6-11-12-3a29-3a34.png)

**Tem Oportunidade, Foi Adicionado à Oportunidade, Foi Removido da Oportunidade**

Se você estiver procurando leads que têm oportunidades baseadas em uma combinação de critérios, use a variável **Tem oportunidade**, **Foi adicionado à Oportunidade** ou **Foi removido da Oportunidade** filtro. Eles lhe dizem:

* **Tem oportunidade**: Se este cliente potencial tiver uma oportunidade correspondente
* **Foi adicionado à Oportunidade**: Se este cliente potencial tiver sido adicionado a uma oportunidade correspondente
* **Foi removido da Oportunidade**: Se este cliente potencial tiver sido removido de uma oportunidade correspondente

Adicionar os critérios de pesquisa como **Restrições** no filtro. As restrições incluem os campos padrão e personalizados da oportunidade:

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

Por exemplo, digamos que você queira encontrar leads que tenham oportunidades abertas de pelo menos US$ 5.000. Arraste no **Tem oportunidade** filtrar e usar o **Está Fechado** e **Valor** restrições:

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>Quando você usa vários filtros de Oportunidade, pode obter respostas incorretas. Se você criou o exemplo acima com dois filtros de Oportunidade, você obteria uma lista de leads que têm qualquer oportunidade que seja de pelo menos US$ 5.000 e qualquer oportunidade que seja fechada, mesmo que essas sejam oportunidades separadas.

**A oportunidade foi atualizada**

O **A oportunidade foi atualizada** o filtro procura qualquer oportunidade quando um campo de oportunidade específico foi atualizado. Escolha o campo para verificar com o menu suspenso Atributo do acionador e use as restrições para restringir o conjunto de alterações.

Por exemplo, esse filtro mostrará todos os leads que tiveram sua alteração de data de fechamento nos últimos 30 dias:

![](assets/image2015-6-11-12-3a33-3a7.png)

## Acionadores da oportunidade {#opportunity-triggers}

Os seguintes acionadores de oportunidade estão disponíveis. Eles funcionam exatamente como os filtros correspondentes (descritos anteriormente), exceto que podem acionar campanhas exatamente quando o evento ocorre:

* A oportunidade é atualizada
* Adicionado à oportunidade
* Removido da oportunidade

Por exemplo, você pode usar essa Smart List para acionar quando qualquer lead for adicionado a qualquer oportunidade. No fluxo, você pode adicioná-los à lista de Suspensões de marketing ou enviar a eles um email direcionado.

![](assets/image2015-6-11-12-3a33-3a48.png)

Para acionar os campos personalizados da oportunidade, use a variável **A oportunidade é atualizada** e escolha o campo na lista suspensa:

![](assets/image2015-6-11-12-3a33-3a34.png)
