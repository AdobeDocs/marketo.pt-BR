---
description: Instalar o Marketo para Microsoft Dynamics 2016/Dynamics 365 no local Etapa 3 de 3 - Documentação do Marketo - Documentação do produto
title: Instalar o Marketo para Microsoft Dynamics 2016/Dynamics 365 no Local Etapa 3 de 3
exl-id: ae801a59-8e29-479c-84c5-a18c7511f21f
feature: Microsoft Dynamics
source-git-commit: 2d3264ab75d2327f9226373aad383e7a51508589
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 3%

---

# Etapa 3 de 3: Conectar o Marketo Dynamics (2016 No Local/Dynamics 365 No Local) {#step-of-connect-marketo-dynamics-on-premises-2016}

>[!PREREQUISITES]
>
>* [Instalar o Marketo para Microsoft Dynamics 2016/Dynamics 365 no Local Etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"}
>* [Instalar o Marketo para Microsoft Dynamics 2016/Dynamics 365 no Local Etapa 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md){target="_blank"}

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Inserir informações do Usuário da Sincronização Dinâmica {#enter-dynamics-sync-user-information}

1. Faça logon no Marketo e clique em **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Clique em **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Selecione **[!DNL Microsoft]**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Clique em **[!UICONTROL Editar]** em **[!UICONTROL Inserir credenciais]**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Verifique se suas credenciais estão corretas, pois não é possível reverter as alterações subsequentes no esquema após o envio. Se credenciais incorretas forem salvas, será necessário obter uma nova assinatura do Marketo.

1. Insira o **[!UICONTROL Nome de Usuário]**, **[!UICONTROL Senha]**, a **[!UICONTROL URL]** do Microsoft Dynamics e um **Segredo/ID do Cliente**. Clique em **[!UICONTROL Salvar]** quando terminar.

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* Se seu Marketo foi provisionado antes de outubro de 2020, ID do cliente e Segredo são campos opcionais. Caso contrário, elas são obrigatórias. A obtenção dessas informações dependerá da versão do MSD que você estiver usando.
   >* O Nome de Usuário no Marketo deve corresponder ao Nome de Usuário para o usuário de sincronização no CRM. O formato pode ser `user@domain.com` ou DOMÍNIO\usuário.
   >* Se você não souber a URL, [saiba como encontrá-la aqui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

   >[!TIP]
   >
   >Não sabe o URL? Mostraremos como encontrar sua [URL do Dynamics Organization Service](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) aqui.

## Selecionar campos para a sincronização {#select-fields-to-sync}

1. Clique em **[!UICONTROL Editar]** em **[!UICONTROL Selecionar campos para sincronização]**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Selecione os campos que deseja sincronizar com o Marketo para que sejam pré-selecionados. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>O Marketo armazena uma referência aos campos a serem sincronizados. Se você excluir um campo no Dynamics, recomendamos fazê-lo com a [sincronização desabilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}. Em seguida, atualize o esquema no Marketo editando e salvando os [Selecionar campos para sincronização](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}.

## Sincronizar campos para um filtro personalizado {#sync-fields-for-a-custom-filter}

Se você criou um filtro personalizado, selecione os novos campos que serão sincronizados com o Marketo.

1. Acesse Administrador e selecione **[!DNL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **[!UICONTROL Editar]** em Detalhes da Sincronização de Campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Role para baixo até o campo e marque-o. O nome real deve ser new_synctomkto, mas o Nome de exibição pode ser qualquer item. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Ativar sincronização {#enable-sync}

1. Clique em **[!UICONTROL Editar]** em **[!UICONTROL Habilitar sincronização]**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >O Marketo não eliminará automaticamente a duplicação em relação a uma sincronização do Microsoft Dynamics ou ao inserir pessoas manualmente.

1. Leia tudo na janela pop-up, insira seu email e clique em **[!UICONTROL Iniciar sincronização]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Dependendo do número de registros, a sincronização inicial pode levar de algumas horas a alguns dias. Você receberá uma notificação por e-mail após a conclusão.

   ![](assets/image2015-3-16-9-59-51.png)
