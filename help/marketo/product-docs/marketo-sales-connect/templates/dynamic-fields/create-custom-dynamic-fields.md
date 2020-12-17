---
unique-page-id: 14352508
description: Criar campos dinâmicos personalizados - Documentos de marketing - Documentação do produto
title: Criar campos dinâmicos personalizados
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---


# Criar campos dinâmicos personalizados {#create-custom-dynamic-fields}

Há duas maneiras de criar campos dinâmicos personalizados.

## Salvando campos personalizados para um ou alguns contatos {#saving-custom-fields-for-one-or-a-few-contacts}

1. Clique no nome de um contato na página Pessoas.
1. Escolha a lista suspensa ao lado de Cancelar inscrição e selecione **Editar**.
1. Role para baixo até a parte inferior da página de edição. Em seguida, é possível criar um nome e um valor para o seu campo.
1. Clique em **Salvar**.

## Salvando campos personalizados para muitos contatos {#saving-custom-fields-for-many-contacts}

1. Crie uma planilha CSV com seus campos personalizados em sua própria coluna.
1. Siga o [processo de carregamento CSV normal](http://docs.marketo.com/x/HIPS), parando na tela de mapeamento de campo.
1. Em vez de um dos campos predefinidos, escolha **Adicionar um novo campo personalizado** no menu suspenso.
1. Digite o nome do campo desejado e clique em **OK**.
1. Conclua o upload do CSV. Seus contatos aparecerão com o campo personalizado adicionado.

>[!NOTE]
>
>Depois de criar seu campo personalizado, pode levar cerca de 30 minutos para que o campo apareça no menu suspenso de campo dinâmico no editor de modelo.

## Como usar seus campos personalizados em um modelo {#how-to-use-your-custom-fields-in-a-template}

Depois que seus campos personalizados forem armazenados usando os métodos acima, você poderá referenciá-los em seus modelos.

1. [Crie um ](http://docs.marketo.com/x/OCDG) modelo e clique no botão Campos  **** dinâmicos, como você normalmente faria.
1. Selecione **Campos personalizados** no menu suspenso exibido.
1. Você verá seus campos personalizados pré-armazenados e poderá selecionar um para preencher em seu modelo.

