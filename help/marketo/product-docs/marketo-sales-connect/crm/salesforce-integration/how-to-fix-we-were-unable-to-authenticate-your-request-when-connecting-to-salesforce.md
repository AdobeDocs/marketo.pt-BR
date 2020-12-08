---
unique-page-id: 14352484
description: Como corrigir "Não foi possível autenticar sua solicitação" ao conectar-se ao Salesforce - Marketing to Docs - Documentação do produto
title: Como corrigir "Não foi possível autenticar sua solicitação" ao conectar-se ao Salesforce
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Como corrigir &quot;Não foi possível autenticar sua solicitação&quot; ao conectar-se ao Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Se você receber a mensagem de erro &quot;Não foi possível autenticar sua solicitação&quot; ao tentar conectar o Sales Connect ao Salesforce, pode haver uma restrição no seu acesso à API do Salesforce. Consulte seu administrador do Salesforce para verificar se os seguintes itens estão no lugar.

## Habilitar API em permissões de usuário {#enable-api-in-user-permissions}

1. Faça logon de administrador do Salesforce no SFDC.
1. Selecione **Configuração**.
1. Selecione **Gerenciar usuários**.
1. Selecione **Perfis**.
1. Encontre o Perfil em que os usuários do ToutApp estão e clique em **Editar**.
1. Role para baixo até Permissões **** administrativas e verifique se a opção **API ativada** está marcada.

## Verifique se o Salesforce está bloqueando a conexão do Sales Connect {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Faça logon de administrador do Salesforce no SFDC.
1. Selecione **Configuração**.
1. Selecione **Gerenciar aplicativos**.
1. Selecione **Aplicativos conectados Uso OAuth**.
1. Certifique-se de que o Sales Connect exiba &quot;Bloco&quot; ao lado dele. Se você vir &quot;Desbloquear&quot;, clique no botão para desbloquear o acesso do Sales Connect ao Salesforce.

