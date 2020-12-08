---
unique-page-id: 4719308
description: Adicionar um campo do Salesforce existente à sincronização de marketing - documentos do marketing - documentação do produto
title: Adicionar um campo do Salesforce existente à sincronização de marketing
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Adicionar um campo do Salesforce existente à sincronização de marketing {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Permissões de administrador necessárias**

Normalmente, os novos campos personalizados no Salesforce são sincronizados automaticamente para o Marketing. Caso contrário, os campos podem não estar visíveis para o usuário de Sincronização de marketing. É assim que se pode consertar isto.

1. Clique no seu nome e selecione **Configuração**.

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. Digite o **perfil** na barra de pesquisa esquerda e clique em **Perfis** em **Gerenciar usuários**.

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. Clique no perfil do usuário de sincronização.

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. Na seção Segurança **no nível do** campo, clique em **Visualização** ao lado do objeto que contém o campo.

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. Clique em **Editar**.

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. Marque a caixa de seleção **Visível** do campo que deseja adicionar à sincronização e clique em **Salvar**.

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   Doce! No próximo ciclo de sincronização, Marketo verá o campo e start a magia.

   >[!NOTE]
   >
   > Se o campo já tiver valores no Salesforce, esses valores não serão sincronizados com o Marketo até a próxima atualização do registro.

