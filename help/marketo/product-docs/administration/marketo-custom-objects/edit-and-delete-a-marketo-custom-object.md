---
unique-page-id: 10093690
description: Editar e excluir um objeto personalizado do Marketo - Documentos do Marketo - Documentação do produto
title: Editar e excluir um objeto personalizado do Marketo
exl-id: 97bae63e-f679-490b-bfa2-51d88355b29c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Editar e excluir um objeto personalizado do Marketo {#edit-and-delete-a-marketo-custom-object}

>[!NOTE]
>
>Não é possível criar, editar ou excluir um Link ou Campo de eliminação de duplicatas depois que o objeto personalizado é aprovado.

## Editar um objeto personalizado {#edit-a-custom-object}

Use o menu Ações personalizadas do objeto para editar ou excluir um objeto personalizado.

1. Clique em **Admin** e, em **Gerenciamento de Banco de Dados**, selecione **Marketo Custom Objects**.

   ![](assets/image2016-1-18-13-3a31-3a51.png)

1. Selecione o objeto personalizado que deseja editar à direita.

   ![](assets/image2016-1-18-13-3a33-3a11.png)

1. Clique na guia **Custom Object Actions** e clique em **Edit Object**.

   ![](assets/image2015-9-23-11-3a37-3a44.png)

   >[!NOTE]
   >
   >Editar objeto mostra os mesmos campos que Criar objeto, exceto pelo nome da API, que não pode ser editado.

1. Faça qualquer alteração. Arraste o controle deslizante se desejar mostrar o objeto na página Detalhes do lead . Clique em **Salvar**.

   ![](assets/image2015-9-15-16-3a48-3a39.png)

1. Certifique-se de aprovar [o objeto editado](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md).

## Excluir um objeto personalizado {#delete-a-custom-object}

É fácil excluir um objeto personalizado, mas você precisa ter cuidado. Objetos personalizados podem ser conectados a outros objetos ou a listas inteligentes. Portanto, o Marketo avisa antes de permitir que você clique em **Excluir**.

>[!CAUTION]
>
>Não é possível restaurar um objeto personalizado após excluí-lo.

1. Clique em **Admin** e, em **Gerenciamento de Banco de Dados**, selecione **Marketo Custom Objects**.

   ![](assets/image2016-1-18-13-3a36-3a0.png)

1. Selecione o objeto que deseja excluir.

   ![](assets/image2015-9-23-16-3a29-3a5.png)

1. Clique em **Ações do objeto personalizado** e selecione **Excluir objeto**.

   ![](assets/image2015-9-23-11-3a39-3a5.png)

   >[!TIP]
   >
   >Além disso, é possível clicar com o botão direito do mouse no objeto e selecionar **Delete Object**.

1. Se o objeto personalizado estiver em formato de rascunho, ainda não tiver sido aprovado, você receberá esse aviso. Se tiver certeza, clique em **Delete**.

   ![](assets/image2015-9-23-16-3a31-3a2.png)

1. Se o objeto personalizado já estiver aprovado, há maior risco se você excluí-lo. Então, você vai receber este aviso mais forte. Insira **Entendo**, marque a caixa de seleção **Não é possível desfazer** e clique em **Excluir**.

   ![](assets/image2016-1-15-9-3a49-3a38.png)

   >[!NOTE]
   >
   >Se o objeto personalizado estiver vinculado a um objeto intermediário, você deverá excluir o objeto intermediário primeiro.

>[!MORELIKETHIS]
>
>[Aprovar um objeto personalizado](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
