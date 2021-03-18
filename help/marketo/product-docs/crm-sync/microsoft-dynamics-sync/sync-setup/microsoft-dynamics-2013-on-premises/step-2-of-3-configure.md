---
unique-page-id: 3571816
description: Etapa 2 de 3 - Configurar usuário de sincronização para o Marketo (2013 no local) - Documentação do Marketo - Documentação do produto
title: Etapa 2 de 3 - Configurar usuário de sincronização para Marketo (On-Premise 2013)
translation-type: tm+mt
source-git-commit: 9d8a6d9880de5d2af211906c2410f2057c1f454d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Etapa 2 de 3: Configurar usuário de sincronização para o Marketo (2013 no local) {#step-of-configure-sync-user-for-marketo-on-premises}

Excelente trabalho ao concluir as etapas anteriores, vamos continuar avançando nisso.

>[!PREREQUISITES]
>
>[Etapa 1 de 3: Instalar a solução Marketo no Dynamics (2013 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)

## Atribuir Função de Usuário de Sincronização {#assign-sync-user-role}

Atribua a função Usuário de sincronização do Marketo somente ao usuário de sincronização do Marketo. Não é necessário atribuí-lo a nenhum outro usuário.

>[!NOTE]
>
>Isso se aplica ao plug-in do Marketo versão 4.0.0.14 e posterior. Para versões anteriores, todos os usuários devem ter a função de sincronização do usuário. Para atualizar o Marketo, consulte [Atualizar a solução Marketo para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

1. Em **Configurações**, clique em **Administração**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Selecione **Users**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. Você verá uma lista de usuários aqui. Selecione o usuário dedicado da Sincronização do Marketo ou entre em contato com o [Ative Diretory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [administrador para criar um novo usuário dedicado ao Marketo.](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Selecione o usuário de sincronização. Clique em ![](assets/image2015-3-26-11-3a16-3a22.png) e selecione **Gerenciar funções**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Marque **Marketo Sync User** e clique em **OK**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >Se você não vir a função, volte para [etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) e importe a solução.

   >[!NOTE]
   >
   >Qualquer atualização feita em seu CRM pelo Usuário de sincronização **not** será sincronizada novamente com o Marketo.

## Configurar a solução do Marketo {#configure-marketo-solution}

Quase pronto! Temos apenas algumas últimas partes da configuração antes de passar para o próximo artigo.

1. Em **Configurações**, clique em **Marketo Config**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >Se **Config do Marketo** estiver ausente, tente atualizar a página. Se o problema persistir, [publique a solução do Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) novamente ou tente sair e entrar novamente.

1. Clique em **Padrão**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Clique no campo **Marketo User** e selecione o usuário de sincronização.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Clique em ![](assets/image2015-3-13-15-3a10-3a11.png) no canto inferior direito para salvar as alterações.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Clique em **Publicar todas as personalizações**.

   ![](assets/publish-all-customizations1.png)

## Antes de prosseguir para a Etapa 3 {#before-proceeding-to-step}

* Se quiser restringir o número de registros sincronizados, [configure um filtro de sincronização personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) agora.
* Execute o processo [Validar o Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Ele verifica se as configurações iniciais foram feitas corretamente.
* Faça logon no usuário de sincronização do Marketo no Microsoft Dynamics CRM.

Excelente trabalho!

>[!MORELIKETHIS]
>
>[Etapa 3 de 3: Conectar o Marketo e o Dynamics (2013 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-3-of-3-connect.md)
