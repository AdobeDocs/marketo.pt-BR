---
description: Atualizar campo Tipo de atividade ao registrar atividades no Salesforce - Documentação do Marketo - Documentação do produto
title: Atualizar campo Tipo de atividade ao registrar atividades no Salesforce
source-git-commit: 46c48172a58cf6bd2e9772ef57510fd7d808adc2
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Atualizar campo Tipo de atividade ao registrar atividades no Salesforce {#update-activity-type-field-when-logging-activities-to-salesforce}

As ações podem sincronizar automaticamente suas atividades de email e chamada com o Salesforce a serem usadas para relatórios e aumentar a visibilidade do histórico de atividades. Ao registrar atividades, verifique se o campo Tipo de atividade está atualizado corretamente para Email, Chamada ou Resposta, dependendo do tipo de atividade que está sendo registrada.

>[!NOTE]
>
>O registro de emails via CCO não olhará para a lista de opções Tipo de tarefa e preencherá automaticamente o campo tipo como &quot;email&quot;, pois estão sendo entregues ao Salesforce pelo endereço CCO.

## O que você deve saber {#things-to-know}

* Uma conexão com o Salesforce é necessária para que o Tipo de tarefa seja atualizado.
* Não deve haver nenhum valor padrão de Tipo selecionado na lista de opções de Tipo de Tarefa.
* Chamada, Resposta e Email devem existir na lista de seleção Tipo de tarefa (questões de capitalização).
* Workflows ou Triggers no Salesforce que atualizam o campo Tipo de tarefa podem interferir nesse processo.

## Configuração {#setup}

Primeiro, verifique se você tem os valores corretos da lista de seleção em vigor. Você precisará da ajuda de seu administrador do Salesforce para fazer alterações na lista de opções.

Primeiro, verifique quais valores você está perdendo na Lista de opções de tipo de tarefa (sem Email, Chamada e Resposta). Você pode precisar da ajuda de seu administrador do Salesforce para revisar isso e fazer alterações na lista de opções do Tipo de atividade. Para fazer essas alterações, o administrador do Salesforce pode seguir as etapas abaixo.

### No Salesforce Lightning {#salesforce-lightning}

1. Navegue até [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Clique no ícone de engrenagem no canto superior direito e selecione **Configuração** > **Gerenciador de objetos**.
1. Digite &quot;tarefa&quot; na caixa &#39;Localização rápida&#39;.
1. No painel esquerdo, clique em **Campos e relacionamentos**.
1. Clique no rótulo do campo **Tipo**.
1. Em Tipo de Tarefa Valor da Lista de Escolha, clique em **Novo**.
1. Digite o nome dos valores da lista de opções do tipo de tarefa que estão ausentes (&quot;Email, &quot;Chamada&quot;, &quot;Resposta&quot;).
1. Clique em **Salvar**.

### No Salesforce Classic {#salesforce-classic}

1. Navegue até [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Clique em **Configuração** > **Build** > **Personalizar** > **Atividades** > **Campos de tarefa**.
1. Clique em **Tipo**.
1. Em Tipo de Tarefa Valor da Lista de Escolha, clique em **Novo**.
1. Digite o nome dos valores da lista de opções do tipo de tarefa que estão ausentes (&quot;Email, &quot;Chamada&quot;, &quot;Resposta&quot;).
1. Clique em **Salvar**.

Agora que isso está em vigor, você começará a ver o campo Type preenchendo o valor correspondente para Emails, Chamadas e Respostas registrados. Esses valores serão _não_ será preenchida nas tarefas de lembrete de Ações do Sales Insight.

>[!NOTE]
>
>Se você não vir &#39;Responder&#39; como um valor, adicione-o clicando em **Novo**. &quot;Resposta&quot; não é um valor padrão no Salesforce.

>[!MORELIKETHIS]
>
>* [Registrando Atributos de Atividade de Vendas no Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [Configurar a personalização dos detalhes de atividade do Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [Configurações de sincronização do Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md){target="_blank"}
