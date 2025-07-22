---
description: Configurações De Sincronização Do Salesforce - Documentação Do Marketo - Documentação Do Produto
title: Configurações de sincronização do Salesforce
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 1%

---

# Configurações de Sincronização de [!DNL Salesforce] {#salesforce-sync-settings}

## Registrando Atividade de Email em Log para [!DNL Salesforce] via API {#logging-email-activity-to-salesforce-via-api}

Essa funcionalidade exige que você esteja na edição Enterprise/Unlimited do [!DNL Salesforce] ou na edição Professional se tiver adquirido a Integração pela API dos Serviços da Web.

>[!PREREQUISITES]
>
>[!DNL Salesforce] e [!DNL Sales Insight Actions] devem estar conectados.

1. Em [!DNL Sales Insight Actions], clique no ícone de engrenagem e selecione **[!UICONTROL Configurações]**.

   ![](assets/salesforce-sync-settings-1.png)

1. Em [!UICONTROL Configurações de Administrador] (ou &quot;[!UICONTROL Minha Conta]&quot; se você não for um Administrador), clique em **[!UICONTROL Salesforce]**.

   ![](assets/salesforce-sync-settings-2.png)

1. Clique na guia **[!UICONTROL Configurações de sincronização]**.

   ![](assets/salesforce-sync-settings-3.png)

1. Clique na seta ao lado de [!UICONTROL Registrar Atividade de Email] em [!DNL Salesforce].

   ![](assets/salesforce-sync-settings-4.png)

1. Clique na guia **[!UICONTROL Salesforce API]**. Neste cartão, você pode configurar sua preferência por informações de log para [!DNL Salesforce]. Clique em **[!UICONTROL Salvar]** quando terminar.

   ![](assets/salesforce-sync-settings-5.png)

## Registrando Atividade de Email em Log para [!DNL Salesforce] via Email para [!DNL Salesforce] (Cco) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Depois de ativar &quot;[!UICONTROL Email para Salesforce (CCO)]&quot;, você receberá um CCO de seus emails de vendas e seus emails serão registrados como atividades em oportunidades, clientes potenciais e contatos.

>[!PREREQUISITES]
>
>[!DNL Salesforce] e [!DNL Sales Insight Actions] devem estar conectados.

**Para registrar seus emails em [!DNL Salesforce] via Email (Cco)**

1. No Marketo Sales, clique no ícone de engrenagem e selecione **[!UICONTROL Configurações]**.

   ![](assets/salesforce-sync-settings-6.png)

1. Em [!UICONTROL Configurações de Administrador] (ou &quot;[!UICONTROL Minha Conta]&quot; se você não for um Administrador), clique em **[!UICONTROL Salesforce]**.

   ![](assets/salesforce-sync-settings-7.png)

1. Clique na guia **[!UICONTROL Configurações de sincronização]**.

   ![](assets/salesforce-sync-settings-8.png)

1. Clique na guia **[!UICONTROL Email to Salesforce (Cco)]** e clique em **[!UICONTROL Ativar]**.

   ![](assets/salesforce-sync-settings-9.png)

Se, por algum motivo, seu endereço de Email para [!DNL Salesforce] não for recebido, siga estas etapas para ativar o recurso CCO na sua conta do [!DNL Salesforce]:

1. Faça logon na instância do [!DNL Salesforce].
1. Encontre seu nome de usuário no canto superior direito e selecione a barra suspensa.
1. Selecione **[!UICONTROL Minhas Configurações]**.
1. Selecione **[!UICONTROL Email]**.
1. Selecione **[!UICONTROL Meu Email para o Salesforce]**.
1. Nesta página, você verá um campo rotulado como &quot;[!UICONTROL Endereço de email do Salesforce]&quot;. Se não houver nada preenchido ao lado dele, role para baixo até &quot;[!UICONTROL Meus Endereços de Email Aceitáveis]&quot;.
1. Digite o(s) endereço(s) de email que deseja Cco.
1. Clique em **[!UICONTROL Salvar alterações]**.

