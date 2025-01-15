---
description: Perguntas frequentes sobre o Adobe Identity Management - Documentação do Marketo - Documentação do produto
title: Perguntas frequentes sobre o Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 573a40c7d2ee7329d82d209bfefc284497295239
workflow-type: tm+mt
source-wordcount: '1595'
ht-degree: 0%

---

# Perguntas frequentes sobre o Adobe Identity Management {#adobe-identity-management-faq}

**O que é a Identidade Adobe?**

O sistema Adobe Identity Management consiste em três componentes.

* [!DNL Adobe Identity Service]: Gerencia a autenticação e a validação do usuário final, incluindo federação e logon único (SSO) de tempo de execução.

* Adobe Admin Console: o Admin Console fornece um local central para gerenciar direitos de Adobe em toda a organização. Ele lida com gerenciamento de usuários, serviços em nuvem, direitos de licença de desktop, configuração de federação e fornece recursos de segurança de prevenção contra perda de dados.

* API de gerenciamento de usuários do Adobe (UMAPI): permite que organizações gerenciem usuários e direitos corporativos no Adobe Admin Console no nível da API.

**Quando as assinaturas de Marketo Engage existentes serão integradas ao IMS?**

Atualmente, as assinaturas de Marketo Engage existentes estão sendo migradas para o Adobe IMS após qualquer evento de vendas, que inclui renovações, eventos de recontratação e/ou adendos. As migrações fora de um evento de vendas são compatíveis a partir de outubro de 2024.

**Após a migração, as URLs do Marketo Engage permanecerão as mesmas?**

Não. Os URLs serão diferentes após a migração.

**Há algo que precisamos fazer para nos prepararmos para a alteração da URL?**

Sim. Após a migração, o Marketo Engage deixará de ser distribuído do experience.adobe.com para o Adobe Experience Cloud. Incluir na lista de permissões Você precisará trabalhar com sua equipe de TI para classificar todos os domínios de Adobe [na parte superior deste artigo](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} para evitar a interrupção do acesso ao Marketo Engage.

Links e marcadores anteriores para ativos Marketo Engage no domínio engage-xx.marketo.com _continuarão a funcionar._ No entanto, primeiro você deve fazer logon na instância do Marketo Engage para o URL para o qual está navegando. Por exemplo, para navegar até um marcador para uma Campanha inteligente na instância com a Munchkin ID 123-ABC-456, é necessário primeiro fazer logon na instância do Marketo Engage com a Munchkin ID 123-ABC-456.

**Isso funciona com SSO?**

