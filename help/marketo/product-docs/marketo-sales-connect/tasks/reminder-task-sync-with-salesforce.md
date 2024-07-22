---
description: Sincronização de tarefas de lembrete com o Salesforce - Documentação do Marketo - Documentação do produto
title: Lembrete de sincronização de tarefas com o Salesforce
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 2%

---

# Lembrete de sincronização de tarefas com o Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Para saber como habilitar a Sincronização de Tarefas, confira [Sincronizar Tarefas/Lembretes do Sales Connect com Tarefas do Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

Quando as configurações de sincronização de tarefas estiverem habilitadas, os usuários verão suas tarefas de lembrete sincronizadas bidirecionalmente com o Salesforce. Isso significa que os usuários podem gerenciar tarefas do Salesforce ou do Sales Connect e ter certeza de que os sistemas permanecerão alinhados.

## Sincronização de Campo de Tarefa de Lembrete {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Abaixo está uma lista dos campos de tarefa de lembrete no Sales Connect e seus campos correspondentes do Salesforce que são suportados por meio da sincronização de tarefa bidirecional.

<table>
 <tr>
  <th>Campo de Tarefa Conexão de Vendas</th>
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
  <td><p>Mostra o status da tarefa. As tarefas do Sales Connect têm dois status que são mapeados para dois dos valores na lista de opções de status da tarefa do Salesforce.</p>
  <p>Abrir no Sales Connect = Não iniciado no Salesforce.</p>
  <p>Concluído no Sales Connect = Concluído no Salesforce.</p>
  <p>Os outros valores de status no Salesforce não serão sincronizados com o Sales Connect.</p></td>
 </tr>
 <tr>
  <td>Prioridade</td>
  <td>Prioridade</td>
  <td><p>A prioridade Conexão de vendas pode ser Normal ou Alta, que é mapeada para os valores de prioridade Normal e Alta no Salesforce.</p>
  <p>O valor de prioridade baixa no Salesforce não será sincronizado com o Sales Connect.</p></td>
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

## Sincronizando pela primeira vez as tarefas do Sales Connect com o Salesforce {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Quando você ativa a sincronização entre as tarefas do Sales Connect e do Salesforce pela primeira vez, importamos suas tarefas do Salesforce. Nós **não** transferiremos quaisquer tarefas atuais que você tenha no Sales Connect para o Salesforce. Para reduzir a desordem e as duplicatas, as únicas tarefas que são sincronizadas do Sales Connect no Salesforce são as tarefas criadas *depois* de você sincronizar o Sales Connect com o SFDC.

Veja o que acontece quando você sincroniza tarefas do Sales Connect e do SFDC:

* Assim que você clicar em salvar na sincronização de tarefas, elas começarão a sincronizar. Isso levará algum tempo inicialmente.

* Qualquer lembrete que tenha sido atualizado ou criado nas últimas 24 horas será enviado do SFDC para o Sales Connect. A sincronização é baseada na data de conclusão e todas essas tarefas serão sincronizadas no back-end, mas no Command Center, você só verá tarefas com data de conclusão para hoje e amanhã.

* Se a sincronização tiver sido ativada anteriormente e você excluir qualquer tarefa no SFDC, qualquer item que tiver sido excluído nos últimos 15 dias será excluído do Centro de comando.

* Sincronizaremos constantemente as tarefas entre o Sales Connect e o SFDC enquanto a sincronização estiver habilitada.

Após a sincronização inicial, todas as tarefas que você criar, editar, concluir ou excluir no Sales Connect serão sincronizadas com sua lista de tarefas no Salesforce. Qualquer ação criada, editada, concluída ou excluída no Salesforce atualizará sua lista de tarefas no Sales Connect.

Para ativar esta sincronização, marque a caixa de sincronização na [página Configurações](https://toutapp.com/login) do aplicativo Web.

>[!NOTE]
>
>O campo de assunto de uma tarefa pode ser atualizado no Sales Connect e essa atualização será sincronizada no campo de assunto do Salesforce da tarefa sincronizada correspondente, se você estiver usando o campo dinâmico `{{activity_subject}}` nas configurações de [Personalização de detalhes da atividade](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md). Por outro lado, qualquer atualização feita no campo de assunto no Salesforce _não_ sincronizará com o campo de assunto da tarefa de lembrete do Sales Connect.
