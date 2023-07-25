---
description: Como corrijo "Não foi possível autenticar sua solicitação" ao me conectar ao Salesforce - Documentação do Marketo - Documentação do produto
title: Como corrijo "Não foi possível autenticar sua solicitação" ao me conectar ao Salesforce
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Como corrijo &quot;Não foi possível autenticar sua solicitação&quot; ao me conectar ao Salesforce {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Se você receber a mensagem de erro &quot;Não foi possível autenticar sua solicitação&quot; ao tentar conectar as ações do Sales Insight ao Salesforce, poderá haver uma restrição no seu acesso à API do Salesforce. Consulte o administrador do Salesforce para verificar se os itens a seguir estão em vigor.

## Habilitar API em Permissões do usuário {#enable-api-in-user-permissions}

1. Peça a um administrador do Salesforce que faça logon no SFDC.
1. Selecionar **Configuração**.
1. Selecionar **Gerenciar usuários**.
1. Selecionar **Perfis**.
1. Localize o Perfil em que estão os usuários do ToutApp e clique em **Editar**.
1. Role para baixo até **Permissões administrativas** e verifique se **API habilitada** está marcado.

## Verifique se o Salesforce está bloqueando a conexão das ações do Sales Insight {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Peça a um administrador do Salesforce que faça logon no SFDC.
1. Selecionar **Configuração**.
1. Selecionar **Gerenciar aplicativos**.
1. Selecionar **Uso do OAuth de aplicativos conectados**.
1. Certifique-se de que as Ações do Sales Insight mostrem &quot;Bloquear&quot; ao lado dele. Se você vir &quot;Desbloquear&quot;, clique no botão para desbloquear o acesso das Ações do Sales Insight ao Salesforce.
