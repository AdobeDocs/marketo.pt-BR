---
description: Sincronização de tarefas de lembrete com o Salesforce - Documentação do Marketo - Documentação do produto
title: Lembrete de sincronização de tarefas com o Salesforce
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 2%

---

# Lembrete de sincronização de tarefas com o Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Para saber como habilitar a Sincronização de Tarefas, confira [Sincronizar Tarefas/Lembretes de Ações de Insight de Vendas com Tarefas do Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

Quando as configurações de sincronização de tarefas estiverem habilitadas, os usuários verão suas tarefas de lembrete sincronizadas bidirecionalmente com o Salesforce. Isso significa que os usuários podem gerenciar tarefas das ações Salesforce ou Sales Insight e ter certeza de que os sistemas permanecerão alinhados.

## Sincronização de Campo de Tarefa de Lembrete {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Abaixo está uma lista dos campos de tarefa de lembrete em Ações do Sales Insight e seus campos correspondentes do Salesforce que são suportados por meio da sincronização bidirecional de tarefas.

<table>
 <tr>
  <th>Campo de Tarefas Ações do Sales Insight</th>
  <th>Campo de tarefas do Salesforce</th>
  <th>Tarefa do Salesforce</th>
 </tr>
 <tr>
  <td>Nome da tarefa</td>
  <td>Campo de assunto</td>
  <td>Um pequeno campo de resumo deve mostrar o título da tarefa.</td>
 </tr>
 <tr>
  <td>Status</td>
  <td>Status da tarefa</td>
  <td><p>Mostra o status da tarefa. As tarefas de Ações de Insight de Vendas têm dois status que mapeiam para dois dos valores na lista de opções de status da tarefa do Salesforce.</p>
  <p>Abrir em Ações do Sales Insight = Não iniciado no Salesforce.</p>
  <p>Concluir em ações do Sales Insight = Concluído no Salesforce.</p>
  <p>Os outros valores de status no Salesforce não serão sincronizados com as Ações do Sales Insight.</p></td>
 </tr>
 <tr>
  <td>Prioridade</td>
  <td>Prioridade</td>
  <td><p>A prioridade das Ações do Sales Insight pode ser Normal ou Alta, que é mapeada para os valores de prioridade Normal e Alta no Salesforce.</p>
  <p>O valor de prioridade baixa no Salesforce não será sincronizado com as ações do Sales Insight.</p></td>
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

## Sincronizando pela primeira vez as tarefas de ações do Sales Insight com o Salesforce {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

Quando você ativa a sincronização entre as Ações do Sales Insight e as tarefas do Salesforce pela primeira vez, importamos suas tarefas do Salesforce. Nós **não** transferiremos quaisquer tarefas atuais que você tenha em Ações de insights de vendas para o Salesforce. Para reduzir a desordem e as duplicatas, as únicas tarefas que são sincronizadas das Ações do Sales Insight no Salesforce são tarefas criadas *depois* de você sincronizar as Ações do Sales Insight com o SFDC.

Veja o que acontece quando você sincroniza as Ações do Sales Insight e as tarefas do SFDC:

* Assim que você clicar em salvar na sincronização de tarefas, elas começarão a sincronizar. Isso levará algum tempo inicialmente.

* Qualquer lembrete que tenha sido atualizado ou criado nas últimas 24 horas será enviado do SFDC para as ações do Sales Insight. A sincronização é baseada na data de conclusão e todas essas tarefas serão sincronizadas no back-end, mas no Command Center, você só verá tarefas com data de conclusão para hoje e amanhã.

* Se a sincronização tiver sido ativada anteriormente e você excluir qualquer tarefa no SFDC, qualquer item que tiver sido excluído nos últimos 15 dias será excluído do Centro de comando.

* Sincronizaremos constantemente as tarefas entre as ações do Sales Insight e o SFDC enquanto a sincronização estiver habilitada.

Após a sincronização inicial, todas as tarefas que você criar, editar, concluir ou excluir nas Ações do Sales Insight serão sincronizadas com sua lista de tarefas no Salesforce. Qualquer coisa criada, editada, concluída ou excluída no Salesforce atualizará sua lista de tarefas em Ações de insight de vendas.

Para ativar esta sincronização, marque a caixa de sincronização na [página Configurações](https://toutapp.com/login) do aplicativo Web.

>[!NOTE]
>
>O campo de assunto de uma tarefa pode ser atualizado em Ações de Insight de vendas e essa atualização será sincronizada no campo de assunto do Salesforce para a tarefa sincronizada correspondente, se você estiver usando o campo dinâmico `{{activity_subject}}` nas configurações de [Personalização de detalhes da atividade](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md). Por outro lado, qualquer atualização feita no campo de assunto no Salesforce _não_ sincronizará com o campo de assunto da tarefa de lembrete de Ações do Sales Insight.
