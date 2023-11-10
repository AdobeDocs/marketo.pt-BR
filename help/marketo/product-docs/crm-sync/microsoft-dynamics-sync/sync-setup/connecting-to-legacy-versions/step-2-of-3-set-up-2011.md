---
unique-page-id: 3571807
description: Etapa 2 de 3 - Configurar usuário do Marketo Sync no Dynamics (2011 no local) - Documentação do Marketo - Documentação do produto
title: Etapa 2 de 3 - Configurar o usuário do Marketo Sync no Dynamics (2011 no local)
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---

# Etapa 2 de 3: Configurar usuário do Marketo Sync no Dynamics (2011 no local) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Ótimo trabalho completando as etapas anteriores, vamos continuar percorrendo isso.

>[!PREREQUISITES]
>
>[Etapa 1 de 3: instalar a solução da Marketo (2011 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}

## Atribuir Função de Usuário de Sincronização {#assign-sync-user-role}

Atribua a função de Usuário de sincronização do Marketo somente ao usuário de sincronização do Marketo. Você não precisa atribuí-lo a nenhum outro usuário.

>[!NOTE]
>
>Isso se aplica ao plug-in do Marketo versão 4.0.0.14 e posterior. Para versões anteriores, todos os usuários devem ter a função de usuário sincronizar. Para atualizar o Marketo, consulte [Atualizar a solução Marketo para Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>A configuração de idioma do Usuário de sincronização [deve ser definido como inglês](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. No menu inferior esquerdo, selecione **[!UICONTROL Configurações]**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Na árvore, selecione **[!UICONTROL Administração]**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Selecionar **[!UICONTROL Usuários]**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Você verá uma lista de usuários aqui. Selecione o usuário de sincronização dedicado do Marketo ou entre em contato com [Serviços de Federação do Ative Diretory (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} administrador para criar um novo usuário dedicado ao Marketo. Clique em **[!UICONTROL Gerenciar Funções]**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Marcar **[!UICONTROL Usuário de sincronização do Marketo]** e clique em **[!UICONTROL OK]**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Se você não vir a função, volte para [etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"} e importe a solução.

   >[!NOTE]
   >
   >Quaisquer atualizações feitas em seu CRM pelo Usuário do Sync _não_ ser sincronizado com o Marketo.

## Configurar a solução da Marketo {#configure-marketo-solution}

Quase pronto! Temos apenas algumas últimas configurações antes de passar para o próximo artigo.

1. Selecionar **[!UICONTROL Configurações]**. Em seguida, selecione **[!UICONTROL Configuração do Marketo]** na árvore.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Se a Configuração do Marketo estiver ausente, tente atualizar a página. Se o problema persistir, [publicar a solução da Marketo novamente](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"} ou faça logout e login novamente.

1. Clique em **[!UICONTROL Padrão]**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Clique em ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. Na janela pop-up, selecione o usuário de sincronização. Clique em **[!UICONTROL OK]**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Clique em **[!UICONTROL Salvar]** para salvar as alterações.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Clique em **[!UICONTROL Publicar todas as personalizações]**.

   ![](assets/publish-all-customizations1.png)

## Antes de prosseguir para a Etapa 3 {#before-proceeding-to-step}

* Se quiser restringir o número de registros sincronizados, [configurar um filtro de sincronização personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} agora.
* Execute o [Validar a sincronização do Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} processo. Ele verifica se as configurações iniciais foram feitas corretamente.
* Faça logon no Usuário do Marketo Sync no Microsoft Dynamics CRM.

  Excelente trabalho!

>[!MORELIKETHIS]
>
>[Etapa 3 de 3: Conectar o Microsoft Dynamics com o Marketo (2011 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2011.md){target="_blank"}
