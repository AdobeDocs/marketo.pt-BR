---
description: Por que minhas atividades de vendas e meus campos de atividade não estão sendo sincronizados com o Salesforce? - Documentação do Marketo - Documentação do produto
title: Por que minhas atividades de vendas e meus campos de atividade não estão sendo sincronizados com o Salesforce?
exl-id: 5da855f2-18c6-456a-9e5d-ef4499596b3c
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Por que minhas atividades de vendas e meus campos de atividade não estão sendo sincronizados com o Salesforce? {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Não vejo atividades de email ou de chamada sincronizadas com o Salesforce.**

* Verifique se você está conectado ao Salesforce. Cada usuário precisará ter uma conexão para registrar seu email e chamadas para o Salesforce.
* Verifique se você configurou as [Configurações de Sincronização do Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* Os emails farão uma pesquisa de registro com base na Salesforce ID como a pesquisa primária e o endereço de email como o secundário. Você pode confirmar que um registro de pessoa tem uma Salesforce ID e um endereço de email vinculados a ela no [aplicativo Web Ações](https://toutapp.com/next#command_center){target="_blank"}.
* As chamadas farão uma pesquisa de registro somente com base na Salesforce ID. Se nenhuma Salesforce ID existir no registro de pessoa em Ações, a chamada não será registrada. Você pode confirmar que um registro de pessoa tem uma Salesforce ID vinculada a ela no [aplicativo Web Ações](https://toutapp.com/next#command_center){target="_blank"}.

**Não estou vendo campos de atividade na atualização do Salesforce.**

Se você não estiver vendo a atualização dos [campos do atributo de atividade](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} do email no Salesforce, talvez seja devido a restrições na Acessibilidade de Campo da sua equipe. A segurança em nível de campo do Salesforce oferece aos administradores do Salesforce a capacidade de colocar restrições em relação a quais informações podem ser visualizadas e editadas pelos usuários. Se os usuários de Ações não tiverem acesso para visualizar e editar esses campos, a sincronização de atividades das Ações não atualizará esses campos.

* Peça ao administrador do Salesforce para garantir que essas configurações de segurança não interfiram nos [campos de Ações e Atividade do Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* Se você for um administrador do Salesforce, poderá ver sua Acessibilidade de campo na guia Controles de segurança. Os principais objetos com os quais as ações interagirão são: Clientes potenciais, Contatos, Contas, Oportunidades e Tarefa/Atividades.

>[!NOTE]
>
>Os campos associados aos objetos de cliente potencial, contato, conta e oportunidade serão instalados com o pacote Sales Insight Salesforce. Os campos associados ao [tipo de registro de Tarefa/Atividade precisarão ser criados](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} por um Administrador do Salesforce.
