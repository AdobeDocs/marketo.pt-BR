---
unique-page-id: 14352541
description: Sincronização de tarefas do Sales Connect com o Salesforce pela primeira vez - Marketo Docs - Documentação do produto
title: Sincronizar pela primeira vez as tarefas do Sales Connect com o Salesforce
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 3%

---

# Sincronizando [!DNL Sales Connect] Tarefas com [!DNL Salesforce] pela primeira vez {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Quando você ativa a sincronização entre as tarefas do [!DNL Sales Connect] e do [!DNL Salesforce] pela primeira vez, nós importamos suas tarefas do [!DNL Salesforce]. Nós **não** transferiremos quaisquer tarefas atuais que você tenha em [!DNL Sales Connect] para [!DNL Salesforce]. Para reduzir a desordem e as duplicatas, as únicas tarefas que são sincronizadas de [!DNL Sales Connect] para [!DNL Salesforce] são tarefas criadas *depois* que você sincroniza [!DNL Sales Connect] com o SFDC.

Veja o que acontece quando você sincroniza tarefas do [!DNL Sales Connect] e do SFDC:

- Assim que você clicar em salvar na sincronização de tarefas, elas começarão a sincronizar. Isso levará algum tempo inicialmente.

- Todos os lembretes atualizados ou criados nas últimas 24 horas serão extraídos do SFDC para [!DNL Sales Connect]. A sincronização é baseada na data de conclusão e todas essas tarefas serão sincronizadas no back-end, mas no Command Center, você só verá tarefas com data de conclusão para hoje e amanhã.

- Se a sincronização tiver sido ativada anteriormente e você excluir qualquer tarefa no SFDC, qualquer item excluído nos últimos 15 dias será excluído do Centro de comando.

- Sincronizaremos constantemente as tarefas entre o [!DNL Sales Connect] e o SFDC enquanto a sincronização estiver habilitada.

Após a sincronização inicial, todas as tarefas que você criar, editar, concluir ou excluir no [!DNL Sales Connect] serão sincronizadas com a sua lista de tarefas no [!DNL Salesforce]. Qualquer ação criada, editada, concluída ou excluída no [!DNL Salesforce] atualizará sua lista de tarefas no [!DNL Sales Connect].

Para ativar esta sincronização, marque a caixa de sincronização na [página Configurações](https://toutapp.com/login) do aplicativo Web.
