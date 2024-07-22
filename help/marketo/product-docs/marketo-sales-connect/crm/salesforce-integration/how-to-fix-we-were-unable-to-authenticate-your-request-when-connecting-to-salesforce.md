---
unique-page-id: 14352484
description: Como corrigir o problema "Não foi possível autenticar sua solicitação" ao se conectar ao Salesforce - Documentação do Marketo - Documentação do produto
title: Como corrigir o problema "Não foi possível autenticar sua solicitação" ao se conectar ao Salesforce
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Como corrigir o problema &quot;Não foi possível autenticar sua solicitação&quot; ao se conectar ao Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Se você receber a mensagem de erro &quot;Não foi possível autenticar sua solicitação&quot; ao tentar conectar o Sales Connect ao Salesforce, pode haver uma restrição no seu acesso à API do Salesforce. Consulte o administrador do Salesforce para verificar se os itens a seguir estão em vigor.

## Habilitar API em Permissões do usuário {#enable-api-in-user-permissions}

1. Peça a um administrador do Salesforce que faça logon no SFDC.
1. Selecione **Instalação**.
1. Selecione **Gerenciar Usuários**.
1. Selecione **Perfis**.
1. Localize o Perfil em que estão os usuários do ToutApp e clique em **Editar**.
1. Role para baixo até **Permissões administrativas** e verifique se **API Habilitada** está marcado.

## Verifique se o Salesforce está bloqueando a conexão do Sales Connect {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Peça a um administrador do Salesforce que faça logon no SFDC.
1. Selecione **Instalação**.
1. Selecione **Gerenciar Aplicativos**.
1. Selecione **Uso do OAuth de aplicativos conectados**.
1. Certifique-se de que o Sales Connect mostre &quot;Bloquear&quot; ao lado dele. Se você vir &quot;Desbloquear&quot;, clique no botão para desbloquear o acesso do Sales Connect ao Salesforce.
