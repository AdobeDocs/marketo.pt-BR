---
unique-page-id: 3571816
description: Etapa 2 de 3 - Configurar usuário de sincronização para Marketo (2013 nas instalações) - Documentação do produto - Documentação do produto
title: Etapa 2 de 3 - Configurar usuário de sincronização para o Marketo (locais 2013)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# Etapa 2 de 3: Configurar o usuário de sincronização para o Marketing (2013 On-Premise) {#step-of-configure-sync-user-for-marketo-on-premises}

Excelente trabalho ao completar os passos anteriores, vamos continuar a avançar nisto.

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: Instalar a solução Marketo no Dynamics (2013 On-Premise)](step-1-of-3-install.md)


## Atribuir função de usuário de sincronização {#assign-sync-user-role}

Atribua a função Usuário de sincronização de marketing somente ao usuário de sincronização de marketing. Não é necessário atribuí-lo a nenhum outro usuário.

>[!NOTE]
>
>Isso se aplica ao plug-in Marketo versão 4.0.0.14 e posterior. Para versões anteriores, todos os usuários devem ter a função de usuário de sincronização. Para atualizar o Marketo, consulte [Atualizar a solução de marketing para Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Em **Configurações**, clique em **Administração**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Selecione **Usuários**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. Você verá uma lista de usuários aqui. Selecione seu usuário dedicado de Sincronização de Marketing ou entre em contato com seu [administrador do Ative Diretory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [para criar um novo usuário dedicado ao Marketo.](http://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Selecione o usuário de sincronização. Clique em ![](assets/image2015-3-26-11-3a16-3a22.png)e selecione **Gerenciar funções**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Marque **Usuário de sincronização de marketing** e clique em **OK**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >Se você não vir a função, volte para [etapa 1 de 3](step-1-of-3-install.md) e importe a solução.

   >[!NOTE]
   >
   >Todas as atualizações feitas em seu CRM pelo Usuário de sincronização serão **e não** sincronizadas de volta ao Marketo.

## Configurar a solução de marketing {#configure-marketo-solution}

Quase pronto! Temos apenas algumas últimas configurações antes de passar para o próximo artigo.

1. Em **Configurações**, clique em **Configuração do Marketing**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >Se **Configuração do Marketing** estiver ausente, tente atualizar a página. Se o problema persistir, [publique a solução Marketo](https://docs.marketo.com/pages/viewpage.action?pageId=3571813#Step1of3:InstalltheMarketoSolutioninDynamics(2013On-Premises)-PublishAllCustomizations) novamente ou tente fazer logoff e login novamente.

1. Clique em **Padrão**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Clique no campo **Usuário do Marketing** e selecione o usuário de sincronização.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Clique em ![](assets/image2015-3-13-15-3a10-3a11.png) no canto inferior direito para salvar as alterações.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Clique em **Publicar todas as personalizações**.

   ![](assets/publish-all-customizations1.png)

## Antes de prosseguir para a Etapa 3 {#before-proceeding-to-step}

* Se você quiser restringir o número de registros sincronizados, [configure um filtro de sincronização personalizado](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) agora.
* Execute o processo [Validar Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Ele verifica se as configurações iniciais foram feitas corretamente.
* Faça logon no usuário de sincronização de marketing no Microsoft Dynamics CRM.

Ótimo trabalho!

>[!NOTE]
>
>**Artigos relacionados**
>
>* [Etapa 3 de 3: Connect Marketing e Dynamics (2013 no local)](step-3-of-3-connect.md)

