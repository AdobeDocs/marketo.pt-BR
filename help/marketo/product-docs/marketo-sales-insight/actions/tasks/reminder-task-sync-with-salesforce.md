---
description: Sincronização de tarefas do lembrete com o Salesforce - Documentos do Marketo - Documentação do produto
title: Sincronização de Tarefa de Lembrete com o Salesforce
hide: true
hidefromtoc: true
source-git-commit: acb077e9d6e9fa4027d660ee182a13820f16ad83
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 2%

---

# Sincronização de Tarefa de Lembrete com o Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Para saber como habilitar o check-out da Sincronização de tarefas [Sincronizar Tarefas/Lembretes de Ações de Insight de Vendas para Tarefas do Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

Quando as configurações de sincronização de tarefas estiverem ativadas, os usuários verão suas tarefas de lembrete sincronizadas bidirecionalmente com o Salesforce. Isso significa que os usuários podem gerenciar tarefas do Salesforce ou de Ações de insight de vendas e se sentem confiantes de que os sistemas permanecerão alinhados.

## Sincronização do Campo de Tarefa do Lembrete {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Abaixo está uma lista dos campos de tarefa de lembrete nas Ações de Insight de Vendas e seus campos correspondentes do Salesforce que são compatíveis por meio da sincronização de tarefa bidirecional.

<table>
 <tr>
  <th>Campo de Tarefa Ações de Insight de Vendas</th>
  <th>Campo de tarefa do Salesforce</th>
  <th>Tarefa Salesforce</th>
 </tr>
 <tr>
  <td>Nome da tarefa</td>
  <td>Campo Assunto</td>
  <td>Um campo de resumo curto destinado a mostrar o título da tarefa.</td>
 </tr>
 <tr>
  <td>Status</td>
  <td>Status da tarefa</td>
  <td><p>Mostra o status da tarefa. As tarefas Ações de Insight de Vendas têm dois status que são mapeados para dois dos valores na lista de seleção de status da tarefa do Salesforce.</p>
  <p>Abrir em Ações de Insight de vendas = Não iniciado no Salesforce.</p>
  <p>Concluído em Ações de insight de vendas = Concluído no Salesforce.</p>
  <p>Os outros valores de status no Salesforce não serão sincronizados com as Ações de Insight de Vendas.</p></td>
 </tr>
 <tr>
  <td>Prioridade</td>
  <td>Prioridade</td>
  <td><p>A prioridade Ações de insight de vendas pode ser Normal ou Alta, o que mapeia para os valores de prioridade Normal e Alta no Salesforce.</p>
  <p>O valor de prioridade baixa no Salesforce não será sincronizado com as Ações de insight de vendas.</p></td>
 </tr>
 <tr>
  <td>Data de vencimento</td>
  <td>Data de vencimento</td>
  <td>A data de vencimento da tarefa.</td>
 </tr>
 <tr>
  <td>Detalhes</td>
  <td>Comentários</td>
  <td>Mostra informações mais detalhadas sobre o que deveria ser concluído com a tarefa de lembrete.</td>
 </tr>
</table>

## Sincronização de tarefas de insight de vendas com o Salesforce pela primeira vez {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

Quando você ativa a sincronização entre as Ações de insight de vendas e as tarefas do Salesforce pela primeira vez, importamos suas tarefas do Salesforce. Nós vamos **not** passe o mouse sobre qualquer tarefa atual que você tenha em Ações de insight de vendas para o Salesforce. Para reduzir a desordem e as duplicatas, as únicas tarefas sincronizadas das Ações de Insight de Vendas no Salesforce são tarefas criadas *after* sincronize Ações de insight de vendas com o SFDC.

Veja o que acontece quando você sincroniza ações de insight de vendas e tarefas SFDC:

* Assim que você clicar em salvar na sincronização de tarefas, eles começarão a sincronizar. Isso levará algum tempo inicialmente.

* Todos os lembretes que foram atualizados ou criados nas últimas 24 horas serão transferidos do SFDC para Ações de Insight de Vendas. A sincronização é baseada na data de vencimento e todas essas tarefas serão sincronizadas no back-end, mas no Centro de comando, você só verá tarefas que vencem hoje e amanhã.

* Se a sincronização tiver sido ativada anteriormente e você excluir qualquer tarefa no SFDC, qualquer coisa que tenha sido excluída nos últimos 15 dias será excluída do Centro de Comando.

* Nós sincronizaremos constantemente as tarefas entre as Ações de insight de vendas e o SFDC, desde que a sincronização esteja ativada.

Após a sincronização inicial, qualquer tarefa que você criar, editar, concluir ou excluir em Ações de Insight de vendas será sincronizada com a lista de tarefas no Salesforce. E qualquer item criado, editado, concluído ou excluído no Salesforce atualizará sua lista de tarefas em Ações de insight de vendas.

Para ativar essa sincronização, basta marcar a caixa de sincronização em seu [Página Configurações](https://toutapp.com/login) na aplicação web.

>[!NOTE]
>
>O campo de assunto de uma tarefa pode ser atualizado em Ações de Insight de Vendas e essa atualização será sincronizada no campo de assunto do Salesforce para a tarefa sincronizada correspondente, se você estiver usando o `{{activity_subject}}` campo dinâmico em seu [Personalização de detalhes da atividade](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) configurações. Por outro lado, qualquer atualização feita no campo de assunto no Salesforce _not_ sincronize com o campo de assunto da tarefa de lembrete Ações do Sales Insight.
