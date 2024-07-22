---
unique-page-id: 7504739
description: Instalar o Marketo para Microsoft Dynamics 2015 no local Etapa 2 de 3 - Documentação do Marketo - Documentação do produto
title: Instalar o Marketo para Microsoft Dynamics 2015 no Local Etapa 2 de 3
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# Etapa 2 de 3 Configurar o Marketo for Dynamics (2015 no local){#step-of-set-up-for-marketo-on-premises-2015}

Ótimo trabalho para concluir as etapas anteriores. Vamos continuar passando por isso.

>[!PREREQUISITES]
>
>[Instalar o Marketo para Microsoft Dynamics 2015 no Local Etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"}

## Atribuir Função de Usuário de Sincronização {#assign-sync-user-role}

Atribua a função de Usuário de sincronização do Marketo somente ao usuário de sincronização do Marketo. Você não precisa atribuí-lo a nenhum outro usuário.

>[!NOTE]
>
>Isso se aplica à versão 4.0.0.14 e posterior do Marketo. Para versões anteriores, todos os usuários devem ter a função de usuário sincronizar. Para atualizar sua Marketo, consulte [Atualizar a Solução da Marketo para o Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>A configuração de idioma do Usuário de Sincronização [ deve ser definida como Inglês](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. Em **[!UICONTROL Configurações]**, clique em **[!UICONTROL Segurança]**.

   ![](assets/assign1.png)

1. Clique em **[!UICONTROL Usuários]**.

   ![](assets/assign2.png)

1. Você verá uma lista de usuários aqui. Selecione o usuário dedicado do Marketo Sync ou contate o administrador do [Ative Diretory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} (ADFS) para criar um usuário dedicado para o Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Selecione o usuário de sincronização. Clique em **[!UICONTROL Gerenciar Funções]**.

   ![](assets/assign4.png)

1. Verifique o usuário de sincronização do Marketo e clique em **[!UICONTROL OK]**.

   ![](assets/assign5.png)

   >[!IMPORTANT]
   >
   >O usuário de sincronização deve ter permissão de leitura para a configuração do Marketo.

   >[!TIP]
   >
   >Se você não vir a função, volte para a [etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"} e importe a solução.

   >[!NOTE]
   >
   >Quaisquer atualizações feitas em seu CRM pelo Usuário da Sincronização _não_ serão sincronizadas com o Marketo novamente.

## Configurar a solução da Marketo {#configure-marketo-solution}

Quase pronto! Temos apenas algumas últimas configurações antes de passar para o próximo artigo.

1. Em **[!UICONTROL Configurações]**, clique em **[!UICONTROL Configuração do Marketo]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Se a Configuração do Marketo estiver ausente, tente atualizar a página. Se o problema persistir, [publique a Solução da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"} ou tente fazer logoff e logon novamente.

1. Clique em **[!UICONTROL Padrão]**.

   ![](assets/configure2.png)

1. Clique no campo **[!UICONTROL Usuário do Marketo]** e selecione o usuário de sincronização.

   ![](assets/configure3.png)

1. Clique no ícone de salvar no canto inferior direito.

   ![](assets/configure4.png)

1. Clique em **[!UICONTROL Todas as personalizações do Publish]**.

   ![](assets/publish-all-customizations1.png)

   >[!NOTE]
   >
   >O usuário de sincronização deve ter permissão de leitura para a configuração do Marketo.

## Antes de prosseguir para a Etapa 3 {#before-proceeding-to-step}

* Se quiser restringir o número de registros sincronizados, [configure um filtro de sincronização personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} agora.
* Execute o processo [Validar sincronização do Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}. Ele verifica se as configurações iniciais foram feitas corretamente.
* Faça logon no Usuário do Marketo Sync no Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Instalar o Marketo para Microsoft Dynamics 2015 no Local Etapa 3 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2015.md){target="_blank"}
