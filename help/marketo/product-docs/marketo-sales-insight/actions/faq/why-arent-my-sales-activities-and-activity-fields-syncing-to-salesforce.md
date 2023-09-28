---
description: Por que minhas atividades de vendas e meus campos de atividade não estão sendo sincronizados com o Salesforce? - Documentação do Marketo - Documentação do produto
title: Por que minhas atividades de vendas e meus campos de atividade não estão sendo sincronizados com o Salesforce?
exl-id: 0836876d-1b89-4464-a841-81320a6e45fd
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Por que minhas atividades de vendas e meus campos de atividade não estão sendo sincronizados com o Salesforce? {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Não vejo atividades de email ou chamada sincronizadas com o Salesforce.**

* Verifique se você está conectado ao Salesforce. Cada usuário precisará ter uma conexão para registrar seu email e chamadas para o Salesforce.
* Verifique se você configurou o [Configurações de sincronização do Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* Os emails farão uma pesquisa de registro com base na ID do Salesforce como a pesquisa primária e o endereço de email como secundário. Você pode confirmar que um registro de pessoa tem uma ID do Salesforce e um endereço de email vinculados a ela na [Aplicativo Web de ações](https://toutapp.com/next#command_center){target="_blank"}.
* As chamadas farão uma pesquisa de registro somente com base na ID do Salesforce. Se não houver uma ID do Salesforce no registro pessoal em Ações, a chamada não será registrada. Você pode confirmar que um registro de pessoa tem uma ID do Salesforce vinculada a ela na [Aplicativo Web de ações](https://toutapp.com/next#command_center){target="_blank"}.

**Não estou vendo os campos de atividade na atualização do Salesforce.**

Se você não estiver vendo o email [campos de atributo de atividade](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} atualização no Salesforce, pode ser devido a restrições na Acessibilidade de campo da sua equipe. A segurança de nível de campo do Salesforce dá aos administradores do Salesforce a capacidade de colocar restrições em torno de quais informações podem ser visualizadas e editadas pelos usuários. Se os usuários de Ações não tiverem acesso para visualizar e editar esses campos, a sincronização de atividades das Ações não atualizará esses campos.

* Fale com o administrador do Salesforce para garantir que essas configurações de segurança não interfiram no [Ações Campos de atividade do Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* Se você for um administrador do Salesforce, poderá ver sua Acessibilidade de campo na guia Controles de segurança. Os principais objetos com os quais as ações interagirão são: Clientes potenciais, Contatos, Contas, Oportunidades e Tarefa/Atividades.

>[!NOTE]
>
>Os campos associados aos objetos de cliente potencial, contato, conta e oportunidade serão instalados com o pacote Sales Insight Salesforce. Campos associados à [O tipo de registro de tarefa/atividade precisará ser criado](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} por um administrador do Salesforce.
