---
description: Saiba como habilitar permissões de IA do Marketo, definir regras organizacionais e gerenciar configurações como integrações e notificações.
title: Configurações e configuração
hide: true
hidefromtoc: true
exl-id: d6f37214-65b9-48c1-bf9f-d64b4eda87b9
source-git-commit: dc2126b2949411a436cb48a91d187ec8b8fa21f2
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Configurações e configuração {#settings-setup}

Saiba como habilitar permissões e usar a área Configurações para exibir detalhes de conexão, definir regras organizacionais e configurar integrações e notificações.

## Permissões {#permissions}

>[!IMPORTANT]
>
>Na fase Alpha da IA do Marketo, o _acesso é habilitado por padrão_ para as seguintes funções: Administrador, Administrador de produto do Adobe, Usuário de marketing, Usuário padrão. Portanto, em vez de ativá-lo para funções que você deseja ter acesso, desative-o para funções que não deseja.

### Acesso para todos {#access-for-all}

Se você quiser que a IA do Marketo seja habilitada para todas as funções listadas acima, não é necessário fazer nada.

### Acesso para alguns {#access-for-some}

Se quiser remover o acesso de qualquer função, siga as etapas abaixo.

1. Em Meu Marketo, clique em **Administrador** e depois em **Usuários e funções**.

   ![](assets/settings-setup-1.png)

1. Na guia _Funções_, selecione a função desejada e clique em **Editar Função**.

   ![](assets/settings-setup-2.png)

1. Role para baixo e _desmarque_ a caixa de seleção **Acessar compilação com IA** e clique em **Salvar**.

   ![](assets/settings-setup-3.png)

Repita essas etapas para qualquer outra função desejada.

### Função personalizada {#custom-role}

Você também tem a opção de [criar uma nova função](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"} e personalizar suas permissões, adicionando a _Compilação do Access com IA_, juntamente com qualquer outra coisa que desejar, e [atribuindo essa função](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"} a usuários específicos.

<!-- ## Permissions {#permissions}

In order to access Marketo AI, Admins must first enable role permissions. 

1. In your My Marketo, click **Admin**, then **Users & Roles**.

   ![](assets/settings-setup-1.png)

1. In the _Roles_ tab, select the desired role and click **Edit Role**.

   ![](assets/settings-setup-2.png)

1. Scroll down and select the **Access Build with AI** checkbox and click **Save**.

   ![](assets/settings-setup-3.png)

-->

## Configurações {#settings}

1. Em Minha Marketo, clique no bloco **Criar com IA**.

   ![](assets/settings-setup-4.png)

1. Clique no ícone de engrenagem.

   ![](assets/settings-setup-5.png)

### Conexão {#connection}

Esta guia não contém campos editáveis. Ele mostra as informações da conta como sua Munchkin ID e Organização IMS.

![](assets/settings-setup-6.png)

### Regras organizacionais {#organizational-rules}

Defina as diretrizes e restrições organizacionais que a IA do Marketo segue ao criar ou modificar ativos do Marketo Engage.

![](assets/settings-setup-7.png){width="800" zoomable="yes"}

>[!NOTE]
>
>As regras usam o formato Markdown com o material de frente YAML. As regras globais se aplicam a todos os espaços de trabalho. As regras do Workspace substituem as configurações globais.

### Integrações (em breve) {#integrations}

Configure conexões com serviços e APIs externos.

_Esta guia pode aparecer na interface do usuário, mas ainda não está disponível para uso. Procure atualizações_.

### Notificações (em breve) {#notifications}

Gerencie preferências de alerta e canais de notificação.

_Esta guia pode aparecer na interface do usuário, mas ainda não está disponível para uso. Procure atualizações_.
