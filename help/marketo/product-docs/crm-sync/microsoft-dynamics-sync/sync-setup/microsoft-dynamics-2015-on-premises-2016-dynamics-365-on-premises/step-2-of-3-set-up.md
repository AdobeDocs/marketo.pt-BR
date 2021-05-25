---
unique-page-id: 7504739
description: Instale o Marketo para Dynamics 2015 no local e 2016 365 no local etapa 2 de 3 - Documentação da Marketo - Documentação do produto
title: Instale o Marketo para Dynamics 2015 no local e 2016 365 no local Etapa 2 de 3
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
source-git-commit: 5473e1a78769ba23e9c3a5926407cf42ef9685a0
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Etapa 2 de 3 Configurar o Marketo para Dynamics (2015 no local e 2016 365 no local){#step-of-set-up-for-marketo-on-premises-and-365}

Excelente trabalho ao concluir as etapas anteriores. Vamos continuar a passar por isto.

>[!PREREQUISITES]
[Instale o Marketo para Dynamics 2015 no local e 2016 365 no local Etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)>
>

## Atribuir Função de Usuário de Sincronização {#assign-sync-user-role}

Atribua a função Usuário de sincronização do Marketo somente ao usuário de sincronização do Marketo. Não é necessário atribuí-lo a nenhum outro usuário.

>[!NOTE]
Isso se aplica ao Marketo versão 4.0.0.14 e posterior. Para versões anteriores, todos os usuários devem ter a função de sincronização do usuário. Para atualizar sua Marketo, consulte [Atualizar a Solução da Marketo para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
A configuração de idioma do Usuário de sincronização [deve ser definida como inglês](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. Em **Configurações**, clique em **Segurança**.

   ![](assets/assign1.png)

1. Clique em **Usuários**.

   ![](assets/assign2.png)

1. Você verá uma lista de usuários aqui. Selecione o usuário dedicado do Marketo Sync ou entre em contato com o administrador do [Ative Diretory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS) para criar um usuário dedicado ao Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Selecione o usuário de sincronização. Clique em **Gerenciar funções**.

   ![](assets/assign4.png)

   Marque Marketo Sync User (Usuário de sincronização do) e clique em OK.

   ![](assets/assign5.png)

   >[!TIP]
   Se você não vir a função, volte para [etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md) e importe a solução.

   >[!NOTE]
   Qualquer atualização feita em seu CRM pelo Usuário de sincronização **not** será sincronizada novamente com o Marketo.

## Configurar a solução Marketo {#configure-marketo-solution}

Quase pronto! Temos apenas algumas últimas partes da configuração antes de passar para o próximo artigo.

1. Em **Configurações**, clique em **Marketo Config**.

   ![](assets/configure1.png)

   >[!NOTE]
   Se a configuração do Marketo estiver ausente, tente atualizar a página. Se o problema persistir, [publique a Solução da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md) ou tente sair e entrar novamente.

1. Clique em **Padrão**.

   ![](assets/configure2.png)

1. Clique no campo **Usuário do Marketo** e selecione o usuário de sincronização.

   ![](assets/configure3.png)

1. Clique no ícone Save no canto inferior direito.

   ![](assets/configure4.png)

1. Clique em **Publicar todas as personalizações**.

   ![](assets/publish-all-customizations1.png)

## Antes de prosseguir para a Etapa 3 {#before-proceeding-to-step}

* Se quiser restringir o número de registros sincronizados, [configure um filtro de sincronização personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) agora.
* Execute o processo [Validar o Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Ele verifica se as configurações iniciais foram feitas corretamente.
* Faça logon no usuário do Marketo Sync no Microsoft Dynamics CRM.

>[!MORELIKETHIS]
[Instale o Marketo para Dynamics 2015 no local e 2016 365 no local Etapa 3 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
