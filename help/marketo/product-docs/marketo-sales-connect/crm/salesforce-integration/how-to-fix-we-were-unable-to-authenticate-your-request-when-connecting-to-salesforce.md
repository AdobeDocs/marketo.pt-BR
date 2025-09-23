---
unique-page-id: 14352484
description: Como corrigir o problema "Não foi possível autenticar sua solicitação" ao se conectar ao Salesforce - Documentação do Marketo - Documentação do produto
title: Como corrigir o problema “Não foi possível autenticar sua solicitação” ao se conectar ao Salesforce
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 65d607e279fb86b0816ccaec2f4bf3c69e309cb9
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 8%

---

# Como Corrigir &quot;Não Foi Possível Autenticar Sua Solicitação&quot; ao Conectar-se a [!DNL Salesforce] {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Se você receber a mensagem de erro &quot;Não foi possível autenticar sua solicitação&quot; ao tentar conectar [!DNL Sales Connect] a [!DNL Salesforce], poderá haver uma restrição no seu acesso à API do [!DNL Salesforce]. Consulte o administrador do [!DNL Salesforce] para verificar se os itens a seguir estão em vigor.

## Habilitar API em Permissões do usuário {#enable-api-in-user-permissions}

1. Peça a um administrador [!DNL Salesforce] para fazer logon no SFDC.
1. Selecione **[!UICONTROL Instalação]**.
1. Selecione **[!UICONTROL Gerenciar Usuários]**.
1. Selecione **[!UICONTROL Perfis]**.
1. Localize o Perfil em que estão os usuários do ToutApp e clique em **[!UICONTROL Editar]**.
1. Role para baixo até **[!UICONTROL Permissões administrativas]** e verifique se **[!UICONTROL API Habilitada]** está marcado.

## Verifique se [!DNL Salesforce] está impedindo [!DNL Sales Connect] de se conectar {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Peça a um administrador [!DNL Salesforce] para fazer logon no SFDC.
1. Selecione **[!UICONTROL Instalação]**.
1. Selecione **[!UICONTROL Gerenciar Aplicativos]**.
1. Selecione **[!UICONTROL Uso do OAuth de aplicativos conectados]**.
1. Certifique-se de que [!DNL Sales Connect] mostra &quot;[!UICONTROL Bloco]&quot; ao lado dele. Se você vir &quot;[!UICONTROL Desbloquear]&quot;, clique no botão para desbloquear o acesso de [!DNL Sales Connect] a [!DNL Salesforce].