**Não é possível localizar meu email para [!DNL Salesforce] em Minhas Configurações**

Se você não vir Meu Email para [!DNL Salesforce] em suas Configurações, talvez o Administrador não o tenha habilitado. Isso pode acontecer se sua equipe for nova no [!DNL Salesforce] ou se sua equipe nunca tiver usado o endereço CCO fornecido pelo [!DNL Salesforce].

>[!NOTE]
>
>Você precisará de privilégios de administrador para configurar isso.

1. Clique em **[!UICONTROL Instalação]**.
1. Clique em **[!UICONTROL Administração de email]**.
1. Clique em **[!UICONTROL Enviar Email para o Salesforce]**.
1. Clique em **[!UICONTROL Editar]**.
1. Marque a caixa ao lado de &quot;Ativo&quot;.
1. Clique em **[!UICONTROL Salvar]**.

## Sincronizar [!DNL Sales Insight Actions] Tarefas/Lembretes para [!DNL Salesforce] Tarefas {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. Em [!DNL Sales Insight Actions], clique no ícone de engrenagem e selecione **[!UICONTROL Configurações]**.

   ![](assets/salesforce-sync-settings-10.png)

1. Em [!UICONTROL Configurações de Administrador] (ou &quot;[!UICONTROL Minha Conta]&quot; se você não for um Administrador), clique em **[!UICONTROL Salesforce]**.

   ![](assets/salesforce-sync-settings-11.png)

1. Clique na guia **[!UICONTROL Configurações de sincronização]**.

   ![](assets/salesforce-sync-settings-12.png)

1. Clique na seta ao lado de Sincronizar tarefas/lembretes de vendas do Marketo com [!DNL Salesforce] tarefas.

   ![](assets/salesforce-sync-settings-13.png)

1. Escolha a opção desejada (&quot;Não sincronizar com [!DNL Salesforce] tarefas&quot; é selecionada por padrão).

   ![](assets/salesforce-sync-settings-14.png)

## Sincronizando [!DNL Sales Insight Actions] Tarefas com [!DNL Salesforce] pela primeira vez {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

Quando você ativa a sincronização entre as tarefas do [!DNL Sales Insight Actions] e do [!DNL Salesforce] pela primeira vez, nós importamos suas tarefas do [!DNL Salesforce]. Não enviaremos nenhuma tarefa atual que você tenha em [!DNL Sales Insight Actions] para [!DNL Salesforce]. Para reduzir a desordem e as duplicatas, as únicas tarefas que são sincronizadas de [!DNL Sales Insight Actions] para [!DNL Salesforce] são as tarefas criadas após a sincronização de [!DNL Sales Insight Actions] com o SFDC.

Veja o que acontece quando você sincroniza tarefas do [!DNL Sales Insight Actions] e do SFDC:

Assim que você clicar em salvar na sincronização de tarefas, elas começarão a sincronizar. Isso levará algum tempo inicialmente.

Todos os lembretes atualizados ou criados nas últimas 24 horas serão extraídos do SFDC para [!DNL Sales Insight Actions]. A sincronização é baseada na data de conclusão e todas essas tarefas serão sincronizadas no back-end, mas no Command Center, você só verá tarefas com data de conclusão para hoje e amanhã.

Se a sincronização tiver sido ativada anteriormente e você excluir qualquer tarefa no SFDC, qualquer item excluído nos últimos 15 dias será excluído do Centro de comando.

Sincronizaremos constantemente tarefas entre o [!DNL Sales Insight Actions] e o SFDC enquanto a sincronização estiver habilitada.

Após a sincronização inicial, todas as tarefas que você criar, editar, concluir ou excluir no [!DNL Sales Insight Actions] serão sincronizadas com a sua lista de tarefas no [!DNL Salesforce]. Qualquer ação criada, editada, concluída ou excluída no [!DNL Salesforce] atualizará sua lista de tarefas no [!DNL Sales Insight Actions].

Para ativar esta sincronização, marque a caixa de sincronização na página [!UICONTROL Configurações] do aplicativo Web.
