---
unique-page-id: 4719308
description: Adicionar um campo existente do Salesforce à sincronização do Marketo - Documentação do Marketo - Documentação do produto
title: Adicionar um campo existente do Salesforce à sincronização do Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Adicionar um campo existente do Salesforce à sincronização do Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Permissões de administrador necessárias**

Normalmente, novos campos personalizados no Salesforce são sincronizados com o Marketo Engage automaticamente. Caso contrário, os campos podem não estar visíveis para o usuário do Marketo Sync. Veja como você pode corrigir isso.

1. Clique no seu nome e selecione **[!UICONTROL Instalação]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Insira &quot;perfil&quot; na barra de pesquisa à esquerda e clique em **[!UICONTROL Perfis]** em **[!UICONTROL Gerenciar usuários]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Clique em sincronizar perfil do usuário.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Na seção **[!UICONTROL Segurança em Nível de Campo]**, clique em **[!UICONTROL Exibir]** ao lado do objeto que contém o campo.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Clique em **[!UICONTROL Editar]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Marque a caixa de seleção **[!UICONTROL Visível]** para o campo que você deseja adicionar à sincronização e clique em **[!UICONTROL Salvar]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   No próximo ciclo de sincronização, o Marketo verá o campo e iniciará a mágica.

   >[!NOTE]
   >
   > Se o campo já tiver valores no Salesforce, esses valores não serão sincronizados com o Marketo até a próxima atualização de registro.
