---
unique-page-id: 7504739
description: Instale o Marketo para o Dynamics 2015 On-Prem e 2016 365 On-Prem Step 2 de 3 - Marketing to Docs - Documentação do produto
title: Instale o Marketo para o Dynamics 2015 On-Prem e 2016 365 On-Prem Etapa 2 de 3
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---


# Etapa 2 de 3 Configurar o Marketing para Dinâmicas (2015 On-Prem e 2016 365 On-Prem){#step-of-set-up-for-marketo-on-premises-and-365}

Excelente trabalho ao concluir as etapas anteriores. Vamos continuar a mexer nisto.

>[!PREREQUISITES]
>
>[Instale o Marketo para o Dynamics 2015 On-Prem e 2016 365 On-Prem Etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## Atribuir função de usuário de sincronização {#assign-sync-user-role}

Atribua a função Usuário de sincronização de marketing somente ao usuário de sincronização de marketing. Não é necessário atribuí-lo a nenhum outro usuário.

>[!NOTE]
>
>Isso se aplica à versão 4.0.0.14 e posterior do Marketo. Para versões anteriores, todos os usuários devem ter a função de usuário de sincronização. Para atualizar seu Marketo, consulte [Atualizar a solução de marketing para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Em **Configurações**, clique em **Segurança**.

   ![](assets/assign1.png)

1. Clique em **Usuários**.

   ![](assets/assign2.png)

1. Você verá uma lista de usuários aqui. Selecione o usuário dedicado de Sincronização de Marketing ou entre em contato com o administrador do [Ative Diretory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS) para criar um usuário dedicado para o Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Selecione o usuário de sincronização. Clique em **Gerenciar funções**.

   ![](assets/assign4.png)

   Marque Marketo Sync User (Usuário de sincronização de marketing) e clique em OK.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Se você não vir a função, volte para [etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md) e importe a solução.

   >[!NOTE]
   >
   >Todas as atualizações feitas em seu CRM pelo Usuário de sincronização serão **e não** sincronizadas de volta ao Marketo.

## Configurar a solução de marketing {#configure-marketo-solution}

Quase pronto! Temos apenas algumas últimas configurações antes de passar para o próximo artigo.

1. Em **Configurações**, clique em **Configuração do Marketing**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Se a configuração de Marketo estiver ausente, tente atualizar a página. Se o problema persistir, [publique a solução Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md) ou tente fazer logoff e login novamente.

1. Clique em **Padrão**.

   ![](assets/configure2.png)

1. Clique no campo **Usuário do Marketing** e selecione o usuário de sincronização.

   ![](assets/configure3.png)

1. Clique no ícone salvar no canto inferior direito.

   ![](assets/configure4.png)

1. Clique em **Publicar todas as personalizações**.

   ![](assets/publish-all-customizations1.png)

## Antes de prosseguir para a Etapa 3 {#before-proceeding-to-step}

* Se você quiser restringir o número de registros sincronizados, [configure um filtro de sincronização personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) agora.
* Execute o processo [Validar Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Ele verifica se as configurações iniciais foram feitas corretamente.
* Faça logon no usuário de sincronização de marketing no Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Instale o Marketo para o Dynamics 2015 On-Prem e 2016 365 On-Prem Etapa 3 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
