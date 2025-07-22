---
description: Etapa 3 de 3 - Conectar o Marketo Engage e [!DNL Veeva] CRM - Documentação do Marketo - Documentação do produto
title: Etapa 3 de 3 - Conectar o Marketo Engage e [!DNL Veeva] CRM
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Etapa 3 de 3: Conectar o Marketo Engage e o [!DNL Veeva] CRM {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

Neste artigo, você configurará o Marketo Engage para sincronizar com sua instância do CRM [!DNL Veeva] configurada. **Você verá [!DNL Salesforce] em algumas janelas pop-up**, pois o CRM do [!DNL Veeva] foi criado na plataforma [!DNL Salesforce].

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: Adicionar Campos do Marketo a [!DNL Veeva]](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}
>* [Etapa 2 de 3: Criar um [!DNL Veeva] Usuário para Marketo](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target="_blank"}

>[!IMPORTANT]
>
>Somente uma Instância do Marketo pode ser conectada a uma instância do CRM [!DNL Veeva] de cada vez.

## Conectar-se ao CRM [!DNL Veeva] usando OAuth {#connect-to-veeva-crm-using-oauth}

1. No Marketo, Clique Em **[!UICONTROL Admin]**. Selecione **[!UICONTROL CRM]** e clique em **[!UICONTROL Sincronizar com Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >Certifique-se de [ocultar todos os campos desnecessários](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} no Marketo do usuário de sincronização antes de clicar em Sincronizar campos. Depois de clicar em Sincronizar campos, todos os campos que o usuário puder ver serão criados no Marketo permanentemente e não poderão ser excluídos.

1. Clique em **[!UICONTROL Fazer logon com Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Marque [!UICONTROL Sandbox] se estiver sincronizando uma Sandbox da Marketo com uma Sandbox do CRM [!DNL Veeva].

1. Clique em **[!UICONTROL Confirmar Credenciais]**.

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. Um pop-up com a página de logon [!DNL Salesforce] será exibido. Insira suas credenciais de &quot;Usuário do Marketo Sync&quot; e clique em **[!UICONTROL Fazer logon]**.

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. Insira o código de verificação recebido por email (enviado por [!DNL Salesforce]) e clique em **[!UICONTROL Verificar]**.

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. Após a verificação bem-sucedida, a página de acesso será exibida solicitando acesso. Clique em **[!UICONTROL Permitir]**.

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. Em alguns minutos, uma janela pop-up será exibida no Marketo Engage. Clique em **[!UICONTROL Confirmar Credenciais]**.

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## Iniciar Sincronização de [!DNL Veeva] {#start-veeva-sync}

1. Clique em **[!UICONTROL Iniciar Sincronização do Veeva]** para iniciar a sincronização persistente do CRM [!DNL Marketo-Veeva].

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >A Marketo não desduplicará automaticamente em uma sincronização de CRM do [!DNL Veeva] ou quando você inserir clientes potenciais manualmente.

1. Clique em **[!UICONTROL Iniciar sincronização]**.

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>O tempo para concluir a sincronização inicial varia dependendo do tamanho e da complexidade do banco de dados.

## Verificar sincronização {#verify-sync}

O Marketo fornece mensagens de status para a sincronização do CRM [!DNL Veeva] na área de Administração. Você pode verificar se a sincronização está funcionando corretamente seguindo estas etapas.

1. No Marketo, clique em **[!UICONTROL Admin]** e depois em **[!UICONTROL Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. O status da sincronização está visível no canto superior direito. Ele mostrará uma das três mensagens: Última sincronização, Sincronização em andamento ou Falha.

>[!MORELIKETHIS]
>
>[Configurar Objetos Personalizados](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}
