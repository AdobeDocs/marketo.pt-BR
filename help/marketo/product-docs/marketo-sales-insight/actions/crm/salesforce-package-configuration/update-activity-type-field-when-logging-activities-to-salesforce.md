---
description: Campo Atualizar tipo de atividade ao registrar atividades no Salesforce - Documentação do Marketo - Documentação do produto
title: Atualizar campo de tipo de atividade ao registrar atividades no Salesforce
exl-id: 800323cb-2b99-42f1-ae30-0f87a9a1b4be
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 6%

---

# Atualizar campo de tipo de atividade ao registrar atividades no Salesforce {#update-activity-type-field-when-logging-activities-to-salesforce}

As ações podem sincronizar automaticamente suas atividades de email e chamada com o Salesforce, para serem usadas em relatórios e aumentar a visibilidade do histórico de atividades. Ao registrar atividades, verifique se o campo Tipo de atividade está atualizado corretamente para Email, Chamada ou Resposta, dependendo do tipo de atividade que está sendo registrada.

>[!NOTE]
>
>O registro de emails por CCO não olhará para a lista de opções Tipo de tarefa e preencherá automaticamente o campo de tipo como &quot;email&quot;, pois estão sendo entregues à Salesforce pelo endereço CCO.

## O que você deve saber {#things-to-know}

* É necessária uma conexão com o Salesforce para que o Tipo de tarefa seja atualizado.
* Não deve haver nenhum valor padrão de Tipo selecionado na lista de opções de Tipo de Tarefa.
* Chamada, Resposta e Email devem existir na lista de seleção Tipo de tarefa (questões de capitalização).
* Workflows ou Triggers na Salesforce que atualizam o campo Tipo de tarefa podem interferir nesse processo.

## Configuração {#setup}

Primeiro, verifique se você tem os valores corretos da lista de seleção em vigor. Você precisará da ajuda do administrador do Salesforce para fazer alterações na lista de opções.

Primeiro, verifique quais valores você está perdendo na Lista de opções de tipo de tarefa (sem Email, Chamada e Resposta). Talvez seja necessária a ajuda do administrador do Salesforce para revisar isso e fazer alterações na lista de opções do Tipo de atividade. Para fazer essas alterações, o administrador do Salesforce pode seguir as etapas abaixo.

### No Salesforce Lightning {#salesforce-lightning}

1. Navegue até [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Clique no ícone de engrenagem no canto superior direito e selecione **Configuração** > **Gerenciador de objetos**.
1. Digite &quot;tarefa&quot; na caixa &#39;Localização rápida&#39;.
1. No painel esquerdo, clique em **Campos e Relações**.
1. Clique no rótulo do campo **Tipo**.
1. Em Valor da Lista de Escolha de Tipo de Tarefa, clique em **Novo**.
1. Digite o nome dos valores da lista de opções do tipo de tarefa que estão ausentes (&quot;Email, &quot;Chamada&quot;, &quot;Resposta&quot;).
1. Clique em **Salvar**.

### No Salesforce Classic {#salesforce-classic}

1. Navegue até [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Clique em **Configuração** > **Compilação** > **Personalizar** > **Atividades** > **Campos de Tarefas**.
1. Clique em **Tipo**.
1. Em Valor da Lista de Escolha de Tipo de Tarefa, clique em **Novo**.
1. Digite o nome dos valores da lista de opções do tipo de tarefa que estão ausentes (&quot;Email, &quot;Chamada&quot;, &quot;Resposta&quot;).
1. Clique em **Salvar**.

Agora que isso está em vigor, você começará a ver o campo Type preenchendo o valor correspondente para Emails, Chamadas e Respostas registrados. Esses valores _não_ serão preenchidos nas tarefas de lembrete de Ações do Sales Insight.

>[!NOTE]
>
>Se você não vir &#39;Responder&#39; como um valor, adicione-o clicando em **Novo**. &quot;Responder&quot; não é um valor padrão no Salesforce.

>[!MORELIKETHIS]
>
>* [Registrando Atributos de Atividade de Vendas em Log no Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [Configurar a personalização dos detalhes da atividade do Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [Sincronizar Atividades de Vendas com o Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}
