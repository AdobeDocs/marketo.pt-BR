---
unique-page-id: 3571819
description: Etapa 3 de 3 - Conectar o Marketo e o Dynamics (2013 no local) - Documentos do Marketo - Documentação do produto
title: Etapa 3 de 3 - Conectar o Marketo e o Dynamics (2013 no local)
exl-id: e28f1cc3-ee15-4981-a537-6c4a1682c4c1
source-git-commit: 2568d3414c8aaec882b79442f6312bae3b9514ab
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 1%

---

# Etapa 3 de 3: Conectar o Marketo e o Dynamics (2013 no local) {#step-of-connect-marketo-and-dynamics-on-premises}

Tudo bem! Instalamos a solução e configuramos o usuário de sincronização. Em seguida, precisamos conectar o Marketo e o Dynamics.

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: Instalar a solução Marketo no Dynamics (2013 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)
>* [Etapa 2 de 3: Configurar usuário de sincronização para Marketo (2013 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-2-of-3-configure.md)


>[!NOTE]
>
>**Permissões de administrador necessárias**

## Inserir Informações do Usuário do Dynamics Sync {#enter-dynamics-sync-user-information}

1. Faça logon no Marketo e clique em **Administrador**.

   ![](assets/login-admin.png)

1. Clique em **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Selecionar **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Clique em **Editar** em **Etapa 1: Inserir Credenciais**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Certifique-se de que suas credenciais estejam corretas, pois não podemos reverter as alterações subsequentes do schema após o envio. Se as credenciais incorretas forem salvas, você terá que obter uma nova assinatura do Marketo.

1. Insira o **Nome do usuário**, **Senha** e Microsoft Dynamics **URL** em seguida, clique em **Salvar**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >* O Nome de usuário no Marketo deve corresponder ao Nome de usuário para o usuário de sincronização no CRM. O formato pode ser user@domain.com ou DOMAIN\user.
   >* Se você não souber o URL, [saiba como encontrá-lo aqui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


## Selecionar campos para a sincronização {#select-fields-to-sync}

Agora, precisamos selecionar os campos que deseja sincronizar.

1. Clique em **Editar** em **Etapa 2: Selecionar Campos para Sincronizar**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Selecione os campos que deseja sincronizar com o Marketo para que sejam pré-selecionados. Clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a10-3a17.png)

   >[!NOTE]
   >
   >O Marketo armazena uma referência aos campos a serem sincronizados. Se você excluir um campo no Dynamics, recomendamos fazer isso com a variável [sincronização desativada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Em seguida, atualize o esquema no Marketo editando e salvando o [Selecionar Campos para Sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Sincronizar campos para um filtro personalizado {#sync-fields-for-a-custom-filter}

Se você criou um filtro personalizado, acesse e selecione os novos campos a serem sincronizados com o Marketo.

1. Acesse Admin e selecione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **Editar** em Detalhes de sincronização de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Role para baixo até o campo e verifique-o. O nome real deve ser new_synctomkto, mas o Nome de exibição pode ser qualquer coisa. Clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## Ativar sincronização {#enable-sync}

1. Clique em **Editar** em **Etapa 3: Ativar Sincronização**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >O Marketo não removerá automaticamente a duplicação em relação a uma sincronização do Microsoft Dynamics ou quando você inserir pessoas ou leads manualmente.

1. Leia tudo no pop-up, insira seu email e clique em **Iniciar Sincronização**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. A primeira sincronização pode levar algumas horas. Depois de terminar, você receberá uma notificação por email.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

Excelente trabalho! Você acabou de desencadear o poder da sincronização bidirecional entre o Marketo e o Microsoft Dynamics. Se você adquiriu o Marketo Sales Insight, é mais divertido ser realizado:

>[!MORELIKETHIS]
>
>[Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 2013](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)
