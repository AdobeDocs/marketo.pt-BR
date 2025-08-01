---
description: Configurar A Personalização Dos Detalhes Da Atividade Do Salesforce - Documentação Do Marketo - Documentação Do Produto
title: Configurar a personalização dos detalhes da atividade do Salesforce
exl-id: 534ebdb5-7a5b-48eb-98f7-2d05a9eae8e8
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 1%

---

# Configurar a personalização dos detalhes da atividade [!DNL Salesforce] {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* As Ações [do Salesforce e do Sales Insight devem estar conectadas](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md)
>* A atividade de email de log via API [deve ser habilitada](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)

A Personalização dos detalhes da atividade permite que administradores configurem as informações que farão logon no [!DNL Salesforce] Campo de Tarefa - Assunto, quando uma atividade/tarefa de lembrete [!DNL Sales Insight Actions] é sincronizada com [!DNL Salesforce].

>[!NOTE]
>
>* As atualizações feitas no campo de assunto em [!DNL Sales Insight Actions] de uma tarefa de lembrete serão refletidas no campo de assunto da tarefa [!DNL Salesforce] correspondente, se você estiver usando o campo dinâmico `{{activity_subject}}` na Personalização dos Detalhes da atividade.
>* Não há suporte para quebras de linha ao registrar informações no campo de assunto [!DNL Salesforce]. Quaisquer quebras de linha no editor de Personalização de Detalhes da Atividade serão removidas quando um assunto da tarefa de vendas for atualizado.

![](assets/configure-salesforce-activity-detail-customization-1.png)

![](assets/configure-salesforce-activity-detail-customization-2.png)

<table>
 <tr>
  <td><strong>1</td>
  <td>Tarefa de lembrete do InMail</td>
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
* Os administradores podem marcar o campo de assunto com um identificador exclusivo, como &quot;Mkto_sales&quot;, para que as atividades de Ações do Sales Insight possam ser facilmente identificadas e diferenciadas de outras atividades de email, atividades de chamada e tarefas.
* Reduza a necessidade de campos de atividade personalizados. O Salesforce impõe limites ao número de campos de atividade personalizados, que podem restringir quais dados estão disponíveis para serem usados em relatórios. Ao usar campos dinâmicos de atividade para adicionar dados principais à linha de assunto, é possível reduzir o número de campos de atividade personalizados que precisam ser criados em sua instância do Salesforce.
* O campo de assunto das atividades e tarefas seguirá um padrão consistente definido pelo Administrador de Ações do Sales Insight.

>[!NOTE]
>
>Se você estiver registrando respostas de email como atividades do [!DNL Salesforce], elas não usarão as configurações de Personalização de Detalhes da Atividade [!DNL Salesforce]. Em vez disso, eles serão registrados como &quot;Responder: Assunto do email&quot;.

## Campos Dinâmicos De Atividade Compatíveis {#activity-dynamic-fields-supported}

Campos Dinâmicos da Atividade fazem referência a informações sobre suas atividades de vendas para preencher dados. Hoje, eles podem ser usados com a Personalização dos Detalhes da atividade do [!DNL Salesforce].

>[!NOTE]
>
>Se não houver um valor para preencher o campo dinâmico de uma atividade/tarefa específica, ele não preencherá nenhum dado desse campo dinâmico quando o Campo Tarefa - Assunto do Salesforce for atualizado.

<table>
 <tr>
  <th>Campo</th>
  <th>Descrição</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>Preencherá o tipo de tarefa como Email, Chamada, InMail ou Personalizado.</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>Preencherá o assunto da tarefa.</p>
      <p>No caso de um email, ele preencherá a linha de assunto do email.</p>
      <p>No caso de chamada, inMail ou personalizado, ele preencherá um valor se houver uma tarefa de lembrete criada com um valor no campo de nome/assunto da tarefa.</p></td>
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
  <td>Se a atividade foi iniciada a partir de uma campanha de vendas, ela preencherá o número da etapa no dia da campanha de vendas em que essa atividade ocorreu.</td>
 </tr>
 <tr>
  <td>{{call_outcome}}</td>
  <td>Se a atividade for uma chamada e um resultado da chamada for selecionado, o valor do resultado da chamada será preenchido.</td>
 </tr>
 <tr>
  <td>{{call_reason}}</td>
  <td>Se a atividade for uma chamada e um motivo de chamada for selecionado, isso preencherá o valor do motivo da chamada.</td>
 </tr>
</table>

## Configurando a Personalização dos Detalhes da Atividade [!DNL Salesforce] {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**Permissões de administrador necessárias.**

Ao configurar os detalhes da atividade, considere quais dados seriam mais relevantes para as vendas ao revisar o histórico da tarefa em [!DNL Salesforce].

1. Clique no ícone de engrenagem e selecione **[!UICONTROL Configurações]**.

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. Clique em **[!UICONTROL Salesforce]**.

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. Clique em **[!UICONTROL Configurações de sincronização]**.

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. No editor de Personalização de detalhes da atividade, adicione o texto livre desejado. O texto que você adicionar não é dinâmico e permanecerá inalterado para o campo de assunto de todas as tarefas sincronizadas com [!DNL Salesforce].

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >Embora não seja obrigatório, quebrar o texto adicionado em colchetes pode facilitar para algumas pessoas discernir entre os dados quando eles são preenchidos em um campo de assunto em [!DNL Salesforce]. Exemplo: `[Sales Insight Actions] - {{Activity_type}}`

1. Adicione outros campos dinâmicos desejados clicando no botão **[!UICONTROL Adicionar Campo Dinâmico]**.

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. Selecione os campos dinâmicos desejados.

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>[!DNL Salesforce] impõe um limite de 255 caracteres. Se os detalhes da atividade excederem esse limite, eles serão truncados para garantir que as informações sejam armazenadas no campo de assunto [!DNL Salesforce].

>[!MORELIKETHIS]
>
>* [Sincronizar Atividades de Vendas com o Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)
>* [Sincronização de Tarefas de Lembrete com o Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
