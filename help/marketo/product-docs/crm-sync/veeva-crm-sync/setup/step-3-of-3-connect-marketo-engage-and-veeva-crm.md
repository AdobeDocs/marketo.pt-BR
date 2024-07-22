---
description: Etapa 3 de 3 - Conectar o Marketo Engage e o Veeva CRM - Documentação do Marketo - Documentação do produto
title: Etapa 3 de 3 - Conectar Marketo Engage e Veeva CRM
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
feature: Veeva CRM
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Etapa 3 de 3: Conectar Marketo Engage e Veeva CRM {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

Neste artigo, você configurará o Marketo Engage para sincronizar com a instância configurada do Veeva CRM. **Você verá o Salesforce em alguns dos pop-ups**, pois o Veeva CRM é criado na plataforma Salesforce.

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: Adicionar campos do Marketo ao Veeva](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}
>* [Etapa 2 de 3: Criar um Usuário Veeva para Marketo](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target="_blank"}

>[!IMPORTANT]
>
>Somente uma instância do Marketo pode ser conectada a uma instância do Veeva CRM de cada vez.

## Conectar-se ao Veeva CRM usando OAuth {#connect-to-veeva-crm-using-oauth}

1. No Marketo, Clique Em **[!UICONTROL Admin]**. Selecione **[!UICONTROL CRM]** e clique em **[!UICONTROL Sincronizar com Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >Certifique-se de [ocultar todos os campos desnecessários](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} no Marketo do usuário de sincronização antes de clicar em Sincronizar campos. Depois de clicar em Sincronizar campos, todos os campos que o usuário puder ver serão criados no Marketo permanentemente e não poderão ser excluídos.

1. Clique em **[!UICONTROL Fazer logon com Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Marque Sandbox se estiver sincronizando uma sandbox da Marketo com uma sandbox do Veeva CRM.

1. Clique em **[!UICONTROL Confirmar Credenciais]**.

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. Um pop-up com a página de logon do Salesforce será exibido. Insira suas credenciais de &quot;Usuário do Marketo Sync&quot; e clique em **[!UICONTROL Fazer logon]**.

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. Insira o código de verificação recebido por email (enviado pelo Salesforce) e clique em **[!UICONTROL Verificar]**.

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. Após a verificação bem-sucedida, a página de acesso será exibida solicitando acesso. Clique em **[!UICONTROL Permitir]**.

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. Em alguns minutos, uma janela pop-up será exibida no Marketo Engage. Clique em **[!UICONTROL Confirmar Credenciais]**.

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## Iniciar sincronização com o Veeva {#start-veeva-sync}

1. Clique em **[!UICONTROL Iniciar Sincronização Veeva]** para iniciar a sincronização persistente Marketo-Veeva CRM.

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >A Marketo não eliminará automaticamente a duplicação em relação a uma sincronização do Veeva CRM ou quando você inserir leads manualmente.

1. Clique em **[!UICONTROL Iniciar sincronização]**.

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>O tempo para concluir a sincronização inicial varia dependendo do tamanho e da complexidade do banco de dados.

## Verificar sincronização {#verify-sync}

O Marketo fornece mensagens de status para a sincronização do Veeva CRM na área de Administração. Você pode verificar se a sincronização está funcionando corretamente seguindo estas etapas.

1. No Marketo, clique em **[!UICONTROL Admin]** e depois em **[!UICONTROL Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. O status da sincronização está visível no canto superior direito. Ele mostrará uma das três mensagens: Última sincronização, Sincronização em andamento ou Falha.

>[!MORELIKETHIS]
>
>[Configurar Objetos Personalizados](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}
