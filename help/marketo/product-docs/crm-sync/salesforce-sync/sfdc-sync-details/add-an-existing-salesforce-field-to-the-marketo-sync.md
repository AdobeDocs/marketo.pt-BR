---
unique-page-id: 4719308
description: Saiba como adicionar um campo existente do Salesforce à sincronização do Marketo. Torne o campo visível para o usuário de sincronização no Salesforce para que seja sincronizado no próximo ciclo.
title: Adicionar um campo existente do Salesforce à sincronização do Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/Vb-1DhNwUPQSPYuCkVzzSDDqWd4tvO-XoPhXn58hj6E'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 8%
---
# Adicionar um campo [!DNL Salesforce] existente à sincronização do Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Permissões de administrador são necessárias**

Normalmente, os novos campos personalizados no Salesforce são sincronizados com o Marketo Engage automaticamente. Caso contrário, os campos podem não estar visíveis para o usuário do Marketo Sync. Veja como você pode corrigir isso.

1. Clique no seu nome e selecione **[!UICONTROL Instalação]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Insira &quot;perfil&quot; na barra de pesquisa à esquerda e clique em **[!UICONTROL Perfis]** em **[!UICONTROL Gerenciar usuários]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Clique em sincronizar perfil do usuário.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Na seção **[!UICONTROL Segurança em Nível de Campo]**, clique em **[!UICONTROL Exibir]** ao lado do objeto que contém o campo.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Clique em **[!UICONTROL Editar]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Marque a caixa de seleção **[!UICONTROL Visível]** para o campo que você deseja adicionar à sincronização e clique em **[!UICONTROL Salvar]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   No próximo ciclo de sincronização, o Marketo verá o campo e iniciará a mágica.

   >[!NOTE]
   >
   > Se o campo já tiver valores em [!DNL Salesforce], esses valores não serão sincronizados com o Marketo até a próxima atualização de registro.
