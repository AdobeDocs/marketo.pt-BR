---
description: Saiba como habilitar o Colaborador para permissões do Marketo Engage, definir regras organizacionais e gerenciar configurações como integrações e notificações.
title: Configurações e configuração
source-git-commit: 01cad5c7d14083c0ef7127850f2488dbfd71f57b
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 3%

---

# Configurações e configuração {#settings-setup}

Saiba como habilitar permissões e usar a área Configurações para exibir detalhes de conexão, definir regras organizacionais e configurar integrações e notificações.

>[!AVAILABILITY]
>
>Esse recurso está disponível para todas as assinaturas. Se você não visualizar o bloco Colaborador para Marketo Engage na tela Meu Marketo, entre em contato com o gerente da conta. Você também deve concordar com os [termos principais da Gen-AI e os termos complementares](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}.

## Permissões e funções {#permission-and-role}

Há uma permissão de _Colaborador de Acesso para o Marketo Engage_ e uma função de _Colaborador para Usuário do Marketo Engage_, dando aos administradores maior controle sobre quais usuários podem acessar o recurso **Colaborador para o Marketo Engage**. A permissão é atribuída no nível da função. O _Colaborador do Usuário do Marketo Engage_ vem com a permissão de _Colaborador do Acesso para o Marketo Engage_ habilitada por padrão.

>[!NOTE]
>
>A permissão _Access Coworker para Marketo Engage_ não está habilitada por padrão para todas as funções. Consulte a tabela abaixo para obter detalhes.

| Função | Status padrão |
| --- | --- |
| Admin | Habilitado |
| Administrador de produtos da Adobe | Habilitado |
| Usuário de campanha de marketing | Desabilitado |
| Usuário padrão | Indisponível |
| Colaborador para usuário do Marketo Engage | Habilitado |
| Funções personalizadas | Desabilitado |

### Permissão Acessar Colaborador para Marketo Engage {#access-coworker-marketo-permission}

Siga as etapas abaixo para habilitar o _Access Coworker for Marketo Engage_ para funções qualificadas que ainda não o tenham habilitado.

1. Em Meu Marketo, clique em **Administrador** e depois em **Usuários e funções**.

   ![](assets/settings-setup-1.png)

1. Na guia _Funções_, selecione a função desejada e clique em **Editar Função**.

   ![](assets/settings-setup-2.png)

1. Role para baixo e marque a caixa de seleção _Acessar Colaborador para Marketo Engage_ e clique em **Salvar**.

   ![](assets/settings-setup-3.png)

   >[!NOTE]
   >
   >Você pode usar essas mesmas etapas para remover a permissão ao **executar** marcar a caixa de seleção _Acessar Colaborador para Marketo Engage_.

### Colaborador para a função de usuário do Marketo Engage {#coworker-marketo-user-role}

Siga estas etapas para atribuir um usuário específico à função _Colaborador do Usuário do Marketo Engage_.

>[!NOTE]
>
>Esta função **somente** contém a permissão _Colaborador de Acesso para Marketo Engage_.

1. Em Meu Marketo, clique em **Administrador** e depois em **Usuários e funções**.

   ![](assets/settings-setup-4.png)

1. Selecione o usuário desejado e clique em **Editar Usuário**.

   ![](assets/settings-setup-5.png)

1. Em _Funções e Espaços de Trabalho_, marque a caixa de seleção _Colaborador do Usuário do Marketo Engage_. Se você tiver mais de um espaço de trabalho, poderá especificar quais terão acesso no menu suspenso de assinaturas **+**. Clique em **Salvar** quando terminar.

   ![](assets/settings-setup-6.png)

### Função personalizada {#custom-role}

Você também tem a opção de [criar uma nova função](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"} e personalizar suas permissões, adicionando o _Access Coworker para Marketo Engage_, juntamente com qualquer outra coisa que desejar, e [atribuindo essa função](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"} a usuários específicos.

## Configurações {#settings}

1. Em Meu Marketo, clique no bloco **[!UICONTROL Colaborador do Marketo Engage]**.

   ![](assets/settings-setup-7.png)

1. Clique no ícone de engrenagem.

   ![](assets/settings-setup-8.png)

### Conexão {#connection}

Esta guia não contém campos editáveis. Ele mostra informações da conta como sua Munchkin ID e Organização IMS.

![](assets/settings-setup-9.png)

### Regras organizacionais {#organizational-rules}

Defina as diretrizes e restrições organizacionais que o Colaborador do Marketo Engage segue ao criar ou modificar ativos do Marketo Engage.

![](assets/settings-setup-10.png){width="800" zoomable="yes"}

>[!NOTE]
>
>As regras usam o formato Markdown com o material de frente YAML. As regras globais se aplicam a todos os espaços de trabalho. As regras do Workspace substituem as configurações globais.

### Integrações (em breve) {#integrations}

Configure conexões com serviços e APIs externos.

_Esta guia pode aparecer na interface do usuário, mas ainda não está disponível para uso. Procure atualizações_.

### Notificações (em breve) {#notifications}

Gerencie preferências de alerta e canais de notificação.

_Esta guia pode aparecer na interface do usuário, mas ainda não está disponível para uso. Verifique se há atualizações neste artigo_.
