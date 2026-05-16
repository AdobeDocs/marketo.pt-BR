---
unique-page-id: 3571819
description: Saiba como conectar o Marketo e o Dynamics 2013 no local na etapa final. Insira as informações do usuário de sincronização no Marketo Admin e habilite a sincronização.
title: Etapa 3 de 3 - Conectar o Marketo e o Dynamics (2013 no local)
exl-id: e28f1cc3-ee15-4981-a537-6c4a1682c4c1
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/pERYRYCLDigsARoh7aAWOTXRFmpIWKz8j-tgDb-ShTQ
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 401
ht-degree: 3%

---

# Etapa 3 de 3: Conectar o Marketo e [!DNL Dynamics] (2013 no Local) {#step-of-connect-marketo-and-dynamics-on-premises}

A solução está instalada e o usuário de sincronização está configurado. Em seguida, conecte o Marketo e o [!DNL Dynamics].

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: instalar a Solução da Marketo em [!DNL Dynamics] (2013 no Local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md)
>* [Etapa 2 de 3: Configurar Usuário de Sincronização para Marketo (2013 No Local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)

>[!NOTE]
>
>**Permissões de administrador são necessárias**

## Inserir Informações de Usuário de Sincronização [!DNL Dynamics] {#enter-dynamics-sync-user-information}

1. Faça logon no Marketo e clique em **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Clique em **[!UICONTROL CRM]**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Selecione **[!DNL Microsoft]**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Clique em **[!UICONTROL Editar]** em **[!UICONTROL Etapa 1: Inserir credenciais]**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Verifique se suas credenciais estão corretas. As alterações subsequentes no esquema não podem ser revertidas após o envio. Se credenciais incorretas forem salvas, uma nova assinatura do Marketo será necessária.

1. Insira o **[!UICONTROL Nome de Usuário]**, **[!UICONTROL Senha]** e [!DNL Microsoft Dynamics] **URL** e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >* O Nome de Usuário no Marketo deve corresponder ao Nome de Usuário para o usuário de sincronização no CRM. O formato pode ser `user@domain.com` ou DOMÍNIO\usuário.
   >* Se você não souber a URL, [saiba como encontrá-la aqui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

## Selecionar campos para a sincronização {#select-fields-to-sync}

Selecione os campos a serem sincronizados.

1. Clique em **[!UICONTROL Editar]** em **[!UICONTROL Etapa 2: Selecionar campos a serem sincronizados]**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Selecione os campos que deseja sincronizar com o Marketo para que sejam pré-selecionados. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2016-8-25-15-3a10-3a17.png)

   >[!NOTE]
   >
   >O Marketo armazena uma referência aos campos a serem sincronizados. Se você excluir um campo em [!DNL Dynamics], recomendamos fazê-lo com a [sincronização desabilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Em seguida, atualize o esquema no Marketo editando e salvando os [[!UICONTROL Selecionar campos para sincronização]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Sincronizar campos para um filtro personalizado {#sync-fields-for-a-custom-filter}

Se você criou um filtro personalizado, acesse e selecione os novos campos que serão sincronizados com o Marketo.

1. Vá para [!UICONTROL Admin] e selecione **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **[!UICONTROL Editar]** em [!UICONTROL Detalhes da sincronização de campo].

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Role para baixo até o campo e marque-o. O nome real deve ser new_synctomkto, mas o Nome de exibição pode ser qualquer item. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## Ativar sincronização {#enable-sync}

1. Clique em **[!UICONTROL Editar]** em **[!UICONTROL Etapa 3: Habilitar Sincronização]**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >A Marketo não desduplicará automaticamente em uma sincronização do [!DNL Microsoft Dynamics] ou quando você inserir pessoas ou clientes potenciais manualmente.

1. Leia tudo na janela pop-up, insira seu email e clique em **[!UICONTROL Iniciar sincronização]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Dependendo do número de registros, a sincronização inicial pode levar de algumas horas a alguns dias. Você receberá uma notificação por e-mail após a conclusão.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

A sincronização bidirecional entre o Marketo e [!DNL Microsoft Dynamics] está configurada. Se você adquiriu o [!DNL Marketo Sales Insight], consulte o seguinte:

>[!MORELIKETHIS]
>
>[Instalar e Configurar [!DNL Marketo Sales Insight] em [!DNL Microsoft Dynamics] 2013](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)
