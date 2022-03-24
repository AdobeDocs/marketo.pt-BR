---
description: Configurar a personalização de detalhes da atividade do Salesforce - Documentos do Marketo - Documentação do produto
title: Configurar Personalização De Detalhes Da Atividade Do Salesforce
hide: true
hidefromtoc: true
exl-id: 534ebdb5-7a5b-48eb-98f7-2d05a9eae8e8
source-git-commit: 43878490538ad5485c9e6d7aa0c7f8f1b443ad8c
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# Configurar Personalização De Detalhes Da Atividade Do Salesforce {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* Ações do Salesforce e do Sales Insight [deve estar conectado](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md)
>* Registro da atividade de email via API [deve estar habilitado](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)


A Personalização de detalhes da atividade permite que os administradores configurem as informações que farão logon no campo Tarefa do Salesforce - Assunto, quando uma atividade/tarefa de lembrete Ações de insight de vendas for sincronizada com o Salesforce.

>[!NOTE]
>
>* As atualizações feitas no campo de assunto em Ações de Insight de Vendas de uma tarefa de lembrete serão refletidas no campo de assunto da tarefa do Salesforce correspondente, se você estiver usando o `{{activity_subject}}` campo dinâmico na Personalização de detalhes da atividade.
>* Quebras de linha não são compatíveis ao registrar informações no campo de assunto do Salesforce. Qualquer quebra de linha no editor Personalização de detalhes da atividade será removida quando um assunto da tarefa de vendas for atualizado.


![](assets/configure-salesforce-activity-detail-customization-1.png)

![](assets/configure-salesforce-activity-detail-customization-2.png)

<table>
 <tr>
  <td><strong>1</td>
  <td>Tarefa do Lembrete de InMail</td>
 </tr>
 <tr>
  <td><strong>2</td>
  <td>Atividade de e-mail</td>
 </tr>
 <tr>
  <td><strong>3</td>
  <td>Atividade de chamada</td>
 </tr>
</table>

O recurso pode ser usado para desbloquear os seguintes benefícios:

* Ao personalizar quais informações estão visíveis no campo de assunto, os detalhes da atividade são facilmente verificáveis para vendas no Salesforce.
* Os administradores podem marcar o campo de assunto com um identificador exclusivo, como &quot;Mkto_sales&quot;, para que as atividades das Ações de insight de vendas possam ser facilmente identificadas e diferenciadas de outras atividades de email, atividades de chamada e tarefas.
* Reduza a necessidade de campos de atividade personalizados. O Salesforce impõe limites no número de campos de atividade personalizados, que podem restringir quais dados estão disponíveis para serem usados nos relatórios. Ao usar campos dinâmicos de atividades para adicionar dados principais à linha de assunto, você pode reduzir o número de campos de atividade personalizados que precisam ser criados na instância do Salesforce.
* O campo de assunto de atividades e tarefas seguirá um padrão consistente definido pelo Administrador de Ações de insight de vendas.

>[!NOTE]
>
>Se você estiver registrando respostas de email como atividades para o Salesforce, elas não usarão as configurações de Personalização de detalhes da atividade do Salesforce . Em vez disso, serão registradas como &quot;Responder: Assunto do email.&quot;

## Campos dinâmicos da atividade compatíveis {#activity-dynamic-fields-supported}

Campos dinâmicos da atividade fazem referência a informações sobre suas atividades de vendas para preencher dados. Hoje, eles podem ser usados com a Personalização de detalhes da atividade do Salesforce.

>[!NOTE]
>
>Se não houver valor para preencher o campo dinâmico de uma atividade/tarefa específica, ele não preencherá nenhum dado para esse campo dinâmico quando o Campo Tarefa - Assunto do Salesforce for atualizado.

<table>
 <tr>
  <th>Campo</th>
  <th>Descrição</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>Preenche o tipo de tarefa como Email, Chamada, InMail ou Personalizado.</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>Preenche o assunto da tarefa.</p>
      <p>No caso de um email, ele preencherá a linha de assunto do email.</p>
      <p>No caso de chamada, inMail ou custom, ele preencherá um valor se houver uma tarefa de lembrete criada com um valor no campo nome/assunto da tarefa.</p></td>
 </tr>
 <tr>
  <td>{{sales_campaign_name}}</td>
  <td>Se a atividade foi iniciada a partir de uma campanha de vendas, ela preencherá o nome da campanha de vendas.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_day}}</td>
  <td>Se a atividade foi iniciada a partir de uma campanha de vendas, ela preencherá o número do dia da campanha de vendas em que essa atividade ocorreu.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_step}}</td>
  <td>Se a atividade foi iniciada a partir de uma campanha de vendas, ela preencherá o número da etapa no dia da campanha de vendas em que a atividade ocorreu.</td>
 </tr>
 <tr>
  <td>{{call_result}}</td>
  <td>Se a atividade for uma chamada e o resultado da chamada for selecionado, o valor do resultado da chamada será preenchido.</td>
 </tr>
 <tr>
  <td>{{call_reason}</td>
  <td>Se a atividade for uma chamada e o motivo da chamada for selecionado, o valor do motivo da chamada será preenchido.</td>
 </tr>
</table>

## Configuração da Personalização de Detalhes da Atividade do Salesforce {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**Permissões de administrador necessárias.**

Ao configurar os detalhes da atividade, considere quais dados seriam mais relevantes para as vendas ao revisar o histórico de tarefas no Salesforce.

1. Clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. Clique em **Salesforce**.

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. Clique em **Sincronizar configurações**.

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. No editor de Personalização de detalhes da atividade , adicione o texto livre desejado. O texto adicionado não é dinâmico e permanecerá inalterado para o campo de assunto de todas as tarefas sincronizadas com o Salesforce.

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >Embora não seja obrigatório, quebrar o texto adicionado entre colchetes pode facilitar a discernimento de algumas pessoas quando os dados são preenchidos com um campo de assunto no Salesforce. Exemplo: `[Sales Insight Actions] - {{Activity_type}}`

1. Adicione outros campos dinâmicos que desejar clicando no botão **Adicionar campo dinâmico** botão.

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. Selecione os campos dinâmicos desejados.

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. Clique em **Salvar**.

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>O Salesforce impõe um limite de 255 caracteres. Se os detalhes da atividade excederem isso, eles serão truncados para garantir que as informações sejam armazenadas no campo de assunto do Salesforce .

>[!MORELIKETHIS]
>
>* [Configurações de sincronização](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Sincronização de Tarefa de Lembrete com o Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)

