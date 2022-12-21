---
unique-page-id: 14352541
description: Sincronização de tarefas de conexão de vendas com o Salesforce pela primeira vez - Documentos do Marketo - Documentação do produto
title: Sincronização de Tarefas de Conexão de Vendas com o Salesforce pela Primeira Vez
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Sincronização de Tarefas de Conexão de Vendas com o Salesforce pela Primeira Vez {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Quando você ativa a sincronização entre as tarefas do Sales Connect e do Salesforce pela primeira vez, importamos suas tarefas do Salesforce. Nós vamos **not** passe o mouse sobre qualquer tarefa atual que você tenha no Sales Connect para o Salesforce. Para reduzir a desordem e as duplicatas, as únicas tarefas sincronizadas do Sales Connect no Salesforce são tarefas criadas *after* sincronize o Sales Connect com o SFDC.

Veja o que acontece quando você sincroniza tarefas do Sales Connect e do SFDC:

- Assim que você clicar em salvar na sincronização de tarefas, eles começarão a sincronizar. Isso levará algum tempo inicialmente.

- Todos os lembretes que foram atualizados ou criados nas últimas 24 horas serão transferidos do SFDC para o Sales Connect. A sincronização é baseada na data de vencimento e todas essas tarefas serão sincronizadas no back-end, mas no Centro de comando, você só verá tarefas que vencem hoje e amanhã.

- Se a sincronização tiver sido ativada anteriormente e você excluir qualquer tarefa no SFDC, qualquer coisa que tenha sido excluída nos últimos 15 dias será excluída do Centro de Comando.

- Sincronizaremos tarefas constantemente entre o Sales Connect e o SFDC, desde que a sincronização esteja ativada.

Após a sincronização inicial, qualquer tarefa que você criar, editar, concluir ou excluir no Sales Connect será sincronizada com a lista de tarefas no Salesforce. E qualquer item criado, editado, concluído ou excluído no Salesforce atualizará sua lista de tarefas no Sales Connect.

Para ativar essa sincronização, basta marcar a caixa de sincronização em seu [Página Configurações](https://toutapp.com/login) na aplicação web.
