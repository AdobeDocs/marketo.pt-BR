---
unique-page-id: 14352508
description: Criar campos dinâmicos personalizados - Documentação do Marketo - Documentação do produto
title: Criar campos dinâmicos personalizados
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Criar campos dinâmicos personalizados {#create-custom-dynamic-fields}

Há duas maneiras de criar campos dinâmicos personalizados.

## Salvando Campos Personalizados para Um ou Alguns Contatos {#saving-custom-fields-for-one-or-a-few-contacts}

1. Clique no nome de um contato na página Pessoas.

1. Escolha o menu suspenso ao lado de Cancelar inscrição e selecione **Editar**.

1. Role para baixo até a parte inferior da página de edição. Em seguida, você pode criar um nome e valor para o campo.

1. Clique em **Salvar**.

## Salvando campos personalizados para muitos contatos {#saving-custom-fields-for-many-contacts}

1. Crie uma planilha CSV com seus campos personalizados em sua própria coluna.

1. Siga o [processo normal de carregamento de CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md), parando na tela de mapeamento de campos.

1. Em vez de um dos campos predefinidos, escolha **Adicionar um novo Campo Personalizado** no menu suspenso.

1. Digite o nome de campo desejado e clique em **OK**.

1. Conclua o upload do CSV. Seus contatos aparecerão com o campo personalizado adicionado.

>[!NOTE]
>
>Após criar o campo personalizado, pode levar cerca de 30 minutos para que ele apareça no menu suspenso de campos dinâmicos no editor de modelo.

## Como usar seus campos personalizados em um modelo {#how-to-use-your-custom-fields-in-a-template}

Depois que os campos personalizados forem armazenados usando os métodos acima, você poderá referenciá-los em seus modelos.

1. [Crie um modelo](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md) e clique no botão **Campos Dinâmicos**, como você faria normalmente.

1. Selecione **Campos Personalizados** no menu suspenso exibido.

1. Você verá seus campos personalizados pré-armazenados e poderá selecionar um para preencher seu modelo.
