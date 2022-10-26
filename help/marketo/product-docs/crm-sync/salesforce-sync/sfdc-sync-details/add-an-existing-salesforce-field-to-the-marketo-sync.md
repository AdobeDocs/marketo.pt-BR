---
unique-page-id: 4719308
description: Adicionar um campo Salesforce existente ao Marketo Sync - Marketo Docs - Documentação do produto
title: Adicionar um campo Salesforce existente à sincronização do Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
source-git-commit: 81bc90bcccc8073511c9f331471c0cda9f4147cb
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Adicionar um campo Salesforce existente à sincronização do Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Permissões de administrador necessárias**

Normalmente, os novos campos personalizados no Salesforce são sincronizados automaticamente com o Marketo. Caso contrário, os campos podem não estar visíveis para o usuário do Marketo Sync. Veja como você pode consertar isso.

1. Clique no seu nome e selecione **Configuração**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Enter **perfil** na barra de pesquisa esquerda e clique em **Perfis** under **Gerenciar usuários**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Clique no perfil do usuário de sincronização.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Em **Segurança no nível do campo** seção , clique em **Exibir** ao lado do objeto que contém o campo .

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Clique em **Editar**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Verifique a **Visível** caixa de seleção do campo que deseja adicionar à sincronização e clique em **Salvar**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   Doce! No próximo ciclo de sincronização, o Marketo verá o campo e iniciará a mágica.

   >[!NOTE]
   >
   > Se o campo já tiver valores no Salesforce, esses valores não serão sincronizados com o Marketo até que o próximo registro seja atualizado.
