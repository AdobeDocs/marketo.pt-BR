---
description: Descrição aqui.
title: Gerenciamento de Lista de Separação
hide: true
hidefromtoc: true
feature: Field Management
exl-id: 2b75edbb-0ce3-495b-a245-dac2db9c0126
source-git-commit: 3e1f9cb0a896dc9468d778e5ff2c5ffab3e6d80e
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Gerenciamento de Lista de Separação {#picklist-management}

O gerenciamento de lista de opções permite definir um conjunto fixo de valores para um campo para simplificar o gerenciamento de dados e fluxo de trabalho no Marketo Engage. Somente campos não textuais não mapeados para um campo CRM com uma lista de opções definida podem ser gerenciados no Marketo. Se um campo for mapeado para um campo CRM que tenha uma lista de opções definida, os valores desse campo deverão ser definidos no CRM.

Você pode ver o status de uma lista de opções na página Gerenciamento de campos. Um campo pode ter um dos seguintes status de lista de opções:

* **Gerenciado**: um usuário definiu o conjunto de valores que podem ser sugeridos automaticamente para este campo. Somente os valores definidos no gerenciamento de campo são sugeridos automaticamente. Se uma lista de opções gerenciada for excluída, o status da lista de opções será revertido para o valor inicial do campo, Não gerenciado ou Pré-implantado.

* **Não gerenciado**: os valores possíveis para este campo não foram definidos. Os valores são sugeridos automaticamente com base nos que existem nesses campos no banco de dados.

* **Pré-implantado**: o campo tem uma lista definida pelo sistema de valores sugeridos para o usuário.

* **CRM**: o campo tem um valor definido pelo sistema CRM, Salesforce.com ou Microsoft Dynamics, que está sincronizado com a instância.

  ![](assets/picklist-management-1.png)

## Gerenciar lista de opções {#manage-picklist}

Para modificar os valores de um campo, vá para **Admin** > **Gerenciamento de campos** e selecione o campo desejado.

Clique no menu suspenso _Ações do Campo_ e selecione **Gerenciar Lista de Opções**.

![](assets/picklist-management-2.png)

Na caixa de diálogo _Gerenciar Lista de Opções_, você pode adicionar, editar ou excluir valores. Você também pode excluir a lista de opções gerenciada para reverter o campo ao seu status original, _Não gerenciado_ ou _Pré-implantado_.

![](assets/picklist-management-3.png)

Cada entrada da lista de opções tem um Valor de Exibição e um Valor Enviado. O Valor de exibição é o que é sugerido ao usuário ao criar Smart Lists, Campanhas inteligentes ou formulários, enquanto o valor enviado é o que está armazenado. Por exemplo, seu caso de uso Código do território pode sugerir o nome completo de um território (por exemplo, Alberta), enquanto armazena o código de duas letras (AB).

## Sugestão automática {#autosuggest}

Quando a configuração _Lista de opções gerenciada_ estiver habilitada, as etapas Filtros, Opções de Etapa de Fluxo e Alterar Valor dos Dados sugerirão automaticamente valores da lista de opções gerenciada. Quando esta configuração está desabilitada, somente valores não gerenciados são sugeridos.

![](assets/picklist-management-4.png)

![](assets/picklist-management-5.png)

![](assets/picklist-management-6.png)

### Alternância entre listas de seleção gerenciadas e não gerenciadas {#switching}

A maioria das assinaturas do Marketo Engage contém dados de antes da introdução do Managed Picklists. Para usar valores em smart lists ou etapas de fluxo dessa lista de opções de versão não gerenciada (por exemplo, do conjunto completo de valores que existem em registros em seu banco de dados), alterne a configuração Lista de opções gerenciada na visualização da Lista inteligente ou do Campaign. Quando ativados, somente os valores da lista de opções gerenciada são exibidos. Quando desativado, a lista de opções não gerenciada é usada e os valores são sugeridos automaticamente com base nos valores existentes no banco de dados.

## Listas de opções de formulário (Selecionar campos de tipo) {#form-picklists}

Assim como as listas de opções pré-implantadas e gerenciadas pelo CRM, os valores das Listas de opções gerenciadas propagam-se para o Forms ao usar o tipo de campo Selecionar. Para um campo com uma lista de opções gerenciada, selecione esse campo e defina o Tipo de Campo como _Selecionar_.

![](assets/picklist-management-7.png)

Mostra o conjunto de valores da lista de seleção gerenciada definido para esse campo.

![](assets/picklist-management-8.png)
