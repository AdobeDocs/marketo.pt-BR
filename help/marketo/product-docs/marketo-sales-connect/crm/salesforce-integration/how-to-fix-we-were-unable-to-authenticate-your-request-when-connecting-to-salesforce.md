---
unique-page-id: 14352484
description: Como corrigir o erro "Não foi possível autenticar sua solicitação" ao conectar-se ao Salesforce - Marketo Docs - Documentação do produto
title: Como corrigir o erro "Não foi possível autenticar sua solicitação" ao se conectar ao Salesforce
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Como corrigir o erro &quot;Não foi possível autenticar sua solicitação&quot; ao se conectar ao Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Se você receber a mensagem de erro &quot;Não foi possível autenticar sua solicitação&quot; ao tentar conectar o Sales Connect ao Salesforce, pode haver uma restrição no acesso à API do Salesforce. Verifique com seu administrador do Salesforce para garantir que os itens a seguir estejam em vigor.

## Habilitar API nas Permissões do usuário {#enable-api-in-user-permissions}

1. Faça logon de Administrador do Salesforce no SFDC.
1. Selecionar **Configuração**.
1. Selecionar **Gerenciar usuários**.
1. Selecionar **Perfis**.
1. Encontre o Perfil em que os usuários do ToutApp estão e clique em **Editar**.
1. Role para baixo até **Permissões administrativas** e **API habilitada** está marcada.

## Verifique se o Salesforce está bloqueando a conexão de vendas {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Faça logon de Administrador do Salesforce no SFDC.
1. Selecionar **Configuração**.
1. Selecionar **Gerenciar aplicativos**.
1. Selecionar **Uso de OAuth para aplicativos conectados**.
1. Certifique-se de que a Conexão de Vendas mostra &quot;Bloco&quot; ao lado dela. Se você vir &quot;Desbloquear&quot;, clique no botão para desbloquear o acesso do Sales Connect ao Salesforce.
