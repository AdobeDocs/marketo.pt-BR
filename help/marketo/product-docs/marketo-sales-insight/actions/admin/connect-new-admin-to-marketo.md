---
description: Conecte o novo administrador ao Marketo - Documentos do Marketo - Documentação do produto
title: Conectar o novo administrador ao Marketo
hide: true
hidefromtoc: true
source-git-commit: 0ed5981470998dadd5f42384cd2e9572fec94ef6
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Conectar o novo administrador ao Marketo {#connect-new-admin-to-marketo}

Se o outro administrador já estiver conectado ao Marketo, ele só precisará fazer a Etapa 1.

Se o segundo administrador não estiver conectado ao Marketo como administrador...

1. O administrador principal precisa desconectar o segundo administrador do Marketo de Configurações > Marketo > Acesso do usuário

1. O Administrador secundário entra em sua conta do MSC, vai para Configurações > Marketo e clica em **Connect**.

1. Agora, o usuário secundário está conectado ao Marketo como administrador.

1. O administrador principal agora pode fazer logon e se desconectar do Marketo.

>[!NOTE]
>
>Os outros usuários permanecerão conectados enquanto o Usuário B estiver conectado como Administrador antes que o Usuário A se desconecte.

## Atualizar sua conexão com o Marketo {#update-your-marketo-connection}

Se decidir remover o administrador que configurou a integração do Marketo, consulte este artigo para saber como.

A integração do Marketo será vinculada a um usuário administrador do Sales Connect/Actions. Normalmente, esse é o administrador que clicou primeiro no botão &quot;Conectar&quot; na página de conexão do Marketo e estabeleceu a conexão.

Para remover o administrador que estabeleceu a conexão do Marketo, uma nova conexão deve ser estabelecida primeiro por outro usuário administrador. Listamos as tarefas abaixo que precisarão ser concluídas para fazer isso.

Para simplificar as instruções, vamos consultar o administrador conectado no momento como Administrador A e o administrador com o qual deseja estabelecer uma nova conexão com o Marketo como Administrador B:

1. O administrador A (administrador conectado atualmente) precisará remover o acesso à integração com o Marketo do administrador B (novo administrador).

1. Peça ao Administrador B (novo administrador) para estabelecer uma nova conexão com o Marketo.

1. Desconecte o administrador A (administrador conectado originalmente).

>[!NOTE]
>
>O administrador original responsável pela integração do Marketo verá uma opção de &quot;Desconexão&quot; que é clicável ao navegar para a página de integração do Marketo. Outros administradores (que não estabeleceram uma ligação) não o farão. Além disso, os administradores que tiverem acesso à integração do Marketo não poderão clicar em Conectar, por isso você deve seguir as etapas para remover o acesso à integração primeiro.

**Remover o acesso ao Marketo do administrador B**

O administrador A (administrador originalmente responsável pela conexão) deve seguir essas etapas.

1. Navegue até as configurações.

1. Clique em **Marketo**.

1. Clique em **Acesso do usuário**.

1. Procure o administrador para o qual deseja estabelecer a nova conexão do Marketo.

1. Remova o acesso.

**Estabeleça nova conexão para o administrador B**

Essas etapas devem ser seguidas pelo Administrador B (novo administrador)

1. Navegue até as configurações.

1. Clique em **Marketo**.

1. Clique em **Desconectar**.

**Desconectar a integração do Marketo para o Admin A**

Essas etapas devem ser seguidas pelo Administrador A (administrador conectado originalmente)

1. Navegue até as configurações.

1. Clique em **Marketo**.

1. Clique em **Desconectar**.

Agora que um novo administrador estabeleceu uma conexão com o Marketo e o administrador original foi desconectado, o administrador originalmente conectado pode ser removido com segurança da instância do Sales Connect/Actions.
