---
description: Etapa 4 de 4 - Conectar a solução da Marketo com a conexão de controle de senha de proprietário de recurso - Documentação da Marketo - Documentação do produto
title: Etapa 4 de 4 - Conectar a solução da Marketo com a conexão de controle de senha de proprietário de recurso
exl-id: 71a52a3e-f31e-45ee-8196-d536528e42ca
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 4%

---

# Etapa 4 de 4: Conectar a solução Marketo com a conexão de controle de senha de proprietário de recurso {#step-4-of-4-connect-the-marketo-solution-ropc}

Esta é a última etapa da sincronização. Você está quase lá!

>[!PREREQUISITES]
>
>* [Etapa 1 de 4: Instalar a Solução da Marketo com a Conexão de Controle de Senha do Proprietário do Recurso](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}
>* [Etapa 2 de 4: Configurar a Solução da Marketo com a Conexão de Controle de Senha do Proprietário do Recurso](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}
>* [Etapa 3 de 4: Configurar o Aplicativo Cliente no MS Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md){target="_blank"}

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>Se estiver atualizando da Autenticação Básica para o OAuth, você poderá usar [este artigo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"} para reconfigurar sua autenticação.

## Inserir informações do Usuário da Sincronização Dinâmica {#enter-dynamics-sync-user-information}

1. Faça logon no Marketo e clique em **Admin**.

   ![](assets/login-admin.png)

1. Clique em **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Selecione **[!UICONTROL Microsoft]**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Clique em **[!UICONTROL Editar]** em **[!UICONTROL Inserir credenciais]**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Verifique se o URL da organização está correto, pois não é possível reverter as alterações subsequentes no esquema após o envio. Se um URL de organização incorreto for usado, será necessário obter uma nova assinatura do Marketo. Se você não souber a URL, [saiba como encontrá-la aqui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

   >[!NOTE]
   >
   >Antes de inserir novas credenciais, você pode [validá-las aqui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}.

1. Insira o **[!UICONTROL Nome de usuário]**, **[!UICONTROL Senha]**, **URL** do Microsoft Dynamics, **[!UICONTROL ID do Cliente]** e **[!UICONTROL Segredo do Cliente]**. Clique em **[!UICONTROL Salvar]** quando terminar.

   ![](assets/step-4-of-4-connect-ropc-5.png)

   >[!NOTE]
   >
   >O Nome de Usuário no Marketo deve corresponder ao Nome de Usuário para o usuário de sincronização no CRM. O formato pode ser `user@domain.com` ou DOMÍNIO\usuário.

## Selecionar campos para a sincronização {#select-fields-to-sync}

1. Clique em **[!UICONTROL Editar]** em **[!UICONTROL Selecionar campos para sincronização]**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Selecione os campos que deseja sincronizar com o Marketo para que sejam pré-selecionados. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

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

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Ativar sincronização {#enable-sync}

1. Clique em **[!UICONTROL Editar]** em **[!UICONTROL Habilitar sincronização]**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >A Marketo não eliminará automaticamente a duplicação em relação a uma sincronização do Microsoft Dynamics ou quando você inserir pessoas ou leads manualmente.

1. Leia tudo na janela pop-up, digite seu endereço de email e clique em **[!UICONTROL Iniciar sincronização]**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. A primeira sincronização pode levar algumas horas. Depois de concluído, você receberá uma notificação por email.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Excelente trabalho!

>[!MORELIKETHIS]
>
>[Reconfigurar o Método de Autenticação do Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"}
