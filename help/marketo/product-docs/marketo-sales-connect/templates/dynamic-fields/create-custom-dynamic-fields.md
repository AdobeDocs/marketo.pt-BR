---
unique-page-id: 14352508
description: Criar campos dinâmicos personalizados - Documentos do Marketo - Documentação do produto
title: Criar campos dinâmicos personalizados
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Criar campos dinâmicos personalizados {#create-custom-dynamic-fields}

Há duas maneiras de criar campos dinâmicos personalizados.

## Salvar campos personalizados para um ou alguns contatos {#saving-custom-fields-for-one-or-a-few-contacts}

1. Clique no nome de um contato na página Pessoas.

1. Escolha a lista suspensa ao lado de Cancelar inscrição e selecione **Editar**.

1. Role para baixo até a parte inferior da página de edição. Em seguida, é possível criar um nome e um valor para o campo.

1. Clique em **Salvar**.

## Salvar campos personalizados para muitos contatos {#saving-custom-fields-for-many-contacts}

1. Crie uma planilha CSV com os campos personalizados em sua própria coluna.

1. Siga as [processo normal de upload de CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md), parando na tela de mapeamento de campo.

1. Em vez de um dos campos predefinidos, escolha **Adicionar um novo campo personalizado** no menu suspenso .

1. Insira o nome do campo desejado e clique em **OK**.

1. Conclua o upload do CSV. Seus contatos aparecerão com o campo personalizado adicionado.

>[!NOTE]
>
>Após a criação do campo personalizado, pode levar cerca de 30 minutos para que o campo apareça no menu suspenso Campo dinâmico no editor de modelos.

## Como usar os campos personalizados em um modelo {#how-to-use-your-custom-fields-in-a-template}

Depois que os campos personalizados forem armazenados usando os métodos acima, você poderá referenciá-los em seus modelos.

1. [Criar um modelo](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md) e clique no botão **Campos dinâmicos** como você normalmente faria.

1. Selecionar **Campos personalizados** no menu suspenso exibido.

1. Você verá seus campos personalizados pré-armazenados e poderá selecionar um para preencher o modelo.