Sim. A integração com o Adobe IMS é compatível com usuários da Universal ID e SSO. O SSO agora é orientado pelo Adobe IMS e é configurado no nível da organização na Adobe Admin Console. Entretanto, há diferenças no suporte iniciado por IdP de Marketo Engage em comparação ao suporte iniciado por SP de Adobe ([saiba mais aqui](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}). Se você precisar de ajuda com relação às diferenças de SSO depois de migrar para o Admin Console, entre em contato com o [Adobe Customer Care](https://helpx.adobe.com/contact.html){target="_blank"}.

**Qual é a diferença entre um Administrador de Produto do Adobe e um Administrador de Marketo Engage?**

* O administrador de produto do Adobe é uma nova função na plataforma Marketo.
* A função de administrador de produto do Adobe é concedida a usuários adicionados como um administrador de produto no Adobe Admin Console
* O administrador de produto do Adobe é uma função somente leitura e não pode ser editado ou excluído do Marketo Engage.
* O administrador de produto do Adobe tem os mesmos direitos e privilégios de um administrador de Marketo padrão.
* A função do administrador de Marketo Engage ainda é de administrador e é concedida a um usuário no Marketo Engage.

**Há alguma alteração no suporte ao cliente da API de Gerenciamento de Usuários?**

Sim. Aqueles que foram integrados ao Adobe IMS não podem utilizar todas as APIs existentes de gerenciamento de usuários do Marketo. Para ações de convite, atualização e exclusão de usuários, as [APIs de IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} do Adobe devem ser usadas. Para o gerenciamento de funções, as APIs de gerenciamento de usuários do Marketo ainda se aplicam. Além disso, não há outras alterações no suporte ao cliente da API REST do Marketo.

**Com quem contatar para obter suporte se estivermos integrados ao IMS?**

* Migração pré-usuário: casos de suporte a arquivos na [Comunidade da Nação de Marketing](https://nation.marketo.com/t5/support/ct-p/Support) ou email `customercare@marketo.com`.

* Migração pós-usuário: casos de suporte a arquivos na [Comunidade da Nação de Marketing](https://nation.marketo.com/t5/support/ct-p/Support) ou email `customercare@marketo.com`.

* Conclusão da migração pós-suporte: os administradores de suporte de produtos podem arquivar casos por meio do portal de suporte do Experience League.

Se tiver sucesso no Ultimate, você terá acesso ao Admin Console Migration White Glove Service. Entre em contato com a equipe de conta do Adobe (seu gerente de conta) para obter assistência.

**Se eu usar uma Identidade de Adobe para acessar outros aplicativos de Adobe, posso usá-la para acessar o Marketo?**

Mesmo se você tiver outros produtos Adobe, não poderá acessar o Marketo com Adobe Identity até que a assinatura seja migrada para o IMS.

**As funções de usuário do Marketo (em espaços de trabalho) são gerenciadas no Adobe Admin Console?**

Não. O gerenciamento de Função do usuário (em espaços de trabalho) é concluído no Marketo Engage.

**Sou um Administrador do Marketo em uma assinatura integrada do IMS e não tenho acesso ao Admin Console. Como obter acesso?**

Qualquer sistema Adobe ou administrador de produto que tenha acesso ao Admin Console da sua organização pode conceder acesso a você. Se você não tem certeza de quem na sua organização tem privilégios de administrador no console, contate o [Atendimento ao cliente do Adobe](https://helpx.adobe.com/contact.html){target="_blank"}.

**Como um Administrador adicionaria usuários ao Marketo [!DNL Sales Connect]?**

Embora exista um cartão de produto no Admin Console para [!DNL Sales Connect], o Admin Console não deve ser usado para adicionar/gerenciar usuários. O link a seguir permitirá que Administradores gerenciem usuários via Marketo [!DNL Sales Connect]: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Onde posso obter mais informações sobre a Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/br/enterprise/admin-guide.html){target="_blank"}.

**Ainda vou para a seção de Administrador no Marketo para fazer alterações na conta do usuário para minha conta?**

Não, você precisaria navegar para [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Como isso funciona com a Universal ID da Marketo?**

Os integrados à identidade Adobe podem acessar todas as assinaturas habilitadas para IMS de maneira contínua por meio do alternador de assinaturas no produto.

**Isso funciona com SSO?**

Sim. A integração do Marketo com o Adobe IMS é compatível com usuários da Universal ID e SSO. O SSO agora é orientado pelo Adobe IMS e é configurado no nível da organização na Adobe Admin Console. [Saiba mais aqui](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}.

**Já fui integrado ao Adobe Identity e agora desejo implementar o SSO. O que devo fazer?**

Se você quiser implementar o Logon único e sua assinatura tiver sido integrada à Identidade do Adobe sem SSO implementado na Organização do Adobe, envie um tíquete para o [Suporte da Marketo](https://nation.marketo.com/){target="_blank"} e especifique o tópico como &quot;Marketo no Admin Console, implementando o SSO.&quot;

**Como funciona a autorização do dispositivo?**

No momento, o Adobe IMS não oferece suporte a nada como o recurso de autorização de dispositivo do Marketo.

**Ainda é possível usar o recurso &quot;Logon na Caixa de Diálogo Convidar Usuário&quot; para tornar o logon de um usuário exclusivo em seu email?**

Não. O fluxo de trabalho do Convite de usuário não está mais ativo quando uma assinatura é habilitada para IMS, portanto, o recurso não é mais válido. A identidade Adobe exige que a identidade de um usuário seja orientada por seu email.

**Para o Adobe IMS, temos a opção de usar Adobe ID, Enterprise ID ou Federated ID?**

Sim, você determina o tipo de identidade para ter o suporte da sua organização. Mais informações podem ser encontradas aqui: [Visão geral da identidade](https://helpx.adobe.com/br/enterprise/using/identity.html) e aqui: [Configurar identidade](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}.

**Quais cartões de produto são compatíveis com o Adobe Admin Console?**

As placas de produto compatíveis são: Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect e Marketo Sales Insight Actions.

**E se meu logon de usuário não corresponder ao meu email quando eu migrar para uma Identidade Adobe?**

Os usuários atuais do Marketo Engage com logons diferentes de seu endereço de email não farão mais logon com essa credencial depois de migrados para uma Identidade do Adobe. As identidades Adobe sempre são autenticadas com o endereço de email de um usuário. Você pode atualizar um endereço de email de identidade do Adobe em [account.adobe.com](https://account.adobe.com){target="_blank"}.

**O que acontece após a migração da Identidade do Adobe se minha assinatura usar configurações de restrição de IP?**

Quando as assinaturas são integradas à Identidade do Adobe, as configurações de restrição de IP não são migradas para o Adobe Admin Console. As configurações de restrição de IP da Marketo incluem permitir somente o acesso de endereços IP específicos e bloquear o acesso de endereços IP específicos. No momento, o Adobe Identity Management System não oferece suporte aos recursos de restrição de IP.

A partir do início de 2025, o Adobe Identity Management System lançará um recurso para oferecer suporte somente a endereços IP específicos, oferecendo suporte a uma transição para usuários do Marketo que atualmente utilizam esse recurso. Aqueles que atualmente usam esse recurso não serão submetidos à migração do usuário até que o recurso seja lançado. Depois que o recurso for entregue, os usuários serão notificados sobre a migração que está sendo agendada. Mais informações sobre o recurso serão fornecidas quando disponíveis.

Os usuários que atualmente usam a restrição de IP, bloqueando endereços específicos do acesso, não poderão mais usar esse recurso após serem migrados para a Identidade do Adobe, pois ele não é compatível com o Sistema Adobe Identity Management.

**O que acontece após a migração de identidade do Adobe se eu tiver usuários com uma função com a opção de &#39;Ignorar logon único&#39;?**

Quando as assinaturas são integradas à Identidade do Adobe, o Logon único (SSO) é configurado no nível da Organização do Adobe para todos os usuários. Quando o SSO estiver configurado, ele será aplicado a todos os usuários do Marketo/todas as instâncias do Marketo nessa Adobe Org. Anteriormente, o Marketo permitia que uma função de usuário fosse configurada para ter a opção de &#39;Ignorar logon único&#39;. Isso não é suportado pelo sistema Adobe Identity Management.

**Tenho mais de uma assinatura, mas nem todas têm o Logon Único habilitado. O que acontece após a migração de identidade do Adobe?**

Quando as assinaturas são integradas à Identidade do Adobe, o Logon único (SSO) é configurado no nível da Organização do Adobe. Isso significa que o SSO se aplica a todas as instâncias de produto na Adobe Org. Quando o SSO estiver configurado, ele será aplicado a todas as instâncias do Marketo nessa Adobe Org. Anteriormente, o Marketo oferecia suporte a essa configuração no nível da instância. Isso não é suportado pelo sistema Adobe Identity Management.

**Há alguma alteração necessária para CNAMEs, SPF ou DKIM que usamos atualmente para o Marketo Engage após a migração da Identidade Adobe?**

Não, não há nenhum impacto nessas configurações.

**Como posso evitar que as sessões atinjam o tempo limite?**

Em [Configurações Avançadas](https://helpx.adobe.com/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}, você pode personalizar a vida útil máxima da sessão desejada (são necessárias permissões de Administrador do Sistema). É recomendável estabelecer essa configuração após a migração do produto, mas antes da migração do usuário.

**Agora preciso entrar no Experience Cloud para acessar o Marketo Engage. Há uma maneira de simplificar este fluxo?**

Sim. Você pode criar um marcador do navegador do link que é iniciado depois de clicar no botão **Iniciar** na página de entrada da instância do Marketo Engage para ignorar essa página a partir de agora.

![](assets/faq-1.png)
