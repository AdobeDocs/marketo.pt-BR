---
unique-page-id: 3571807
description: Etapa 2 de 3 - Configurar usuário de sincronização de marketing no Dynamics (2011 no local) - Documentação do produto - Documentação do produto
title: Etapa 2 de 3 - Configurar usuário de sincronização de marketing no Dynamics (2011 no local)
translation-type: tm+mt
source-git-commit: 309f299275bfe75e8af0150be0a5ffdf28a54cf8
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---


# Etapa 2 de 3: Configurar usuário de sincronização de marketing no Dynamics (2011 no local) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Excelente trabalho ao completar os passos anteriores, vamos continuar a avançar nisto.

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: Instale a solução Marketo (2011 On-Premise)](step-1-of-3-install.md)

>



## Atribuir função de usuário de sincronização {#assign-sync-user-role}

Atribua a função Usuário de sincronização de marketing somente ao usuário de sincronização de marketing. Não é necessário atribuí-lo a nenhum outro usuário.

>[!NOTE]
>
>Isso se aplica ao plug-in Marketo versão 4.0.0.14 e posterior. Para versões anteriores, todos os usuários devem ter a função de usuário de sincronização. Para atualizar o Marketo, consulte [Atualizar a solução de marketing para Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. No menu inferior esquerdo, selecione **Settings**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Na árvore, selecione **Administração**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Selecione **Usuários**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Você verá uma lista de usuários aqui. Selecione seu usuário dedicado de sincronização de marketing ou entre em contato com seu administrador [Serviços de Federação do Ative Diretory (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) para criar um novo usuário dedicado ao Marketo. Clique em **Gerenciar funções**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Marque **Usuário de sincronização de marketing** e clique em **OK**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Se você não vir a função, volte para [etapa 1 de 3](step-1-of-3-install.md) e importe a solução.

   >[!NOTE]
   >
   >Todas as atualizações feitas em seu CRM pelo Usuário de sincronização serão **e não** sincronizadas de volta ao Marketo.

## Configurar a solução de marketing {#configure-marketo-solution}

Quase pronto! Temos apenas algumas últimas configurações antes de passar para o próximo artigo.

1. Selecione **Configurações**. Em seguida, selecione **Marketo Config **na árvore.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Se a configuração de Marketo estiver ausente, tente atualizar a página. Se o problema persistir, [publique a solução Marketo novamente](step-1-of-3-install.md) ou faça logout e volte a fazer logon.

1. Clique em **Padrão**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Clique em ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. No pop-up, selecione o usuário de sincronização. Em seguida, clique em **OK**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Clique em **Salvar** para salvar as alterações.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Clique em **Publicar todas as personalizações**.

   ![](assets/publish-all-customizations1.png)

## Antes de prosseguir para a Etapa 3 {#before-proceeding-to-step}

    * Se você quiser restringir o número de registros que sincronizar, [configure um filtro de sincronização personalizado](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) agora.
    * Execute o processo [Validar Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Ele verifica se as configurações iniciais foram feitas corretamente.
    * Faça logon no usuário de sincronização de marketing no Microsoft Dynamics CRM.

Ótimo trabalho!

>[!NOTE]
>
>**Artigos relacionados**
>
>[Etapa 3 de 3: Conecte o Microsoft Dynamics com o Marketing (On-Premise 2011)](step-3-of-3-connect.md)

