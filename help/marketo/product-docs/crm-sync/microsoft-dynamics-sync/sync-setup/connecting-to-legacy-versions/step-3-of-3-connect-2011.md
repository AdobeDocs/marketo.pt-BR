---
unique-page-id: 3571809
description: Etapa 3 de 3 -Conectar o Microsoft Dynamics com o Marketo (2011 no local) - Documentação do Marketo - Documentação do produto
title: Etapa 3 de 3 - Conectar o Microsoft Dynamics com o Marketo (2011 no local)
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
feature: Microsoft Dynamics
source-git-commit: 2d3264ab75d2327f9226373aad383e7a51508589
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 2%

---

# Etapa 3 de 3: Conectar o Microsoft Dynamics com o Marketo (2011 no local) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

Tudo bem! Instalamos a solução e configuramos o usuário de sincronização. Em seguida, precisamos conectar o Marketo e o Dynamics.

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: instalar a solução da Marketo (2011 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}
>* [Etapa 2 de 3: Configurar o Usuário de Sincronização do Marketo no Dynamics (2011 no Local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md){target="_blank"}

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Inserir Informações de Usuário da Sincronização Dinâmica {#enter-dynamics-sync-user-information}

1. Faça logon no Marketo e clique em **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Clique em **[!UICONTROL CRM]**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Clique em **[!DNL Microsoft]**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Clique em **[!UICONTROL Editar]** em **[!UICONTROL Inserir credenciais]**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Verifique se suas credenciais estão corretas, pois não é possível reverter as alterações subsequentes no esquema após o envio. Se credenciais incorretas forem salvas, será necessário obter uma nova assinatura do Marketo.

1. Insira o **[!UICONTROL Nome de Usuário]**, **[!UICONTROL Senha]** e a **[!UICONTROL URL]** do CRM e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* O Nome de Usuário no Marketo deve corresponder ao Nome de Usuário para o usuário de sincronização no CRM. O formato pode ser `user@domain.com` ou DOMÍNIO\usuário.
   >* Se você não souber a URL, [saiba como encontrá-la aqui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

## Selecionar campos para a sincronização {#select-fields-to-sync}

Agora precisamos selecionar os campos que queremos sincronizar.

1. Clique em **[!UICONTROL Editar]** em **[!UICONTROL Selecionar campos para sincronização]**.

   ![](assets/image2015-3-16-9-51-28a.png)

1. Há campos pré-selecionados que serão sincronizados. Adicione mais se desejar e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

   >[!NOTE]
   >
   >O Marketo armazena uma referência aos campos a serem sincronizados. Se você excluir um campo no Dynamics, recomendamos fazê-lo com a [sincronização desabilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}. Em seguida, atualize o esquema no Marketo editando e salvando os [Selecionar campos para sincronização](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}.

## Sincronizar campos para um filtro personalizado {#sync-fields-for-a-custom-filter}

Se você criou um filtro personalizado, selecione os novos campos que serão sincronizados com o Marketo.

1. Vá para Admin e selecione **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **[!UICONTROL Editar]** em Detalhes da Sincronização de Campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Role para baixo até o campo e marque-o. O nome real deve ser new_synctomkto, mas o Nome de exibição pode ser qualquer item. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Ativar sincronização {#enable-sync}

1. Clique em **[!UICONTROL Editar]** em **[!UICONTROL Habilitar sincronização]**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >A Marketo não eliminará automaticamente a duplicação em relação a uma sincronização do Microsoft Dynamics, ou quando você inserir pessoas ou leads manualmente.

1. Leia tudo na janela pop-up, insira seu email e clique em **[!UICONTROL Iniciar sincronização]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Dependendo do número de registros, a sincronização inicial pode levar de algumas horas a alguns dias. Você receberá uma notificação por e-mail após a conclusão.

   ![](assets/image2014-12-11-11-3a55-3a15.png)
