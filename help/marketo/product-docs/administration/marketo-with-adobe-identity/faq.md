---
description: Perguntas frequentes sobre o Adobe Identity Management - Documentação do Marketo - Documentação do produto
title: Perguntas frequentes sobre o Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 2%

---

# Perguntas frequentes {#faq}

**O que é a Identidade Adobe?**

O sistema Adobe Identity Management consiste em três componentes.

* [!DNL Adobe Identity Service]: lida com autenticação e validação do usuário final, incluindo federação e logon único (SSO) de tempo de execução.

* Adobe Admin Console: o Admin Console fornece um local central para gerenciar direitos de Adobe em toda a organização. Ele lida com gerenciamento de usuários, serviços em nuvem, direitos de licença de desktop, configuração de federação e fornece recursos de segurança de prevenção contra perda de dados.

* API de gerenciamento de usuários do Adobe (UMAPI): permite que organizações gerenciem usuários e direitos corporativos no Adobe Admin Console no nível da API.

**Quando as assinaturas Marketo Engage existentes serão integradas ao IMS?**

As assinaturas existentes do Marketo serão migradas para o Sistema Adobe Identity Management ainda este ano. O Suporte da Marketo não poderá fornecer atualizações relacionadas à migração do Adobe IMS. A equipe da conta do Adobe entrará em contato com a linha do tempo estimada para os próximos meses.

**Qual é a diferença entre um Administrador de produto do Adobe e um Administrador de Marketo Engage?**

* O administrador de produto do Adobe é uma nova função na plataforma Marketo.
* A função de administrador de produto do Adobe é concedida a usuários adicionados como um administrador de produto no Adobe Admin Console
* O administrador de produto do Adobe é uma função somente leitura e não pode ser editado ou excluído do Marketo Engage.
* O administrador de produto do Adobe tem os mesmos direitos e privilégios de um administrador de Marketo padrão.
* A função do administrador de Marketo Engage ainda é de administrador e é concedida a um usuário no Marketo Engage.

**Há alguma mudança no suporte ao cliente da API de gerenciamento de usuários?**

Sim. Aqueles que foram integrados ao Adobe IMS não podem utilizar todas as APIs existentes de gerenciamento de usuários do Marketo. Para ações de convite, atualização e exclusão do usuário, o Adobe [APIs IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} deve ser usado. Para o gerenciamento de funções, as APIs de gerenciamento de usuários do Marketo ainda se aplicam. Além disso, não há outras alterações no suporte ao cliente da API REST do Marketo.

**Com quem devemos entrar em contato para obter suporte se estivermos integrados ao IMS?**

Você seguiria o procedimento padrão para entrar em contato com [Suporte ao Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

**Se eu usar uma Identidade de Adobe para acessar outros aplicativos de Adobe, é possível usá-la para acessar o Marketo?**

Mesmo se você tiver outros produtos Adobe, não poderá acessar o Marketo com Adobe Identity até que a assinatura seja migrada para o IMS.

**As funções de usuário do Marketo (em espaços de trabalho) são gerenciadas no Adobe Admin Console?**

Nº O gerenciamento de Função do usuário (em espaços de trabalho) é concluído no Marketo Engage.

**Sou um Administrador do Marketo em uma assinatura integrada do IMS e não tenho acesso ao Admin Console. Como faço para obter acesso?**

Qualquer sistema Adobe ou administrador de produto que tenha acesso ao Admin Console da sua organização pode conceder acesso a você. Se você não tem certeza de quem na sua organização tem privilégios de administrador no console, entre em contato com [Atendimento ao cliente Adobe](https://helpx.adobe.com/contact.html){target="_blank"}.

**Como um administrador adicionaria usuários ao Marketo [!DNL Sales Connect]?**

Embora exista um cartão de produto no Admin Console para [!DNL Sales Connect], o Admin Console não deve ser usado para adicionar/gerenciar usuários. O link a seguir permitirá que administradores gerenciem usuários por meio do Marketo [!DNL Sales Connect]: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Onde posso obter mais informações sobre a Adobe Admin Console?**

[https://helpx.adobe.com/br/enterprise/admin-guide.html](https://helpx.adobe.com/br/enterprise/admin-guide.html){target="_blank"}.

**Ainda posso ir até a seção Administrador no Marketo para fazer alterações na conta do usuário para minha conta?**

Não, você precisaria navegar para [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Como isso funciona com a Universal ID da Marketo?**

Os integrados à identidade Adobe podem acessar todas as assinaturas habilitadas para IMS de maneira contínua por meio do alternador de assinaturas no produto.

**Isso funciona com SSO?**

Sim. A integração do Marketo com o Adobe IMS é compatível com usuários da Universal ID e SSO. O SSO agora é orientado pelo Adobe IMS e é configurado no nível da organização na Adobe Admin Console. [Saiba mais aqui](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**Como funciona a autorização do dispositivo?**

No momento, o Adobe IMS não oferece suporte a nada como o recurso de autorização de dispositivo do Marketo.

**Ainda é possível usar o recurso &quot;Logon na caixa de diálogo Convidar usuário&quot; para tornar o logon de um usuário exclusivo em seu email?**

Nº O fluxo de trabalho do Convite de usuário não está mais ativo quando uma assinatura é habilitada para IMS, portanto, o recurso não é mais válido. A identidade Adobe exige que a identidade de um usuário seja orientada por seu email.

**Para o Adobe IMS, temos a opção de usar Adobe ID, Enterprise ID ou Federated ID?**

Sim, você determina o tipo de identidade para ter o suporte da sua organização. Mais informações podem ser encontradas aqui: [Visão geral da identidade](https://helpx.adobe.com/enterprise/using/identity.html) e aqui: [Configurar identidade](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**Quais cartões de produto são compatíveis com o Adobe Admin Console?**

As placas de produto compatíveis são: Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect e Marketo Sales Insight Actions.
