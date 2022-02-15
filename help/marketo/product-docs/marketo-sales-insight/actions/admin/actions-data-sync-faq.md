---
description: Perguntas frequentes sobre sincronização de dados de ações - Documentação do Marketo - Documentação do produto
title: Perguntas frequentes sobre a sincronização de dados de ações
hide: true
hidefromtoc: true
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 441482ea4d367d6d751c4dd5b8bcd67f7fb7935a
workflow-type: tm+mt
source-wordcount: '1045'
ht-degree: 2%

---

# Perguntas frequentes sobre a sincronização de dados de ações {#actions-data-sync-faq}

A sincronização de campo de unificação de dados para Ações de Insight de Vendas permite que o sistema extraia informações de pessoas do banco de dados do Marketo Engage para o banco de dados Ações de Insight de Vendas .

Isso fornece dados de pessoas atualizados no aplicativo web Ações de insight de vendas e permite que o sistema colete IDs exclusivas para registros de pessoas correspondentes no Marketo e registros de cliente/contato/conta/oportunidade no Salesforce, para que os registros possam ser referenciados corretamente para dados de registro.

Essa sincronização pode ser ativada na guia Configuração de ações de insight de vendas na seção Admin do Marketo Engage. Para obter mais informações, consulte [Iniciar Sincronização de Dados](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/msi-actions-admin-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

O diagrama acima mostra como os dados da atividade e da tarefa das pessoas podem sincronizar entre os sistemas. Algumas observações:

* Os registros de pessoas são sincronizados com as Ações de insight de vendas do Marketo Engage, tornando o Marketo Engage na fonte de verdade para os dados de pessoas das Ações de insight de vendas
* Ações de insight de vendas e Marketo Engage [dispor de um mecanismo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) para coletar e sincronizar o status de cancelamento de subscrição no Salesforce
* O status de cancelamento de inscrição não é sincronizado entre Ações de vendas e Marketo Engage, mas as Ações de insight de vendas podem ser configuradas para verificar o status de cancelamento de assinatura do Marketo das pessoas antes de permitir que os vendedores enviem um email com [Verificação de cancelamento de assinatura do Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

Abaixo estão algumas perguntas frequentes relacionadas ao funcionamento da sincronização de unificação de dados.

## Quais leads/contatos são sincronizados com ações de insight de vendas? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

Os clientes potenciais e os contatos que têm um proprietário de vendas atribuído a eles serão sincronizados em Ações de vendas.

Você pode ver se um cliente potencial/contato tem um proprietário de vendas no Salesforce observando o campo proprietário padrão que existe.

O proprietário de vendas não precisa ser o usuário de sincronização da Marketo ou qualquer usuário específico do Salesforce ou de vendas. Tudo o que precisamos é que haja um usuário listado no campo proprietário do cliente potencial e proprietário do contato listado no Salesforce, para que possamos identificá-lo como um cliente potencial de vendas e sincronizá-lo nas Ações de informações de vendas. Todas as atualizações nos campos que sincronizamos também serão detectadas e atualizadas em Ações de insight de vendas.

## De onde vêm os dados da atividade exibidos na Grade Inteligente de Insight de Vendas? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

Os dados da atividade, como email, chamada, momento interessante e Web, são todos provenientes do banco de dados do Marketo Engage. O Sales Insight Smart Grid faz uma solicitação para a instância do Marketo Engage para recuperá-la sempre que um usuário de vendas carregar o painel Sales Insight .

![](assets/actions-data-sync-faq-4.png)

Para garantir que todos os dados da atividade possam ser provenientes do Marketo Engage, as Ações de insight de vendas sincronizam todos os dados da atividade com o Marketo Engage.

## Quais campos relacionados ao registro de pessoas são sincronizados de Marketo Engage para Ações de insight de vendas? {#what-fields-sync}

Há 11 campos que são sincronizados de Marketo Engage para Ações de insight de vendas:

* Nome
* Sobrenome
* ID de contato do Salesforce
* ID de cliente do Salesforce
* ID do Marketo
* Empresa
* Título
* E-mail
* Número de telefone
* URL do Linkedin
* Fonte

## Os campos que sincronizam entre o Marketo Engage e as Ações de insight de vendas são configuráveis? {#are-the-fields-that-sync-configurable}

Configurar quais campos de Marketo Engage sincronizam com Ações de Insight de Vendas não está disponível, nem a capacidade de mapear campos. A sincronização do Marketo mapeia automaticamente campos padrão do Marketo para campos padrão na sua instância de Ação de vendas.

## Por que as ações de insight de vendas têm seu próprio banco de dados? {#why-does-actions-have-its-own-database}

As Ações de insight de vendas têm seu próprio aplicativo da Web com um banco de dados dedicado de pessoas e atividades para fornecer um espaço de trabalho otimizado que seja criado e projetado para equipes de vendas. Isso permite que os gerentes e vendedores de vendas tenham um espaço para criar e gerenciar sua estratégia de engajamento sem conceder acesso ou privilégios ao espaço de trabalho do Marketo Engage principal, que é otimizado para especialistas em operações de marketing.

## Como as duplicatas são tratadas? {#how-are-duplicates-handled}

Seu banco de dados de Ações de vendas será uma cópia das pessoas qualificadas (leads/contatos com um proprietário de vendas) que existem no banco de dados do Marketo Engage. Isso significa que, se houver dois registros com o mesmo endereço de email criado no Marketo, haverá um registro duplicado criado em Ações de vendas.

## Quanto tempo leva para a sincronização inicial ser concluída? {#how-long-initial-sync}

O processo inicial para sincronizar todos os dados de clientes potenciais de vendas em uma nova instância de Ações de insight de vendas normalmente processará pessoas em cerca de 1.000 a cada 1-2 minutos. Esta é apenas uma estimativa e pode variar.

Quando a sincronização inicial ocorrer e todos os seus leads de vendas tiverem sido preenchidos na instância do aplicativo Web Ações de informações de vendas, haverá uma sincronização incremental que será executada sempre que houver uma atualização para um dos campos compatíveis que estiverem sincronizados.

## Os usuários de Ações de insight de vendas podem editar dados de pessoas no aplicativo Web Ações? {#can-actions-users-edit-people-data}

Não, a capacidade de criar e editar registros de pessoas em Ações não está disponível para usuários e administradores do aplicativo Web Ações. Criar e editar pessoas deve ser feito no Salesforce ou no Marketo Engage. As Ações de insight de vendas usam o Marketo como fonte de verdade para dados de pessoas sincronizando continuamente novos dados, de modo que, se uma pessoa for atualizada ou criada no Marketo a partir de um fluxo de trabalho no Marketo ou sincronizada do Salesforce, essas atualizações serão passadas para o banco de dados do aplicativo web Ações de insight de vendas .

## As atividades de vendas registram na Marketo? {#do-sales-activities-log-to-marketo}

Sim, as atividades de envolvimento de vendas farão logon no Marketo como atividades nativas. Essas atividades também incluem filtros nativos que podem ser usados com restrições para direcionar leads com base em atributos de atividade de vendas.

![](assets/actions-data-sync-faq-5.png)

Abaixo está uma lista das atividades que fazem logon no Marketo:

* Enviar e-mail de vendas
* Abrir e-mail de vendas
* Clicar em e-mail de vendas
* Respondido para Email de Vendas
* E-mail de vendas foi devolvido
* Chamada de Vendas Recebida
* Adicionar a campanha de vendas
* Removido da Campanha de Vendas

## As atividades de vendas registram-se no Salesforce? {#do-sales-activities-log-to-salesforce}

Sim, as atividades de envolvimento de vendas farão logon no Salesforce como tarefas nativas. Essas tarefas podem ser usadas nos relatórios do Salesforce para potencializar painéis de equipes que rastreiam as atividades de vendas.

As Ações de insight de vendas permitem que os administradores configurem quais atividades de vendas são registradas no Salesforce. Essas atividades incluem emails, chamadas e tarefas de lembrete de abertura.

![](assets/actions-data-sync-faq-6.png)

O diagrama acima mostra quais informações são registradas no Salesforce. Atividades como emails e chamadas são registradas no Salesforce em uma [sincronização unidirecional](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md). [Cancelamentos de assinatura](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) e [Tarefas de Lembrete](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) são atualizadas com uma sincronização bidirecional. Cada uma dessas sincronizações de dados é configurável na interface do aplicativo Web Ações do Sales Insight .

>[!MORELIKETHIS]
>
>* [Sincronização de cancelamentos de assinatura com o Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Verificação de cancelamentos de inscrições no Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [Configurações de sincronização do Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Sincronização de Tarefa de Lembrete com o Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Iniciar Sincronização de Dados](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/msi-actions-admin-guide.md#initiate-data-sync)

