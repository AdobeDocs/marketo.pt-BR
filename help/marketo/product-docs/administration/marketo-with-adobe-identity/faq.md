---
description: Perguntas frequentes sobre o Adobe Identity Management - Documentação do Marketo - Documentação do produto
title: Perguntas frequentes sobre o Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 8b44c3b2ccabeb796a3a8f7775848a5063279076
workflow-type: tm+mt
source-wordcount: '1645'
ht-degree: 0%

---

# Perguntas frequentes sobre o Adobe Identity Management {#adobe-identity-management-faq}

**O que é a Identidade do Adobe?**

O Sistema Adobe Identity Management consiste em três componentes.

* [!DNL Adobe Identity Service]: Gerencia a autenticação e a validação do usuário final, incluindo federação e logon único (SSO) de tempo de execução.

* Adobe Admin Console: a Admin Console fornece um local central para gerenciar direitos da Adobe em toda a organização. Ele lida com gerenciamento de usuários, serviços em nuvem, direitos de licença de desktop, configuração de federação e fornece recursos de segurança de prevenção contra perda de dados.

* API de gerenciamento de usuários do Adobe (UMAPI): permite que organizações gerenciem usuários e direitos corporativos no Adobe Admin Console no nível da API.

**Quando as assinaturas existentes do Marketo Engage serão integradas ao IMS?**

Atualmente, as assinaturas do Marketo Engage existentes estão sendo migradas para o Adobe IMS após qualquer evento de vendas, que inclui renovações, eventos de recontratação e/ou adendos. As migrações fora de um evento de vendas são compatíveis a partir de outubro de 2024.

**Após a migração, as URLs do Marketo Engage permanecerão as mesmas?**

