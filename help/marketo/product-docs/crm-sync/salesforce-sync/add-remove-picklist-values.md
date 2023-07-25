---
unique-page-id: 4719312
description: Adicionar/Remover Valores Da Lista De Opções - Documentação Do Marketo - Documentação Do Produto
title: Adicionar/Remover Valores da Lista de Seleção
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Adicionar/Remover Valores da Lista de Seleção {#add-remove-picklist-values}

Estas são algumas informações que você deve saber sobre como adicionar e remover valores da lista de opções no Salesforce.

## Adição De Valores De Lista De Opções {#adding-picklist-values}

1. Se um valor adicional for adicionado no Salesforce a um tipo de campo de lista de opções, você receberá uma [notificação](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md) identificando quais formulários serão afetados.

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. Vá para o editor de formulários e [adicione o valor adicional](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md) à lista de sugestões.

## Remover Valores da Lista de Seleção {#remove-picklist-values}

Quando um valor de lista de opções é removido de um campo no Salesforce, você terá que remover manualmente esse valor de todos os formulários que hospedam esse campo.

>[!NOTE]
>
>Se um campo de cliente potencial e um campo de contato no Salesforce tiverem valores diferentes, os valores em comum estarão disponíveis para uso no Marketo.

Se um campo de cliente potencial e um campo de contato no Salesforce tiverem valores diferentes:

1. Adicionar um valor adicional no SFDC a uma lista de opções receberá uma notificação.
1. A notificação informará onde ele é usado. Agora você pode adicionar esse novo valor como uma opção no formulário, se desejar.

Se uma lista de opções de um cliente potencial do SFDC tiver valores diferentes de uma lista de opções de um contato do SFDC, os valores comuns serão usados como opções de valor padrão no formulário.

Se você remover um valor de uma lista de opções, terá que removê-lo manualmente como uma opção de seus formulários.
