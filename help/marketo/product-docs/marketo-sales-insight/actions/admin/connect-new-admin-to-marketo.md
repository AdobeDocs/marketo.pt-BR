---
description: Conectar novo administrador ao Marketo - Documentação do Marketo - Documentação do produto
title: Conectar novo(a) admin ao Marketo
exl-id: ef405bca-a29a-40fc-9efa-eccff5f45956
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 2%

---

# Conectar novo(a) admin ao Marketo {#connect-new-admin-to-marketo}

Se o outro Administrador já estiver conectado ao Marketo, ele só precisará fazer a Etapa 1.

Se o segundo Administrador não estiver conectado ao Marketo como Administrador...

1. O Administrador primário precisa desconectar o segundo Administrador do Marketo de [!UICONTROL Configurações] > Marketo > [!UICONTROL Acesso de Usuário].

1. O Administrador secundário faz logon em sua conta MSC, vai para [!UICONTROL Configurações] > Marketo e clica em **[!UICONTROL Conectar]**.

1. Agora o usuário secundário está conectado ao Marketo como um Administrador.

1. O Administrador principal agora pode fazer logon e se desconectar do Marketo.

>[!NOTE]
>
>Os outros usuários permanecerão conectados enquanto o Usuário B estiver conectado como Administrador antes que o Usuário A se desconecte.

## Atualizar a conexão do Marketo {#update-your-marketo-connection}

Se você decidir remover o Administrador que configurou a integração do Marketo, consulte este artigo para saber como.

A integração do Marketo será vinculada a um usuário administrador de [!DNL Sales Connect]/Ações. Normalmente, esse é o Administrador que clicou pela primeira vez no botão **[!UICONTROL Conectar]** na página de conexão do Marketo e estabeleceu a conexão.

Para remover o Administrador que estabeleceu a conexão do Marketo, uma nova conexão deve ser estabelecida primeiro por outro usuário Administrador. Listamos abaixo as tarefas que precisarão ser concluídas para fazer isso.

Para fins de simplificação das instruções, nos referiremos ao Admin atualmente conectado como Admin A e ao Admin que você deseja estabelecer uma nova conexão com o Marketo com o como Admin B:

1. O Administrador A (atualmente conectado como Admin) precisará remover o acesso à integração com o Marketo do Administrador B (novo Admin).

1. Faça com que o Administrador B (novo Administrador) estabeleça uma nova conexão com o Marketo.

1. Desconecte o Admin A (originalmente conectado como Admin).

>[!NOTE]
>
>O administrador original responsável pela integração do Marketo verá uma opção &quot;Desconectar&quot; que é clicável ao navegar até a página de integração do Marketo. Outros administradores (que não estabeleceram uma conexão) não. Além disso, os administradores que receberam acesso à integração do Marketo não poderão clicar em Conectar, por isso é necessário seguir as etapas para remover o acesso à integração primeiro.

**Remover o Acesso ao Marketo do Administrador B**

O administrador A (originalmente responsável pela conexão) deve seguir essas etapas.

1. No aplicativo Web, clique no ícone de engrenagem e selecione **[!UICONTROL Configurações]**.

1. Clique em **Marketo**.

1. Clique em **[!UICONTROL Acesso de Usuário]**.

1. Procure pelo Administrador para o qual você deseja estabelecer a nova conexão do Marketo.

1. Remover acesso.

**Estabelecer nova conexão para o administrador B**

Essas etapas devem ser seguidas pelo Administrador B (novo administrador)

1. No aplicativo Web, clique no ícone de engrenagem e selecione **[!UICONTROL Configurações]**.

1. Clique em **Marketo**.

1. Clique em **[!UICONTROL Desconectar]**.

**Desconectar Integração do Marketo para o Administrador A**

Essas etapas devem ser seguidas pelo Administrador A (originalmente conectado como Administrador).

1. No aplicativo Web, clique no ícone de engrenagem e selecione **[!UICONTROL Configurações]**.

1. Clique em **Marketo**.

1. Clique em **[!UICONTROL Desconectar]**.

Agora que um novo Administrador estabeleceu uma conexão com o Marketo e o Administrador original foi desconectado, o Administrador originalmente conectado pode ser removido com segurança da instância [!DNL Sales Connect]/Ações.
