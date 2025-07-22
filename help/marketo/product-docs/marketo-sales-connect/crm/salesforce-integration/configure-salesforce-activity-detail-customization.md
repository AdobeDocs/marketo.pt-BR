---
description: Configurar A Personalização Dos Detalhes Da Atividade Do Salesforce - Documentação Do Marketo - Documentação Do Produto
title: Configurar a personalização dos detalhes da atividade do Salesforce
exl-id: 4b20ca29-18d6-4026-9bf9-77656ad1442d
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 1%

---

# Configurar a personalização dos detalhes da atividade [!DNL Salesforce] {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* [!DNL Salesforce] e [!DNL Marketo Sales Connect] [devem estar conectados](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md)
>* A atividade de email de log via API [deve ser habilitada](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)

A Personalização dos detalhes da atividade permite que os administradores configurem as informações que farão logon no campo Tarefa - Assunto da Salesforce, quando uma atividade/tarefa de lembrete do [!DNL Sales Connect] for sincronizada com o Salesforce.

>[!NOTE]
>
>* As atualizações feitas no campo de assunto em [!DNL Sales Connect] de uma tarefa de lembrete serão refletidas no campo de assunto da tarefa [!DNL Salesforce] correspondente, se você estiver usando o campo dinâmico `{{activity_subject}}` na Personalização dos Detalhes da atividade.
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
* Os administradores podem marcar o campo de assunto com um identificador exclusivo, como &quot;Mkto_sales&quot;, para que as atividades do Sales Connect possam ser facilmente identificadas e diferenciadas de outras atividades de email, atividades de chamada e tarefas.
* Reduza a necessidade de campos de atividade personalizados. O Salesforce impõe limites ao número de campos de atividade personalizados, que podem restringir quais dados estão disponíveis para serem usados em relatórios. Ao usar campos dinâmicos de atividade para adicionar dados principais à linha de assunto, é possível reduzir o número de campos de atividade personalizados que precisam ser criados em sua instância do Salesforce.
* O campo de assunto das atividades e tarefas seguirá um padrão consistente definido pelo Administrador do Sales Connect.

>[!NOTE]
>
>Se você estiver registrando respostas de email como atividades do [!DNL Salesforce], elas não usarão as configurações de Personalização de Detalhes da Atividade [!DNL Salesforce]. Em vez disso, eles serão registrados como &quot;Responder: Assunto do email&quot;.

## Campos Dinâmicos De Atividade Compatíveis {#activity-dynamic-fields-supported}

Campos Dinâmicos da Atividade fazem referência a informações sobre suas atividades de vendas para preencher dados. Hoje, eles podem ser usados com a Personalização dos Detalhes da atividade do [!DNL Salesforce].

>[!NOTE]
>
>Se não houver um valor para preencher o campo dinâmico para uma atividade/tarefa específica, ele não preencherá nenhum dado para esse campo dinâmico quando o Campo Tarefa - Assunto [!DNL Salesforce] for atualizado.

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

## Configuração da personalização de detalhes de atividades do Salesforce {#configuring-salesforce-activity-detail-customization}

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
   >Embora não seja obrigatório, quebrar o texto adicionado em colchetes pode facilitar para algumas pessoas discernir entre os dados quando eles são preenchidos em um campo de assunto no Salesforce. Exemplo: `[Sales Connect] - {{Activity_type}}`

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
>* [Configurações de sincronização](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Sincronização de Tarefa de Lembrete com [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-connect/tasks/reminder-task-sync-with-salesforce.md)
>* [[!DNL Sales Connect] Personalização do CRM](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md)
