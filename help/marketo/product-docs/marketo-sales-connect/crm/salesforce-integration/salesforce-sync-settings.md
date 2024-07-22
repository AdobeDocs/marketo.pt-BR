---
unique-page-id: 18317669
description: Configurações De Sincronização Do Salesforce - Documentação Do Marketo - Documentação Do Produto
title: Configurações de sincronização do Salesforce
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 4%

---

# Configurações de sincronização do Salesforce {#salesforce-sync-settings}

## Registrar atividade de email no Salesforce via API {#logging-email-activity-to-salesforce-via-api}

Essa funcionalidade exige que você esteja na edição Enterprise/Unlimited do Salesforce ou na edição Professional se tiver adquirido a Integração por meio da API dos Serviços da Web.

>[!PREREQUISITES]
>
>O Salesforce e o Sales Connect devem estar conectados.

1. No Sales Connect, clique no ícone de engrenagem no canto superior direito e selecione **Configurações**.

   ![](assets/one-2.png)

1. Em Minha conta (Configurações do administrador, se você for um Administrador), clique em **Salesforce**.

   ![](assets/two-2.png)

1. Clique na guia **Configurações de sincronização**.

   ![](assets/three-1.png)

1. Clique na seta ao lado de Registrar atividade de email no Salesforce.

   ![](assets/four-1.png)

1. Clique na guia **API do Salesforce**. Neste cartão, você pode configurar sua preferência para registrar informações no Salesforce. Clique em **Salvar** quando terminar.

   ![](assets/five.png)

## Registrar atividade de email no Salesforce por email para o Salesforce (Cco) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Depois de ativar &quot;Enviar email para o Salesforce (Cco)&quot;, você receberá um CCO de seus emails de vendas e seus emails serão registrados como atividades em oportunidades, clientes potenciais e contatos.

>[!PREREQUISITES]
>
>O Salesforce e o Sales Connect devem estar conectados.

**Para registrar seus emails no Salesforce por Email (Cco)**

1. No Sales Connect, clique no ícone de engrenagem no canto superior direito e selecione **Configurações**.

   ![](assets/one-3.png)

1. Em Minha conta (Configurações do administrador, se você for um Administrador), clique em **Salesforce**.

   ![](assets/two-3.png)

1. Clique na guia **Configurações de sincronização**.

   ![](assets/three-1.png)

1. Clique na guia **Email para o Salesforce (CCO)** e clique em **Ativar**.

   ![](assets/six-2.png)

Se, por algum motivo, seu endereço de email para o Salesforce não for recebido, siga estas etapas para ativar o recurso CCO em sua conta do Salesforce:

1. Faça logon na sua instância do Salesforce.
1. Encontre seu nome de usuário no canto superior direito e selecione a barra suspensa.
1. Selecione **Minhas Configurações**.
1. Selecione **Email**.
1. Selecione **Meu email para o Salesforce**.
1. Nessa página, você verá um campo chamado &quot;Endereço de email do Salesforce&quot;. Se não houver nada preenchido ao lado dele, role até &quot;Meus endereços de email aceitáveis&quot;.
1. Digite o(s) endereço(s) de email que deseja Cco.
1. Clique em **Salvar alterações**.

**Não consigo encontrar meu email para o Salesforce em Minhas configurações**

Se você não vir Meu email para o Salesforce em suas Configurações, talvez o Administrador não o tenha ativado. Isso pode acontecer se sua equipe for nova no Salesforce ou se ela nunca tiver usado o endereço CCO fornecido pelo Salesforce.

>[!NOTE]
>
>Você precisará de privilégios de administrador para configurar isso.

1. Clique em **Instalação**.
1. Clique em **Administração de email**.
1. Clique em **Enviar email para o Salesforce**.
1. Clique em **Editar**.
1. Marque a caixa ao lado de &quot;Ativo&quot;.
1. Clique em **Salvar**.

## Sincronizar tarefas/lembretes do Sales Connect com tarefas do Salesforce {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. Clique no ícone de engrenagem no canto superior direito e selecione **Configurações**.

   ![](assets/one-3.png)

1. Em Minha conta (Configurações do administrador, se você for um Administrador), clique em **Salesforce**.

   ![](assets/two-2.png)

1. Clique na guia **Configurações de sincronização**.

   ![](assets/three-1.png)

1. Clique na seta ao lado de Sincronizar tarefas/lembretes de conexão de vendas com tarefas do Salesforce.

   ![](assets/seven-2.png)

1. Escolha a opção desejada (&quot;Não sincronizar com tarefas do Salesforce&quot; é selecionado por padrão).

   ![](assets/eight.png)
