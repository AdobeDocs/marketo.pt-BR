---
unique-page-id: 14352541
description: Sincronizando as tarefas do Sales Connect com o Salesforce pela primeira vez - Documentação do Marketo - Documentação do produto
title: Sincronizando pela primeira vez as tarefas do Sales Connect com o Salesforce
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Sincronizando pela primeira vez as tarefas do Sales Connect com o Salesforce {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Quando você ativa a sincronização entre as tarefas do Sales Connect e do Salesforce pela primeira vez, importamos suas tarefas do Salesforce. Nós **não** transferiremos quaisquer tarefas atuais que você tenha no Sales Connect para o Salesforce. Para reduzir a desordem e as duplicatas, as únicas tarefas que são sincronizadas do Sales Connect no Salesforce são as tarefas criadas *depois* de você sincronizar o Sales Connect com o SFDC.

Veja o que acontece quando você sincroniza tarefas do Sales Connect e do SFDC:

- Assim que você clicar em salvar na sincronização de tarefas, elas começarão a sincronizar. Isso levará algum tempo inicialmente.

- Qualquer lembrete que tenha sido atualizado ou criado nas últimas 24 horas será enviado do SFDC para o Sales Connect. A sincronização é baseada na data de conclusão e todas essas tarefas serão sincronizadas no back-end, mas no Command Center, você só verá tarefas com data de conclusão para hoje e amanhã.

- Se a sincronização tiver sido ativada anteriormente e você excluir qualquer tarefa no SFDC, qualquer item que tiver sido excluído nos últimos 15 dias será excluído do Centro de comando.

- Sincronizaremos constantemente as tarefas entre o Sales Connect e o SFDC enquanto a sincronização estiver habilitada.

Após a sincronização inicial, todas as tarefas que você criar, editar, concluir ou excluir no Sales Connect serão sincronizadas com sua lista de tarefas no Salesforce. Qualquer ação criada, editada, concluída ou excluída no Salesforce atualizará sua lista de tarefas no Sales Connect.

Para ativar esta sincronização, marque a caixa de sincronização na [página Configurações](https://toutapp.com/login) do aplicativo Web.
