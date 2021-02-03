---
unique-page-id: 4719312
description: Adicionar/remover valores da lista de opções - Documentos do marketing - Documentação do produto
title: Adicionar/remover valores da lista de opções
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# Adicionar/remover valores da lista de opções {#add-remove-picklist-values}

Estas são algumas informações sobre como adicionar e remover valores de lista de opções no Salesforce.

## Adicionando valores da lista de opções {#adding-picklist-values}

1. Se um valor adicional for adicionado no Salesforce a um tipo de campo de lista de opções, você receberá uma [notificação](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md) identificando quais formulários isso afetará.

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. Vá para o editor de formulários e [adicione o valor adicional](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md) à sua lista de sugestões.

## Remover Valores da Lista de Opções {#remove-picklist-values}

Quando um valor de lista de seleção é removido de um campo no Salesforce, é necessário remover manualmente esse valor de todos os formulários que hospedam esse campo.

>[!NOTE]
>
>Se um campo de cliente potencial e um campo de contato no Salesforce tiverem valores diferentes, os valores em comum estarão disponíveis para uso no Marketo.

Se um campo de cliente potencial e um campo de contato no Salesforce tiverem valores diferentes:

1. A adição de um valor adicional no SFDC a uma lista de opções receberá uma notificação.
1. A notificação informará onde é usada. Agora é possível adicionar esse novo valor como uma opção no formulário, se desejar.

Se uma lista de opções de um cliente potencial SFDC tiver valores diferentes de uma lista de opções para um contato SFDC, os valores comuns serão usados como opções de valor padrão no formulário.

Se você remover um valor de uma lista de opções, será necessário removê-lo manualmente como uma opção dos formulários.
