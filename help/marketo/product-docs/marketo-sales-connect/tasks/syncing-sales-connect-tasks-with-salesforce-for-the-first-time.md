---
unique-page-id: 14352541
description: Sincronização das Tarefas do Sales Connect com o Salesforce pela primeira vez - Documentos do Marketing - Documentação do produto
title: Sincronização de Tarefas do Sales Connect com o Salesforce pela primeira vez
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# Sincronização de Tarefas do Sales Connect com o Salesforce pela primeira vez {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Quando você ativa a sincronização entre o Sales Connect e o Salesforce tarefa pela primeira vez, importamos suas tarefas do Salesforce. Nós **não** enviaremos nenhuma tarefa atual que você tenha no Sales Connect para o Salesforce. Para reduzir a confusão e os duplicados, as únicas tarefas que são sincronizadas do Sales Connect no Salesforce são as tarefas criadas *após* a sincronização do Sales Connect com o SFDC.

Veja o que acontece quando você sincroniza o Sales Connect e as tarefas SFDC:

- Assim que você clicar em Salvar na sincronização do tarefa, eles começarão a sincronizar. Isso levará algum tempo inicialmente.

- Todos os lembretes que foram atualizados ou criados no `last 24 hours` serão enviados do SFDC para o Sales Connect. A sincronização é baseada em `due date` e todas essas tarefas serão sincronizadas no back-end, mas no Command Center, você só verá tarefas vencidas hoje e amanhã.

- Se a sincronização tiver sido ativada anteriormente e você excluir qualquer tarefa no SFDC, tudo o que tiver sido excluído nos últimos 15 dias será excluído do Centro de Comando.

- Sempre sincronizaremos tarefas entre o Sales Connect e o SFDC, contanto que a sincronização esteja ativada.

Após a sincronização inicial, quaisquer tarefas que você criar, editar, concluir ou excluir no Sales Connect serão sincronizadas com sua lista do tarefa no Salesforce. E qualquer item criado, editado, concluído ou excluído no Salesforce atualizará sua lista do tarefa no Sales Connect.

Para ativar essa sincronização, marque a caixa de sincronização na página [](http://toutapp.com/next#settings/crm/salesforce/configure) Configurações no aplicativo da Web.

