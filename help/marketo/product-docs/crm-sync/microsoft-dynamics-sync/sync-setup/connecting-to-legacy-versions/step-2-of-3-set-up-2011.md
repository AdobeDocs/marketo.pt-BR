---
unique-page-id: 3571807
description: Etapa 2 de 3 - Configurar o usuário do Marketo Sync no Dynamics (2011 no local) - Documentos do Marketo - Documentação do produto
title: Etapa 2 de 3 - Configurar o usuário do Marketo Sync no Dynamics (2011 no local)
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
source-git-commit: 2568d3414c8aaec882b79442f6312bae3b9514ab
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Etapa 2 de 3: Configurar o usuário do Marketo Sync no Dynamics (2011 no local) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Excelente trabalho ao concluir as etapas anteriores, vamos continuar avançando nisso.

>[!PREREQUISITES]
>
>[Etapa 1 de 3: Instalar a solução Marketo (2011 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)

## Atribuir Função de Usuário de Sincronização {#assign-sync-user-role}

Atribua a função Usuário de sincronização do Marketo somente ao usuário de sincronização do Marketo. Não é necessário atribuí-lo a nenhum outro usuário.

>[!NOTE]
>
>This applies to Marketo plugin version 4.0.0.14 and later. Para versões anteriores, todos os usuários devem ter a função de sincronização do usuário. To upgrade Marketo, see [Upgrade the Marketo Solution for Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>The language setting of the Sync User [should be set to English](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. No menu inferior esquerdo, selecione **Configurações**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Na árvore, selecione **Administração**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Select **Users**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. You will see a list of users here. Select your dedicated Marketo sync user or contact your [Active Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) administrator to create a new user that&#39;s dedicated to Marketo. Clique em **Gerenciar funções**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Verificar **Usuário do Marketo Sync** e clique em **OK**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >If you don&#39;t see the role, go back to [step 1 of 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) and import the solution.

   >[!NOTE]
   >
   >Qualquer atualização feita em seu CRM pelo Usuário de sincronização **not** ser sincronizado de volta ao Marketo.

## Configurar a solução Marketo {#configure-marketo-solution}

Quase pronto! Temos apenas algumas últimas partes da configuração antes de passar para o próximo artigo.

1. Selecionar **Configurações**. Then select **Marketo Config** in the tree.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Se a configuração do Marketo estiver ausente, tente atualizar a página. Se o problema persistir, [publicar a solução Marketo novamente](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) ou faça logoff e volte.

1. Clique em **Padrão**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Click on ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. Na janela pop-up , selecione o usuário de sincronização. Then click **OK**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Clique em **Salvar** para salvar as alterações.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Click **Publish All Customizations**.

   ![](assets/publish-all-customizations1.png)

## Antes de prosseguir para a Etapa 3 {#before-proceeding-to-step}

    * Se quiser restringir o número de registros sincronizados, [configure um filtro de sincronização personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) agora.
    * Execute o processo [Validar o Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Ele verifica se as configurações iniciais foram feitas corretamente.
    * Efetue logon no usuário de sincronização do Marketo no Microsoft Dynamics CRM.

Muito bem!

>[!MORELIKETHIS]
>
>[Step 3 of 3: Connect Microsoft Dynamics with Marketo (2011 On-Premises)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-3-of-3-connect.md)