Não. As URLs aparecerão no seguinte formato após a migração: `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (os XXXs representam a Munchkin ID e @tenantID é da sua organização da Adobe).

**Há algo que precisamos fazer para nos prepararmos para a alteração da URL?**

Sim. Após a migração, o Marketo Engage deixará de ser distribuído do experience.adobe.com para o Adobe Experience Cloud. Incluir na lista de permissões Você precisará trabalhar com sua equipe de TI para classificar todos os domínios do Adobe listados [na parte superior deste artigo](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} para evitar a interrupção do acesso ao Marketo Engage.

Links e marcadores anteriores para ativos do Marketo Engage no domínio engage-xx.marketo.com _continuarão a funcionar._ No entanto, primeiro faça logon na instância do Marketo Engage para o URL para o qual você está navegando. Por exemplo, para navegar até um marcador de uma Campanha inteligente na instância com a Munchkin ID 123-ABC-456, primeiro é necessário fazer logon na instância do Marketo Engage com a Munchkin ID 123-ABC-456.

Embora não seja planejado, o trabalho de desenvolvimento futuro pode interromper essa função de redirecionamento. Para evitar interrupções inesperadas, é recomendável atualizar os marcadores assim que possível.

**Isso funciona com SSO?**

Sim. A integração com o Adobe IMS é compatível com usuários da Universal ID e SSO. O SSO agora é orientado pelo Adobe IMS e é configurado no nível da organização na Adobe Admin Console. No entanto, há diferenças no suporte iniciado pelo Marketo Engage IdP em comparação ao suporte iniciado pelo SP da Adobe ([saiba mais aqui](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}). Se você precisar de ajuda com relação às diferenças de SSO após a migração para o Admin Console, entre em contato com o [Atendimento ao cliente da Adobe](https://helpx.adobe.com/contact.html){target="_blank"}.

**Qual é a diferença entre um Administrador de Produto do Adobe e um Administrador do Marketo Engage?**

* O Administrador de produto do Adobe é uma nova função na plataforma Marketo.
* A função de Administrador de produto do Adobe é concedida a usuários adicionados como um Administrador de produto no Adobe Admin Console
* O administrador de produto do Adobe é uma função somente leitura e não pode ser editado ou excluído do Marketo Engage.
* O administrador de produto do Adobe tem os mesmos direitos e privilégios de um administrador padrão do Marketo.
* A função de administrador do Marketo Engage ainda é de administrador e é concedida a um usuário no Marketo Engage.
* Somente os usuários com a função Admin padrão do Marketo são atribuídos como um Administrador de produto do Marketo no Admin Console.

**Há alguma alteração no suporte ao cliente da API de Gerenciamento de Usuários?**

Sim. Aqueles que foram integrados ao Adobe IMS não podem utilizar todas as APIs existentes de gerenciamento de usuários do Marketo. Para ações de convite, atualização e exclusão de usuários, as [APIs do IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} do Adobe devem ser usadas. Para o gerenciamento de funções, as APIs de gerenciamento de usuários do Marketo ainda se aplicam. Além disso, não há outras alterações no suporte ao cliente da API REST do Marketo.

**Com quem contatar para obter suporte se estivermos integrados ao IMS?**

* Migração pré-usuário: casos de suporte a arquivos na [Comunidade da Nação de Marketing](https://nation.marketo.com/t5/support/ct-p/Support) ou email `customercare@marketo.com`.

* Migração pós-usuário: casos de suporte a arquivos na [Comunidade da Nação de Marketing](https://nation.marketo.com/t5/support/ct-p/Support) ou email `customercare@marketo.com`.

* Conclusão da migração pós-suporte: os administradores de suporte de produtos podem arquivar casos por meio do portal de suporte da Experience League.

Se tiver o Ultimate Success, você terá acesso ao Admin Console Migration White Glove Service. Entre em contato com a equipe de conta da Adobe (seu Gerente de conta) para obter assistência.

**Se eu usar uma Identidade do Adobe para acessar outros aplicativos do Adobe, posso usá-la para acessar o Marketo?**

Mesmo se você tiver outros produtos da Adobe, não poderá acessar o Marketo com o Adobe Identity até que a assinatura seja migrada para o IMS.

**As funções de usuário do Marketo (em espaços de trabalho) são gerenciadas no Adobe Admin Console?**

Não. O gerenciamento de Função do usuário (em espaços de trabalho) é concluído no Marketo Engage.

**Sou um Administrador do Marketo em uma assinatura integrada do IMS e não tenho acesso à Admin Console. Como obter acesso?**

Qualquer administrador de sistema ou de produto da Adobe que tenha acesso à Admin Console da sua organização pode conceder acesso a você. Se você não tem certeza de quem na sua organização tem privilégios de administrador no console, contate o [Atendimento ao cliente da Adobe](https://helpx.adobe.com/contact.html){target="_blank"}.

**Como um Administrador adicionaria usuários ao Marketo [!DNL Sales Connect]?**

Embora exista um cartão de produto no Admin Console para [!DNL Sales Connect], o Admin Console não deve ser usado para adicionar/gerenciar usuários. O link a seguir permitirá que Administradores gerenciem usuários via Marketo [!DNL Sales Connect]: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Onde posso obter mais informações sobre a Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/br/enterprise/admin-guide.html){target="_blank"}.

**Ainda vou para a seção de Administrador no Marketo para fazer alterações na conta do usuário para minha conta?**

Não, você precisaria navegar até [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Como isso funciona com a Universal ID da Marketo?**

Os integrados à identidade da Adobe podem acessar todas as assinaturas habilitadas para IMS de maneira contínua por meio do alternador de assinaturas no produto.

**Isso funciona com SSO?**

Sim. A integração do Marketo com o Adobe IMS é compatível com usuários da Universal ID e SSO. O SSO agora é orientado pelo Adobe IMS e é configurado no nível da organização na Adobe Admin Console. [Saiba mais aqui](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}.

**Já fui integrado ao Adobe Identity e agora desejo implementar o SSO. O que devo fazer?**

Se você quiser implementar o Logon único e sua assinatura tiver sido integrada à Adobe Identity sem o SSO implementado na Organização da Adobe, envie um tíquete para o [Suporte da Marketo](https://nation.marketo.com/){target="_blank"} e especifique o tópico como &quot;Marketo no Admin Console, implementando o SSO&quot;.

**Como funciona a autorização do dispositivo?**

No momento, o Adobe IMS não oferece suporte a nada como o recurso de autorização de dispositivo do Marketo.

**Ainda é possível usar o recurso &quot;Logon na Caixa de Diálogo Convidar Usuário&quot; para tornar o logon de um usuário exclusivo em seu email?**

Não. O fluxo de trabalho do Convite de usuário não está mais ativo quando uma assinatura é habilitada para IMS, portanto, o recurso não é mais válido. A identidade do Adobe exige que a identidade de um usuário seja orientada por seu email.

**Para o Adobe IMS, temos a opção de usar o Adobe ID, Enterprise ID ou Federated ID?**

Sim, você determina o tipo de identidade para ter o suporte da sua organização. Mais informações podem ser encontradas aqui: [Visão geral da identidade](https://helpx.adobe.com/br/enterprise/using/identity.html) e aqui: [Configurar identidade](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}.

**Quais cartões de produto são compatíveis com o Adobe Admin Console?**

Os cartões de produto compatíveis são: Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect e Marketo Sales Insight Actions.

**E se meu logon de usuário não corresponder ao meu email quando eu migrar para uma Adobe Identity?**

Os usuários atuais do Marketo Engage com logons diferentes de seus endereços de email não farão mais logon com essa credencial depois de migrados para uma identidade da Adobe. As identidades da Adobe sempre são autenticadas com o endereço de email de um usuário. Você pode atualizar um endereço de email de identidade da Adobe em [account.adobe.com](https://account.adobe.com){target="_blank"}.

**O que acontece após a migração da Identidade da Adobe se minha assinatura usar configurações de restrição de IP?**

Quando as assinaturas são integradas à Adobe Identity, as configurações de restrição de IP não são migradas para a Adobe Admin Console. As configurações de restrição de IP da Marketo incluem permitir somente o acesso de endereços IP específicos e bloquear o acesso de endereços IP específicos. No momento, o Adobe Identity Management System não é compatível com recursos de restrição de IP.

Em meados de 2025, o Adobe Identity Management System lançará um recurso que permite somente endereços IP específicos, oferecendo suporte a uma transição para usuários do Marketo que atualmente utilizam esse recurso. Aqueles que atualmente usam esse recurso não serão submetidos à migração do usuário até que o recurso seja lançado. Depois que o recurso for entregue, os usuários serão notificados sobre a migração que está sendo agendada. Mais informações sobre o recurso serão fornecidas quando disponíveis.

Os usuários que atualmente usam a restrição de IP, bloqueando endereços específicos do acesso, não poderão mais usar esse recurso após a migração para o Adobe Identity, pois ele não é compatível com o Adobe Identity Management System.

**O que acontece após a migração da Adobe Identity se eu tiver usuários com uma função com a opção de &#39;Ignorar Logon Único&#39;?**

O Adobe Admin Console vem com um diretório padrão da Business ID. Os usuários fora dos domínios reivindicados nos diretórios do Federated ID em uma organização da Adobe serão atribuídos a esse diretório com um tipo de identidade da Adobe ID. Esses usuários poderão acessar o Marketo Engage sem passar pelo Logon único (SSO) e a propriedade da licença permanece com a empresa, não com os indivíduos.

**Tenho mais de uma assinatura, mas nem todas têm o Logon Único habilitado. O que acontece após a migração da Adobe Identity?**

Quando as assinaturas são integradas à Adobe Identity, o Logon único (SSO) é configurado no nível da Organização da Adobe. Isso significa que o SSO se aplica a todas as instâncias de produtos na organização da Adobe. Quando o SSO estiver configurado, ele será aplicado a todas as instâncias do Marketo nessa organização da Adobe. Anteriormente, o Marketo oferecia suporte a essa configuração no nível da instância. Isso não é suportado pelo Adobe Identity Management System.

**Há alguma alteração necessária para CNAMEs, SPF ou DKIM que usamos atualmente para o Marketo Engage após a migração da Identidade Adobe?**

Não, não há nenhum impacto nessas configurações.

**Como posso evitar que as sessões atinjam o tempo limite?**

Em [Configurações Avançadas](https://helpx.adobe.com/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}, você pode personalizar a vida útil máxima da sessão desejada (são necessárias permissões de Administrador do Sistema). É recomendável estabelecer essa configuração após a migração do produto, mas antes da migração do usuário.

**Agora preciso entrar no Experience Cloud para acessar o Marketo Engage. Há uma maneira de simplificar este fluxo?**

Sim. Você pode criar um marcador do navegador do link que é iniciado depois de clicar no botão **Iniciar** na página de entrada da instância do Marketo Engage para ignorar essa página a partir de agora.

![](assets/faq-1.png)
