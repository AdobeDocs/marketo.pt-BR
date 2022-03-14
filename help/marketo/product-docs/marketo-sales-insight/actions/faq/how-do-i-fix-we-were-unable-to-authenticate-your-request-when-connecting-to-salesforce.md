---
description: Como Corrigir "Não Conseguimos Autenticar Sua Solicitação" Ao Conectar-Se Ao Salesforce - Documentos Marketo - Documentação Do Produto
title: Como Corrigir "Não Foi Possível Autenticar Sua Solicitação" Ao Conectar-Se Ao Salesforce
hide: true
hidefromtoc: true
source-git-commit: c398aff77e09f4a63db5d51af55178aa663ec98e
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Como Corrigir &quot;Não Foi Possível Autenticar Sua Solicitação&quot; Ao Conectar-Se Ao Salesforce {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Se você receber a mensagem de erro &quot;Não foi possível autenticar sua solicitação&quot; ao tentar conectar Ações do Sales Insight ao Salesforce, pode haver uma restrição no acesso à API do Salesforce. Verifique com seu administrador do Salesforce para garantir que os itens a seguir estejam em vigor.

## Habilitar API nas Permissões do usuário {#enable-api-in-user-permissions}

1. Faça logon de Administrador do Salesforce no SFDC.
1. Selecionar **Configuração**.
1. Selecionar **Gerenciar usuários**.
1. Selecionar **Perfis**.
1. Encontre o Perfil em que os usuários do ToutApp estão e clique em **Editar**.
1. Role para baixo até **Permissões administrativas** e **API habilitada** está marcada.

## Verifique se o Salesforce está bloqueando a conexão de ações de insight de vendas {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Faça logon de Administrador do Salesforce no SFDC.
1. Selecionar **Configuração**.
1. Selecionar **Gerenciar aplicativos**.
1. Selecionar **Uso de OAuth para aplicativos conectados**.
1. Certifique-se de que as Ações de insight de vendas mostram &quot;Bloco&quot; ao lado dele. Se você vir &quot;Desbloquear&quot;, clique no botão para desbloquear o acesso das Ações de insight de vendas ao Salesforce.
