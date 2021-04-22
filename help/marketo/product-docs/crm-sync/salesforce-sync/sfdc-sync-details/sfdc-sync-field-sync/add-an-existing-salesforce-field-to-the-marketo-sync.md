---
unique-page-id: 4719308
description: Adicionar um campo Salesforce existente ao Marketo Sync - Marketo Docs - Documentação do produto
title: Adicionar um campo Salesforce existente à sincronização do Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Adicionar um campo Salesforce existente ao Marketo Sync {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Permissões de administrador necessárias**

Normalmente, os novos campos personalizados no Salesforce são sincronizados automaticamente com o Marketo. Caso contrário, os campos podem não estar visíveis para o usuário do Marketo Sync. Veja como você pode consertar isso.

1. Clique no seu nome e selecione **Setup**.

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. Insira **profile** na barra de pesquisa esquerda e clique em **Profiles** em **Manage Users**.

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. Clique no perfil do usuário de sincronização.

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. Na seção **Field-Level Security**, clique em **View** ao lado do objeto que contém o campo.

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. Clique em **Editar**.

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. Marque a caixa de seleção **Visível** do campo que deseja adicionar à sincronização e clique em **Salvar**.

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   Doce! No próximo ciclo de sincronização, o Marketo verá o campo e iniciará a mágica.

   >[!NOTE]
   >
   > Se o campo já tiver valores no Salesforce, esses valores não serão sincronizados com o Marketo até que o próximo registro seja atualizado.
