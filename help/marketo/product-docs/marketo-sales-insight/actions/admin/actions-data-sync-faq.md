---
description: Perguntas frequentes sobre a sincronização de dados de ações - Documentação do Marketo - Documentação do produto
title: Perguntas frequentes sobre a Sincronização de Dados de Ações
feature: Sales Insight Actions
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 26173379c89393596b3ece18c7f7e945a79588d9
workflow-type: tm+mt
source-wordcount: '1054'
ht-degree: 3%

---

# Perguntas frequentes sobre a Sincronização de Dados de Ações {#actions-data-sync-faq}

A sincronização de campo de unificação de dados para Ações do Sales Insight permite que o sistema extraia informações de pessoas do banco de dados do Marketo Engage para o banco de dados de Ações do Sales Insight.

Isso fornece dados de pessoas atualizados no aplicativo Web de ações do Sales Insight e permite que o sistema colete IDs exclusivas para registros de pessoas correspondentes no Marketo e registros de cliente potencial/contato/conta/oportunidade no Salesforce, para que os registros possam ser referenciados corretamente para dados de log.

Essa sincronização pode ser ativada na guia Configuração das ações do Sales Insight, na seção de Administrador do Marketo Engage. Para obter mais informações, confira [Iniciar Sincronização de Dados](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

O diagrama acima mostra como os dados de atividades e tarefas das pessoas podem ser sincronizados entre sistemas. Algumas observações:

* Os registros de pessoas são sincronizados com as Ações de insight de vendas do Marketo Engage, tornando o Marketo Engage a fonte da verdade para os dados de pessoas das Ações de insight de vendas
* As ações do Marketo Engage e do Sales Insight [têm um mecanismo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) para coletar e sincronizar o status de cancelamento de inscrição no Salesforce
* O status de cancelamento de inscrição não é sincronizado das Ações de vendas para o Marketo Engage, mas as Ações de insight de vendas podem ser configuradas para verificar o status de cancelamento de inscrição de pessoas no Marketo antes de permitir que os vendedores enviem um email com [Verificação de cancelamento de inscrição do Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

Abaixo estão algumas perguntas frequentes relacionadas ao funcionamento da sincronização de unificação de dados.

## Quais clientes potenciais/contatos são sincronizados com as ações do Sales Insight? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

Clientes potenciais e contatos que tiverem um proprietário de vendas atribuído a eles serão sincronizados em Ações de Vendas.

Você pode ver se um cliente potencial/contato tem um proprietário de vendas no Salesforce observando o campo proprietário padrão existente.

O proprietário das vendas não precisa ser o usuário de sincronização do Marketo ou qualquer usuário de vendas ou Salesforce específico. Tudo o que precisamos é que haja um usuário listado no campo de proprietário do cliente potencial e proprietário do contato listado no Salesforce, para que possamos identificá-lo como um cliente potencial de vendas e sincronizá-lo nas Ações do Sales Insight. Quaisquer atualizações nos campos que sincronizamos também serão detectadas e atualizadas em Ações do Sales Insight.

## De onde os dados da atividade exibidos na Grade inteligente do Sales Insight são obtidos? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

Os dados de atividade, como email, chamada, momento interessante e web, são todos provenientes do banco de dados de Marketo Engage. A Grade inteligente do Sales Insight faz uma solicitação à instância do Marketo Engage para recuperar isso sempre que um usuário de vendas carregar o painel Sales Insight.

![](assets/actions-data-sync-faq-4.png)

Para garantir que todos os dados da atividade possam ser obtidos do Marketo Engage, as Ações do Sales Insight sincronizam todos os dados da atividade no Marketo Engage.

## Quais campos relacionados a registros de pessoas são sincronizados do Marketo Engage para Ações de insights de vendas? {#what-fields-sync}

Há 11 campos que são sincronizados do Marketo Engage para as Ações do Sales Insight:

* Nome
* Sobrenome
* ID de contato do Salesforce
* ID do cliente em potencial do Salesforce
* ID da conta do Salesforce
* ID da oportunidade do Salesforce
* ID do Marketo
* Empresa
* Título
* Email
* Número de telefone
* URL do Linkedin
* Origem

## Os campos que sincronizam entre o Marketo Engage e as ações do Sales Insight podem ser configurados? {#are-the-fields-that-sync-configurable}

Configurar quais campos de Marketo Engage sincronizar com Ações de insights de vendas não está disponível, nem a capacidade de mapear campos. A sincronização do Marketo mapeia automaticamente campos padrão do Marketo para campos padrão na instância de Ação de vendas.

## Por que as ações de Insight de vendas têm seu próprio banco de dados? {#why-does-actions-have-its-own-database}

As Ações de insights de vendas têm seu próprio aplicativo web com um banco de dados dedicado de pessoas e atividades para fornecer um espaço de trabalho otimizado que é criado e projetado para equipes de vendas. Isso permite que gerentes e vendedores tenham um espaço para desenvolver e gerenciar sua estratégia de engajamento   sem conceder acesso ou privilégios ao espaço de trabalho principal do Marketo Engage, que é otimizado para especialistas em operações de marketing.

## Como as duplicatas são tratadas? {#how-are-duplicates-handled}

Seu banco de dados de Ações de vendas será uma cópia das pessoas qualificadas (clientes potenciais/contatos com um proprietário de vendas) existentes no banco de dados do Marketo Engage. Isso significa que, se houver dois registros com o mesmo endereço de email criado no Marketo, haverá um registro duplicado criado nas Ações de vendas.

## Quanto tempo leva para a sincronização inicial ser concluída? {#how-long-initial-sync}

O processo inicial para sincronizar todos os dados de clientes potenciais de vendas em uma nova instância de Ações do Sales Insight normalmente processará pessoas em cerca de 1.000 a cada 1-2 minutos. Isso é apenas uma estimativa e pode variar.

Quando a sincronização inicial ocorrer e todos os leads de vendas tiverem sido preenchidos na instância do aplicativo da Web Ações de insights de vendas, haverá uma sincronização incremental que será executada sempre que houver uma atualização de um dos campos compatíveis que estão sincronizados.

## Os usuários das Ações de insight de vendas podem editar dados de pessoas no aplicativo Web Ações? {#can-actions-users-edit-people-data}

Não, a capacidade de criar e editar registros de pessoas em Ações não está disponível para usuários e administradores do aplicativo Web Ações. Criar e editar pessoas deve ser feito no Salesforce ou Marketo Engage. As Ações do Sales Insight usam o Marketo como fonte da verdade para dados de pessoas, sincronizando continuamente novos dados; portanto, se uma pessoa for atualizada ou criada no Marketo a partir de um fluxo de trabalho no Marketo ou sincronizada a partir do Salesforce, essas atualizações serão passadas para o banco de dados do aplicativo Web de Ações do Sales Insight.

## As atividades de vendas registram no Marketo? {#do-sales-activities-log-to-marketo}

Sim, as atividades do contrato de vendas serão registradas no Marketo como atividades nativas. Essas atividades também incluem filtros nativos que podem ser usados com restrições para direcionar leads com base nos atributos da atividade de vendas.

![](assets/actions-data-sync-faq-5.png)

Veja abaixo uma lista das atividades que fazem logon no Marketo:

* Enviar e-mail de vendas
* Abrir e-mail de vendas
* Clicar em e-mail de vendas
* Respondeu ao e-mail de vendas
* E-mail de vendas foi devolvido
* Chamada de vendas recebida
* Adicionar a campanha de vendas
* Removido da campanha de vendas

## As atividades de vendas registram no Salesforce? {#do-sales-activities-log-to-salesforce}

Sim, as atividades do contrato de vendas serão registradas no Salesforce como tarefas nativas. Essas tarefas podem ser usadas nos relatórios do Salesforce para acionar painéis de equipe que rastreiam as atividades de vendas.

As Ações de insight de vendas permitem que os administradores configurem quais atividades de vendas estão registradas no Salesforce. Essas atividades incluem emails, chamadas e tarefas de lembrete de abertura.

![](assets/actions-data-sync-faq-6.png)

O diagrama acima mostra quais informações estão registradas no Salesforce. Atividades como emails e chamadas são registradas no Salesforce em uma [sincronização unidirecional](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md). [Cancelamentos de assinatura](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) e [Tarefas de Lembrete](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) são mantidos atualizados com uma sincronização bidirecional. Cada uma dessas sincronizações de dados pode ser configurada na interface do aplicativo Web de Ações do Sales Insight.

>[!MORELIKETHIS]
>
>* [Sincronizando cancelamentos de assinatura com Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Verificação de Cancelamento de Inscrição do Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [Configurações de sincronização do Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Sincronização de tarefas de lembrete com o Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Iniciar Sincronização de Dados](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)

