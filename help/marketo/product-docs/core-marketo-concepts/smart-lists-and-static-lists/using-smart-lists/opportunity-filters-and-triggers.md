---
unique-page-id: 8159286
description: Filtros e acionadores de oportunidade - Documentos do Marketing - Documentação do produto
title: Filtros de oportunidade e acionadores
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# Filtros de oportunidade e acionadores {#opportunity-filters-and-triggers}

Filtros e acionadores de oportunidade permitem rastrear eventos de oportunidade do Salesforce. Eles são um pouco diferentes comparados a outros filtros e acionadores.

## Filtros de oportunidade {#opportunity-filters}

Os filtros de oportunidade permitem que você detalhe seus clientes potenciais do Salesforce que têm oportunidades. Você pode encontrá-los na pasta Oportunidades da Paleta ao editar uma lista inteligente. Eles vêm com alguns sabores.

* Número de Ópticos
* Valor Total da Opção
* Receita Esperada da Opção Total
* Tem oportunidade
* A oportunidade foi adicionada
* Oportunidade removida
* A oportunidade foi atualizada

Se você estiver procurando seus campos de Oportunidade (personalizado ou padrão), use o filtro **Tem oportunidade** ou **A oportunidade foi`[Added/Removed/Updated]`** filtros ou acionadores.

**Número de Opções, Quantia Total de Opções, Receita Total Esperada de Opções**

Com esses filtros, você pode encontrar clientes potenciais com base no número total, na quantia ou na receita esperada de todas as suas oportunidades.

![](assets/image2015-6-11-12-3a29-3a34.png)

**Tem oportunidade, foi adicionada à oportunidade, foi removida da oportunidade**

Se você estiver procurando clientes potenciais que tenham oportunidades com base em uma combinação de critérios, use o filtro **Tem oportunidade**, **Foi adicionado à oportunidade** ou **Foi removido do filtro Oportunidade**. Eles lhe dizem:

* **Tem Oportunidade**: Se este cliente potencial tiver uma oportunidade correspondente
* **Foi adicionado à Oportunidade**: Se esse cliente potencial tiver sido adicionado a uma oportunidade correspondente
* **Foi removido da Oportunidade**: Se este cliente potencial tiver sido removido de uma oportunidade correspondente

Adicione os critérios de pesquisa como **Restrições** no filtro. As restrições incluem seus campos padrão e personalizados de oportunidade:

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

Por exemplo, digamos que queiram encontrar clientes potenciais que tenham oportunidades abertas de pelo menos 5.000 dólares. Arraste no filtro **Tem oportunidade** e use as restrições **Está fechado** e **Valor**:

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>Ao usar vários filtros de Oportunidade, você pode obter respostas incorretas. Se você construísse o exemplo acima com dois filtros da Oportunidade, você obteria uma lista de clientes potenciais que têm qualquer oportunidade que seja de pelo menos US$ 5.000 e qualquer oportunidade que seja fechada, mesmo que essas sejam oportunidades separadas.

**A oportunidade foi atualizada**

O filtro **Oportunidade Atualizada** procura qualquer oportunidade quando um campo de oportunidade específico é atualizado. Escolha o campo para verificar com o menu suspenso Atributo do acionador e use as restrições para restringir o conjunto de alterações.

Por exemplo, este filtro mostrará todos os clientes potenciais que tiveram sua data de fechamento alterada nos últimos 30 dias:

![](assets/image2015-6-11-12-3a33-3a7.png)

## Acionadores de oportunidade {#opportunity-triggers}

Os seguintes acionadores de oportunidade estão disponíveis. Eles funcionam exatamente como seus filtros correspondentes (descritos anteriormente), exceto que podem disparar campanhas quando o evento acontece:

* A oportunidade é atualizada
* Adicionado à Oportunidade
* Removido da Oportunidade

Por exemplo, você pode usar essa Lista inteligente para disparar quando qualquer cliente potencial for adicionado a qualquer oportunidade. No fluxo, você pode adicioná-los à lista suspensa de marketing ou enviar a eles um email direcionado.

![](assets/image2015-6-11-12-3a33-3a48.png)

Para acionar seus campos personalizados de oportunidade, use o acionador **Oportunidade é Atualizada** e selecione o campo no menu suspenso:

![](assets/image2015-6-11-12-3a33-3a34.png)
