---
description: Saiba como habilitar permissões de IA do Marketo, definir regras organizacionais e gerenciar configurações como integrações e notificações.
title: Configurações e configuração
exl-id: faf642a1-25f0-4566-b35d-074b003835ed
source-git-commit: 3f7d17870cf0d60c716095ae200c003fc8ff0e28
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 3%

---

# Configurações e configuração {#settings-setup}

Saiba como habilitar permissões e usar a área Configurações para exibir detalhes de conexão, definir regras organizacionais e configurar integrações e notificações.

>[!AVAILABILITY]
>
>Este recurso está em disponibilidade limitada. Para solicitar acesso, preencha [este formulário](https://forms.cloud.microsoft/Pages/ResponsePage.aspx?id=Wht7-jR7h0OUrtLBeN7O4Y-uSf63sAxCmWyqMJg8eMFUMVZSVExSNDA3T0I4SEcwRDFSVTBGWU01Uy4u&origin=QRCode){target="_blank"}. Certifique-se de ter a Munchkin ID da sua assinatura pronta.

>[!PREREQUISITES]
>
>Para usar esse recurso, primeiro você deve concordar com os [termos principais da Gen-AI e os termos complementares](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Entre em contato com seu gerente de conta para obter detalhes.

## Permissões e funções {#permission-and-role}

Há uma permissão _Acessar a IA do Marketo_ e uma função de _Usuário da IA do Marketo_, dando aos administradores maior controle sobre quais usuários podem acessar o recurso **IA do Marketo**. A permissão é atribuída no nível da função. A função de _Usuário da IA do Marketo_ vem com a permissão _Acessar IA do Marketo_ habilitada por padrão.

>[!IMPORTANT]
>
>A permissão _Acessar Marketo AI_ não está habilitada por padrão para todas as funções. Consulte a tabela abaixo para obter detalhes.

| Função | Status padrão |
| --- | --- |
| Admin | Habilitado |
| Administrador de produtos da Adobe | Habilitado |
| Usuário de campanha de marketing | Desabilitado |
| Usuário padrão | Indisponível |
| Usuário da IA do Marketo | Habilitado |
| Funções personalizadas | Desabilitado |

### Permissão Acessar Marketo AI {#access-marketo-ai-permission}

Siga as etapas abaixo para habilitar o _Access Marketo AI_ para as funções qualificadas que ainda não o tenham habilitado.

1. Em Meu Marketo, clique em **Administrador** e depois em **Usuários e funções**.

   ![](assets/settings-setup-1.png)

1. Na guia _Funções_, selecione a função desejada e clique em **Editar Função**.

   ![](assets/settings-setup-2.png)

1. Role para baixo e marque a caixa de seleção _Acessar IA do Marketo_ e clique em **Salvar**.

   ![](assets/settings-setup-3.png)

   >[!NOTE]
   >
   >Você pode usar essas mesmas etapas para remover a permissão ao **executar** marcar a caixa de seleção _Acessar Marketo AI_.

### Função de usuário da IA do Marketo {#marketo-ai-user-role}

Siga estas etapas para atribuir um usuário específico à função _Usuário da IA do Marketo_.

>[!NOTE]
>
>Esta função **somente** contém a permissão _Acessar Marketo AI_.

1. Em Meu Marketo, clique em **Administrador** e depois em **Usuários e funções**.

   ![](assets/settings-setup-4.png)

1. Selecione o usuário desejado e clique em **Editar Usuário**.

   ![](assets/settings-setup-5.png)

1. Em _Funções e Espaços de Trabalho_, marque a caixa de seleção _Usuário da IA do Marketo_. Se você tiver mais de um espaço de trabalho, poderá especificar quais terão acesso no menu suspenso de assinaturas **+**. Clique em **Salvar** quando terminar.

   ![](assets/settings-setup-6.png)

### Função personalizada {#custom-role}

Você também tem a opção de [criar uma nova função](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"} e personalizar suas permissões, adicionando o _Access Marketo AI_, juntamente com qualquer outra coisa que desejar, e [atribuindo essa função](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"} a usuários específicos.

## Configurações {#settings}

1. Em Meu Marketo, clique no bloco **IA do Marketo**.

   ![](assets/settings-setup-7.png)

1. Clique no ícone de engrenagem.

   ![](assets/settings-setup-8.png)

### Conexão {#connection}

Esta guia não contém campos editáveis. Ele mostra as informações da conta como sua Munchkin ID e Organização IMS.

![](assets/settings-setup-9.png)

### Regras organizacionais {#organizational-rules}

Defina as diretrizes e restrições organizacionais que a IA do Marketo segue ao criar ou modificar ativos do Marketo Engage.

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
