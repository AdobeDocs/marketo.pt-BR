---
unique-page-id: 3571807
description: Etapa 2 de 3 - Configurar usuário de sincronização do Marketo no Dynamics (2011 no local) - Documentação do Marketo - Documentação do produto
title: Etapa 2 de 3 - Configurar usuário de sincronização do Marketo no Dynamics (2011 no local)
translation-type: tm+mt
source-git-commit: 9d8a6d9880de5d2af211906c2410f2057c1f454d
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---


# Etapa 2 de 3: Configurar o usuário de sincronização do Marketo no Dynamics (2011 no local) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Excelente trabalho ao concluir as etapas anteriores, vamos continuar avançando nisso.

>[!PREREQUISITES]
>
>[Etapa 1 de 3: Instalar a solução Marketo (2011 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)

## Atribuir Função de Usuário de Sincronização {#assign-sync-user-role}

Atribua a função Usuário de sincronização do Marketo somente ao usuário de sincronização do Marketo. Não é necessário atribuí-lo a nenhum outro usuário.

>[!NOTE]
>
>Isso se aplica ao plug-in do Marketo versão 4.0.0.14 e posterior. Para versões anteriores, todos os usuários devem ter a função de sincronização do usuário. Para atualizar o Marketo, consulte [Atualizar a solução Marketo para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

1. No menu inferior esquerdo, selecione **Settings**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Na árvore, selecione **Administration**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Selecione **Users**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Você verá uma lista de usuários aqui. Selecione seu usuário dedicado de sincronização do Marketo ou entre em contato com o administrador do [Ative Diretory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) para criar um novo usuário dedicado ao Marketo. Clique em **Gerenciar funções**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Marque **Marketo Sync User** e clique em **OK**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Se você não vir a função, volte para [etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) e importe a solução.

   >[!NOTE]
   >
   >Qualquer atualização feita em seu CRM pelo Usuário de sincronização **not** será sincronizada novamente com o Marketo.

## Configurar a solução do Marketo {#configure-marketo-solution}

Quase pronto! Temos apenas algumas últimas partes da configuração antes de passar para o próximo artigo.

1. Selecione **Settings**. Em seguida, selecione **Marketo Config** na árvore.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Se a configuração do Marketo estiver ausente, tente atualizar a página. Se o problema persistir, [publique a solução do Marketo novamente](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) ou faça logoff e volte a fazer logon.

1. Clique em **Padrão**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Clique em ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. Na janela pop-up , selecione o usuário de sincronização. Em seguida, clique em **OK**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Clique em **Save** para salvar as alterações.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Clique em **Publicar todas as personalizações**.

   ![](assets/publish-all-customizations1.png)

## Antes de prosseguir para a Etapa 3 {#before-proceeding-to-step}

    * Se quiser restringir o número de registros sincronizados, [configure um filtro de sincronização personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) agora.
    * Execute o processo [Validar o Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Ele verifica se as configurações iniciais foram feitas corretamente.
    * Efetue logon no usuário de sincronização do Marketo no Microsoft Dynamics CRM.

Excelente trabalho!

>[!MORELIKETHIS]
>
>[Etapa 3 de 3: Conectar o Microsoft Dynamics com o Marketo (2011 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-3-of-3-connect.md)
