---
description: Sincronização de tarefas do lembrete com o Salesforce - Documentos do Marketo - Documentação do produto
title: Sincronização de Tarefa de Lembrete com o Salesforce
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
source-git-commit: d2d6d4389f5a480afdfae6bfb62b9f48f0a2d88e
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 2%

---

# Sincronização de Tarefa de Lembrete com o Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Para saber como habilitar o check-out da Sincronização de tarefas [Sincronizar Tarefas/Lembretes de Ligação de Vendas para Tarefas do Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

Quando as configurações de sincronização de tarefas estiverem ativadas, os usuários verão suas tarefas de lembrete sincronizadas bidirecionalmente com o Salesforce. Isso significa que os usuários podem gerenciar tarefas do Salesforce ou do Sales Connect e se sentem confiantes de que os sistemas permanecerão alinhados.

## Sincronização do Campo de Tarefa do Lembrete {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Abaixo está uma lista dos campos de tarefa de lembrete no Sales Connect e seus campos correspondentes do Salesforce que são compatíveis por meio da sincronização de tarefa bidirecional.

<table>
 <tr>
  <th>Campo Tarefa Conexão de Vendas</th>
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
  <td><p>Mostra o status da tarefa. As tarefas de Conexão de Vendas têm dois status que são mapeados para dois valores na lista de seleção de status de tarefa do Salesforce.</p>
  <p>Abrir em Conexão de Vendas = Não Iniciado no Salesforce.</p>
  <p>Concluído em Conexão de Vendas = Concluído no Salesforce.</p>
  <p>Os outros valores de status no Salesforce não serão sincronizados com o Sales Connect.</p></td>
 </tr>
 <tr>
  <td>Prioridade</td>
  <td>Prioridade</td>
  <td><p>A prioridade Conexão de Vendas pode ser Normal ou Alta, o que mapeia para os valores de prioridade Normal e Alta no Salesforce.</p>
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

## Sincronização de Tarefas de Conexão de Vendas com o Salesforce pela Primeira Vez {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Quando você ativa a sincronização entre as tarefas do Sales Connect e do Salesforce pela primeira vez, importamos suas tarefas do Salesforce. Nós vamos **not** passe o mouse sobre qualquer tarefa atual que você tenha no Sales Connect para o Salesforce. Para reduzir a desordem e as duplicatas, as únicas tarefas sincronizadas do Sales Connect no Salesforce são tarefas criadas *after* sincronize o Sales Connect com o SFDC.

Veja o que acontece quando você sincroniza tarefas do Sales Connect e do SFDC:

* Assim que você clicar em salvar na sincronização de tarefas, eles começarão a sincronizar. Isso levará algum tempo inicialmente.

* Todos os lembretes que foram atualizados ou criados nas últimas 24 horas serão transferidos do SFDC para o Sales Connect. A sincronização é baseada na data de vencimento e todas essas tarefas serão sincronizadas no back-end, mas no Centro de comando, você só verá tarefas que vencem hoje e amanhã.

* Se a sincronização tiver sido ativada anteriormente e você excluir qualquer tarefa no SFDC, qualquer coisa que tenha sido excluída nos últimos 15 dias será excluída do Centro de Comando.

* Sincronizaremos tarefas constantemente entre o Sales Connect e o SFDC, desde que a sincronização esteja ativada.

Após a sincronização inicial, qualquer tarefa que você criar, editar, concluir ou excluir no Sales Connect será sincronizada com a lista de tarefas no Salesforce. E qualquer item criado, editado, concluído ou excluído no Salesforce atualizará sua lista de tarefas no Sales Connect.

Para ativar essa sincronização, basta marcar a caixa de sincronização em seu [Página Configurações](https://toutapp.com/login) na aplicação web.

>[!NOTE]
>
>O campo de assunto de uma tarefa pode ser atualizado no Sales Connect e essa atualização será sincronizada no campo de assunto do Salesforce para a tarefa sincronizada correspondente, se você estiver usando o `{{activity_subject}}` campo dinâmico em seu [Personalização de detalhes da atividade](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) configurações. Por outro lado, qualquer atualização feita no campo de assunto no Salesforce _not_ sincronize para o campo de assunto da tarefa de lembrete do Sales Connect.
