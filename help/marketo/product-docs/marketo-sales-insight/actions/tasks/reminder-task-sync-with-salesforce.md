---
description: Sincronização de tarefa de lembrete com o Salesforce - Documentação do Marketo - Documentação do produto
title: Sincronização de tarefa de lembrete com o Salesforce
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 1%

---

# Sincronização de Tarefa de Lembrete com [!DNL Salesforce] {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Para saber como habilitar a Sincronização de Tarefas, confira [Sincronizar Tarefas/Lembretes de Ações de Insight de Vendas com Tarefas do Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

Quando as configurações de sincronização de tarefa estiverem habilitadas, os usuários verão suas tarefas de lembrete sincronizadas bidirecionalmente com o [!DNL Salesforce]. Isso significa que os usuários podem gerenciar tarefas a partir do [!DNL Salesforce] ou do [!DNL Sales Insight Actions] e ter certeza de que os sistemas permanecerão alinhados.

## Sincronização de Campo de Tarefa de Lembrete {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Abaixo está uma lista dos campos de tarefa de lembrete em [!DNL Sales Insight Actions] e seus campos [!DNL Salesforce] correspondentes que são suportados por meio da sincronização de tarefa bidirecional.

<table>
 <tr>
  <th>[!DNL Sales Insight Actions] Campo de tarefa</th>
  <th>[!DNL Salesforce] Campo de tarefa</th>
  <th>[!DNL Salesforce] Tarefa</th>
 </tr>
 <tr>
  <td>[!UICONTROL Nome da Tarefa]</td>
  <td>[!UICONTROL Campo de Assunto]</td>
  <td>Um pequeno campo de resumo deve mostrar o título da tarefa.</td>
 </tr>
 <tr>
  <td>[!UICONTROL Status]</td>
  <td>[!UICONTROL Status da Tarefa]</td>
  <td><p>Mostra o status da tarefa. [!DNL Sales Insight Actions] tarefas têm dois status que são mapeados para dois dos valores da lista de opções de status de tarefa [!DNL Salesforce].</p>
  <p>Abrir em [!DNL Sales Insight Actions] = Não iniciado em [!DNL Salesforce].</p>
  <p>Concluído em [!DNL Sales Insight Actions] = Concluído em [!DNL Salesforce].</p>
  <p>Os outros valores de status em [!DNL Salesforce] não serão sincronizados com [!DNL Sales Insight Actions].</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Prioridade]</td>
  <td>[!UICONTROL Prioridade]</td>
  <td><p>[!DNL Sales Insight Actions] A prioridade pode ser Normal ou Alta, que mapeia os valores de prioridade Normal e Alta em [!DNL Salesforce].</p>
  <p>O valor de prioridade baixa em [!DNL Salesforce] não será sincronizado com [!DNL Sales Insight Actions].</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Data de Conclusão]</td>
  <td>[!UICONTROL Data de Conclusão]</td>
  <td>A data de vencimento da tarefa.</td>
 </tr>
 <tr>
  <td>[!UICONTROL Detalhes]</td>
  <td>[!UICONTROL Comentários]</td>
  <td>Mostra informações mais detalhadas sobre o que deveria ser concluído com a tarefa de lembrete.</td>
 </tr>
</table>

## Sincronizando [!DNL Sales Insight Actions] Tarefas com [!DNL Salesforce] pela primeira vez {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

Quando você ativa a sincronização entre as tarefas do [!DNL Sales Insight Actions] e do [!DNL Salesforce] pela primeira vez, nós importamos suas tarefas do [!DNL Salesforce]. Nós **não** transferiremos quaisquer tarefas atuais que você tenha em [!DNL Sales Insight Actions] para [!DNL Salesforce]. Para reduzir a desordem e as duplicatas, as únicas tarefas que são sincronizadas de [!DNL Sales Insight Actions] para [!DNL Salesforce] são tarefas criadas *depois* que você sincroniza [!DNL Sales Insight Actions] com o SFDC.

Veja o que acontece quando você sincroniza tarefas do [!DNL Sales Insight Actions] e do SFDC:

* Assim que você clicar em salvar na sincronização de tarefas, elas começarão a sincronizar. Isso levará algum tempo inicialmente.

* Todos os lembretes atualizados ou criados nas últimas 24 horas serão extraídos do SFDC para [!DNL Sales Insight Actions]. A sincronização é baseada na data de conclusão e todas essas tarefas serão sincronizadas no back-end, mas no Command Center, você só verá tarefas com data de conclusão para hoje e amanhã.

* Se a sincronização tiver sido ativada anteriormente e você excluir qualquer tarefa no SFDC, qualquer item excluído nos últimos 15 dias será excluído do Centro de comando.

* Sincronizaremos constantemente as tarefas entre o [!DNL Sales Insight Actions] e o SFDC enquanto a sincronização estiver habilitada.

Após a sincronização inicial, todas as tarefas que você criar, editar, concluir ou excluir no [!DNL Sales Insight Actions] serão sincronizadas com a sua lista de tarefas no [!DNL Salesforce]. Qualquer ação criada, editada, concluída ou excluída no [!DNL Salesforce] atualizará sua lista de tarefas no [!DNL Sales Insight Actions].

Para ativar esta sincronização, marque a caixa de sincronização na [página Configurações](https://toutapp.com/login) do aplicativo Web.

>[!NOTE]
>
>O campo de assunto de uma tarefa pode ser atualizado em [!DNL Sales Insight Actions] e essa atualização será sincronizada no campo de assunto [!DNL Salesforce] da tarefa sincronizada correspondente, se você estiver usando o campo dinâmico `{{activity_subject}}` nas configurações de [Personalização de Detalhes da Atividade](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md). Por outro lado, qualquer atualização feita no campo de assunto em [!DNL Salesforce] irá *não* sincronizar para o campo de assunto da tarefa de lembrete [!DNL Sales Insight Actions].
