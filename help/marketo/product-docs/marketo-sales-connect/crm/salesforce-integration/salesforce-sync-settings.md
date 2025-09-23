---
unique-page-id: 18317669
description: Configurações De Sincronização Do Salesforce - Documentação Do Marketo - Documentação Do Produto
title: Configurações de sincronização do Salesforce
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 3%

---

# Configurações de sincronização do Salesforce {#salesforce-sync-settings}

## Registrar atividade de email no Salesforce por meio da API {#logging-email-activity-to-salesforce-via-api}

Essa funcionalidade exige que você esteja na edição Enterprise/Unlimited do Salesforce ou na edição Professional se tiver adquirido a Integração por meio da API dos Serviços da Web.

>[!PREREQUISITES]
>
>O Salesforce e o Sales Connect devem estar conectados.

1. Em [!DNL Sales Connect], clique no ícone de engrenagem no canto superior direito e selecione **[!UICONTROL Configurações]**.

   ![](assets/one-2.png)

1. Em [!UICONTROL Minha conta] ([!UICONTROL Configurações do administrador], se você for um Administrador), clique em **[!UICONTROL Salesforce]**.

   ![](assets/two-2.png)

1. Clique na guia **[!UICONTROL Configurações de sincronização]**.

   ![](assets/three-1.png)

1. Clique na seta ao lado de Registrar Atividade de Email em [!DNL Salesforce].

   ![](assets/four-1.png)

1. Clique na guia **[!UICONTROL Salesforce API]**. Neste cartão, você pode configurar sua preferência por informações de log para [!DNL Salesforce]. Clique em **[!UICONTROL Salvar]** quando terminar.

   ![](assets/five.png)

## Registrar atividade de email no Salesforce por email no Salesforce (Cco) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Depois de ativar &quot;Email para Salesforce (Cco)&quot;, você receberá um CCO de seus emails de vendas e seus emails serão registrados como atividades em oportunidades, leads e contatos.

>[!PREREQUISITES]
>
>[!DNL Salesforce] e [!DNL Sales Connect] devem estar conectados.

**Para registrar seus emails no Salesforce por Email (Cco)**

1. Em [!UICONTROL Sales Connect], clique no ícone de engrenagem no canto superior direito e selecione **[!UICONTROL Configurações]**.

   ![](assets/one-3.png)

1. Em [!UICONTROL Minha conta] ([!UICONTROL Configurações do administrador], se você for um Administrador), clique em **[!UICONTROL Salesforce]**.

   ![](assets/two-3.png)

1. Clique na guia **[!UICONTROL Configurações de sincronização]**.

   ![](assets/three-1.png)

1. Clique na guia **[!UICONTROL Email to Salesforce (Cco)]** e clique em **[!UICONTROL Ativar]**.

   ![](assets/six-2.png)

Se, por algum motivo, seu endereço de Email para [!DNL Salesforce] não for recebido, siga estas etapas para ativar o recurso CCO na sua conta do [!DNL Salesforce]:

1. Faça logon na instância do [!DNL Salesforce].
1. Encontre seu nome de usuário no canto superior direito e selecione a barra suspensa.
1. Selecione **[!UICONTROL Minhas Configurações]**.
1. Selecione **[!UICONTROL Email]**.
1. Selecione **[!UICONTROL Meu Email para o Salesforce]**.
1. Nessa página, você verá um campo chamado &quot;Endereço de email do Salesforce&quot;. Se não houver nada preenchido ao lado dele, role até &quot;Meus endereços de email aceitáveis&quot;.
1. Digite o(s) endereço(s) de email que deseja Cco.
1. Clique em **[!UICONTROL Salvar alterações]**.

**Não é possível localizar meu email para [!DNL Salesforce] em Minhas Configurações**

Se você não vir Meu email para o Salesforce em suas Configurações, talvez o Administrador não o tenha ativado. Isso pode acontecer se sua equipe for nova no [!DNL Salesforce] ou se sua equipe nunca tiver usado o endereço CCO fornecido pelo [!DNL Salesforce].

>[!NOTE]
>
>Você precisará de privilégios de administrador para configurar isso.

1. Clique em **[!UICONTROL Instalação]**.
1. Clique em **[!UICONTROL Administração de email]**.
1. Clique em **[!UICONTROL Enviar Email para o Salesforce]**.
1. Clique em **[!UICONTROL Editar]**.
1. Marque a caixa ao lado de &quot;[!UICONTROL Ativo]&quot;.
1. Clique em **[!UICONTROL Salvar]**.

## Sincronizar Tarefas/Lembretes da Conexão de Vendas para [!DNL Salesforce] Tarefas {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. Clique no ícone de engrenagem no canto superior direito e selecione **[!UICONTROL Configurações]**.

   ![](assets/one-3.png)

1. Em [!UICONTROL Minha conta] ([!UICONTROL Configurações do administrador], se você for um Administrador), clique em **[!UICONTROL Salesforce]**.

   ![](assets/two-2.png)

1. Clique na guia **[!UICONTROL Configurações de sincronização]**.

   ![](assets/three-1.png)

1. Clique na seta ao lado de [!UICONTROL Sincronizar tarefas/lembretes do envolvimento de vendas com as tarefas do Salesforce].

   ![](assets/seven-2.png)

1. Escolha a opção desejada (&quot;[!UICONTROL Não sincronizar com as tarefas do Salesforce]&quot; está selecionada por padrão).

   ![](assets/eight.png)
