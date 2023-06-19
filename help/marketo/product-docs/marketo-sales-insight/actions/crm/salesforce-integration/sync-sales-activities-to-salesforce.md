---
description: Sincronizar atividades de vendas com o Salesforce - Documentação do Marketo - Documentação do produto
title: Sincronizar atividades de vendas com o Salesforce
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Sincronizar atividades de vendas com o Salesforce {#sync-sales-activities-to-salesforce}

Você pode definir as Ações Configurações de sincronização do Salesforce para registrar atividades de email e chamada para o Salesforce. Isso oferece melhor visibilidade às equipes que trabalham com seu CRM e permite que os gerentes usem essas atividades para criar relatórios personalizados do Salesforce a fim de acompanhar o desempenho de suas equipes.

## Registrar atividade de email no Salesforce via API {#logging-email-activity-to-salesforce-via-api}

Essa funcionalidade exige que você esteja na edição Enterprise/Unlimited do Salesforce ou na edição Professional se tiver adquirido a Integração por meio da API dos Serviços da Web.

>[!PREREQUISITES]
>
>As ações do Salesforce e do Sales Insight devem estar conectadas.

1. Em Ações do Sales Insight, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/sync-sales-activities-to-salesforce-1.png)

1. Em Configurações do administrador (ou &quot;Minha conta&quot; se você não for um administrador), clique em **Salesforce**.

   ![](assets/sync-sales-activities-to-salesforce-2.png)

1. Clique em **Configurações de sincronização** guia.

   ![](assets/sync-sales-activities-to-salesforce-3.png)

1. Clique na seta ao lado de Registrar atividade de email no Salesforce.

   ![](assets/sync-sales-activities-to-salesforce-4.png)

1. Clique em **API do Salesforce** guia. Neste cartão, você pode configurar sua preferência para registrar informações no Salesforce. Clique em **Salvar** quando terminar.

   ![](assets/sync-sales-activities-to-salesforce-5.png)

## Registrar atividade de email no Salesforce por email para o Salesforce (Cco) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Depois de ativar &quot;Enviar email para o Salesforce (Cco)&quot;, você receberá um CCO de seus emails de vendas e seus emails serão registrados como atividades em oportunidades, clientes potenciais e contatos.

>[!PREREQUISITES]
>
>As ações do Salesforce e do Sales Insight devem estar conectadas.

**Para registrar seus emails no Salesforce por email (Cco)**

1. No Marketo Sales, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/sync-sales-activities-to-salesforce-6.png)

1. Em Configurações do administrador (ou &quot;Minha conta&quot; se você não for um administrador), clique em **Salesforce**.

   ![](assets/sync-sales-activities-to-salesforce-7.png)

1. Clique em **Configurações de sincronização** guia.

   ![](assets/sync-sales-activities-to-salesforce-8.png)

1. Clique em **Enviar email para o Salesforce (Cco)** e clique em **Ativar**.

   ![](assets/sync-sales-activities-to-salesforce-9.png)

Se, por algum motivo, seu endereço de email para o Salesforce não for recebido, siga estas etapas para ativar o recurso CCO em sua conta do Salesforce:

1. Faça logon na sua instância do Salesforce.
1. Encontre seu nome de usuário no canto superior direito e selecione a barra suspensa.
1. Selecionar **Minhas configurações**.
1. Selecionar **E-mail**.
1. Selecionar **Meu email para o Salesforce**.
1. Nessa página, você verá um campo chamado &quot;Endereço de email do Salesforce&quot;. Se não houver nada preenchido ao lado dele, role até &quot;Meus endereços de email aceitáveis&quot;.
1. Digite o(s) endereço(s) de email que deseja Cco.
1. Clique em **Salvar alterações**.

**Não consigo encontrar meu email para o Salesforce em Minhas configurações**

Se você não vir Meu email para o Salesforce em suas Configurações, talvez o Administrador não o tenha ativado. Isso pode acontecer se sua equipe for nova no Salesforce ou se ela nunca tiver usado o endereço CCO fornecido pelo Salesforce.

>[!NOTE]
>
>Você precisará de privilégios de administrador para configurar isso.

1. Clique em **Configuração**.
1. Clique em **Administração de e-mail**.
1. Clique em **Enviar email para o Salesforce**.
1. Clique em **Editar**.
1. Marque a caixa ao lado de &quot;Ativo&quot;.
1. Clique em **Salvar**.

## Sincronizar tarefas/lembretes de ações do Sales Insight com tarefas do Salesforce {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. Em Ações do Sales Insight, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/sync-sales-activities-to-salesforce-10.png)

1. Em Configurações do administrador (ou &quot;Minha conta&quot; se você não for um administrador), clique em **Salesforce**.

   ![](assets/sync-sales-activities-to-salesforce-11.png)

1. Clique em **Configurações de sincronização** guia.

   ![](assets/sync-sales-activities-to-salesforce-12.png)

1. Clique na seta ao lado de Sincronizar tarefas/lembretes de vendas do Marketo com tarefas do Salesforce.

   ![](assets/sync-sales-activities-to-salesforce-13.png)

1. Escolha a opção desejada (&quot;Não sincronizar com tarefas do Salesforce&quot; é selecionado por padrão).

   ![](assets/sync-sales-activities-to-salesforce-14.png)

## Sincronizando pela primeira vez as tarefas de ações do Sales Insight com o Salesforce {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

Quando você ativa a sincronização entre as Ações do Sales Insight e as tarefas do Salesforce pela primeira vez, importamos suas tarefas do Salesforce. Não transferiremos nenhuma tarefa atual que você tenha em Ações de insights de vendas para o Salesforce. Para reduzir a desordem e as duplicatas, as únicas tarefas que são sincronizadas das Ações do Sales Insight no Salesforce são tarefas criadas após você sincronizar as Ações do Sales Insight com o SFDC.

Veja o que acontece quando você sincroniza as Ações do Sales Insight e as tarefas do SFDC:

* Assim que você clicar em salvar na sincronização de tarefas, elas começarão a sincronizar. Isso levará algum tempo inicialmente.

* Qualquer lembrete que tenha sido atualizado ou criado nas últimas 24 horas será enviado do SFDC para as ações do Sales Insight. A sincronização é baseada na data de conclusão e todas essas tarefas serão sincronizadas no back-end, mas no Command Center, você só verá tarefas com data de conclusão para hoje e amanhã.

* Se a sincronização tiver sido ativada anteriormente e você excluir qualquer tarefa no SFDC, qualquer item que tiver sido excluído nos últimos 15 dias será excluído do Centro de comando.

* Sincronizaremos constantemente as tarefas entre as ações do Sales Insight e o SFDC enquanto a sincronização estiver habilitada.

* Após a sincronização inicial, todas as tarefas que você criar, editar, concluir ou excluir nas Ações do Sales Insight serão sincronizadas com sua lista de tarefas no Salesforce. Qualquer coisa criada, editada, concluída ou excluída no Salesforce atualizará sua lista de tarefas em Ações de insight de vendas.

* Para ativar essa sincronização, marque a caixa de sincronização na página Configurações no aplicativo Web.
