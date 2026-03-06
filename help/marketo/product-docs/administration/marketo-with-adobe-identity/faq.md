---
description: Perguntas frequentes sobre a Adobe Identity for Marketo Engage, incluindo migração, URLs, SSO, administrador de produto versus administrador do Marketo e incluir na lista de permissões.
title: Perguntas frequentes sobre o gerenciamento de identidades da Adobe
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '1591'
ht-degree: 98%

---

# Perguntas frequentes sobre o gerenciamento de identidades da Adobe {#adobe-identity-management-faq}

**O que é a identidade da Adobe?**

O Adobe Identity Management System consiste em três componentes.

* [!DNL Adobe Identity Service]: cuida da autenticação e validação do usuário final, incluindo federação e logon único (SSO) de tempo de execução.

* Adobe Admin Console: o Admin Console é uma central de gerenciamento de direitos da Adobe para toda a empresa. Ele cuida do gerenciamento de usuários, serviços na nuvem, direitos de licenças para desktop e configuração de federação, e fornece recursos de segurança e prevenção contra perda de dados.

* API de gerenciamento de usuários da Adobe (UMAPI): permite que as organizações gerenciem usuários e direitos empresariais no Adobe Admin Console, no nível da API.

**Quando as assinaturas já existentes do Marketo Engage serão integradas ao IMS?**

Atualmente, as assinaturas do Marketo Engage estão sendo migradas para o Adobe IMS após qualquer evento de vendas, que inclui renovações, eventos de recontratação e/ou adendos. As migrações fora de um evento de vendas são permitidas desde outubro de 2024.

**Após a migração, os URLs do Marketo Engage continuam iguais?**

Não. Os URLs aparecem no seguinte formato após a migração: `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (os XXXs representam Munchkin ID, e @tenantID é o da sua organização da Adobe).

**Temos que fazer algo para nos preparar para a alteração dos URLs?**

Sim. Após a migração, o Marketo Engage deixa de ser distribuído pelo site experience.adobe.com e passa para a Adobe Experience Cloud. Você precisa colaborar com a sua equipe de TI para incluir na lista de permissões todos os domínios da Adobe listados [na parte superior deste artigo](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} a fim de evitar a interrupção do acesso ao Marketo Engage.

Os links e marcadores anteriores de ativos do Marketo Engage no domínio engage-xx.marketo.com _continuarão_ funcionando. No entanto, primeiro faça logon na instância do Marketo Engage referente ao URL até o qual você está navegando. Por exemplo, para navegar até um marcador de uma campanha inteligente na instância com o Munchkin ID 123-ABC-456, primeiro é necessário fazer logon na instância do Marketo Engage com o Munchkin ID 123-ABC-456.

Embora não esteja planejado, o trabalho de desenvolvimento futuro pode interromper essa função de redirecionamento. Para evitar interrupções inesperadas, é recomendável atualizar os marcadores assim que possível.

**Isso funciona com o SSO?**

Sim. A integração com o Adobe IMS é compatível com usuários do Universal ID e SSO. Agora, o SSO é orientado pelo Adobe IMS e configurado no nível da organização no Adobe Admin Console. No entanto, há diferenças na compatibilidade iniciada pelo IdP do Marketo Engage em comparação com a compatibilidade iniciada pelo SP da Adobe ([saiba mais aqui](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}). Se você precisar de ajuda em relação às diferenças do SSO após a migração para o Admin Console, entre em contato com o [Atendimento ao cliente da Adobe](https://helpx.adobe.com/br/contact.html){target="_blank"}.

**Qual é a diferença entre um administrador de produtos da Adobe e um administrador do Marketo Engage?**

* O administrador de produtos da Adobe é uma nova função na plataforma do Marketo.
* A função de administrador de produtos da Adobe é concedida a usuários adicionados como administrador de produtos no Adobe Admin Console
* O administrador de produtos da Adobe é uma função somente de leitura e não pode ser editado nem excluído do Marketo Engage.
* O administrador de produtos da Adobe tem os mesmos direitos e privilégios que um administrador padrão do Marketo.
* A função de administrador do Marketo Engage ainda é de administrador, sendo concedida a um usuário no Marketo Engage.
* Somente os usuários com a função de administrador padrão do Marketo são atribuídos como um administrador de produtos do Marketo no Admin Console.

**Há alguma alteração no suporte ao cliente da API de gerenciamento de usuários?**

Sim. Quem tiver sido integrado ao Adobe IMS não poderá utilizar todas as APIs de gerenciamento de usuários do Marketo. No caso de ações de convite, atualização e exclusão de usuários, as [APIs do IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} da Adobe devem ser usadas. No caso do gerenciamento de funções, as APIs de gerenciamento de usuários do Marketo ainda se aplicam. Além disso, não há nenhuma outra alteração no suporte ao cliente da API REST do Marketo.

**Com quem podemos entrar em contato para obter suporte se estivermos integrados ao IMS?**

* Pré-migração de usuários: abra um caso de suporte na [Comunidade da nação de marketing](https://nation.marketo.com/t5/support/ct-p/Support) ou envie um email a `customercare@marketo.com`.

* Pós-migração de usuários: abra um caso de suporte na [Comunidade da nação de marketing](https://nation.marketo.com/t5/support/ct-p/Support) ou envie um email a `customercare@marketo.com`.

* Suporte pós-conclusão da migração: os administradores de suporte para produtos podem abrir casos por meio do portal de suporte da Experience League.

Se tiver o Ultimate Success, você tem acesso ao Admin Console Migration White Glove Service. Entre em contato com a equipe de conta da Adobe (o seu gerente de conta) para obter assistência.

**Se eu usar uma identidade da Adobe para acessar outros aplicativos da Adobe, posso usá-la para acessar o Marketo?**

Mesmo se você tiver outros produtos da Adobe, não poderá acessar o Marketo com a identidade da Adobe até que a assinatura seja migrada para o IMS.

**As funções de usuários do Marketo (em espaços de trabalho) são gerenciadas no Adobe Admin Console?**

Não. O gerenciamento de funções de usuários (em espaços de trabalho) é realizado no Marketo Engage.

**Sou um administrador do Marketo em uma assinatura integrada do IMS e não tenho acesso ao Admin Console. Como obtenho acesso?**

Qualquer administrador do sistema ou de produtos da Adobe que tenha acesso ao Admin Console da sua organização pode conceder-lhe acesso. Se você não tiver certeza de quem na sua organização tem privilégios de administrador no console, entre em contato com o [Atendimento ao cliente da Adobe](https://helpx.adobe.com/br/contact.html){target="_blank"}.

**Como um administrador adicionaria usuários ao Marketo [!DNL Sales Connect]?**

Embora exista um cartão de produto no Admin Console para o [!DNL Sales Connect], o Admin Console não deve ser usado para adicionar/gerenciar usuários. O link a seguir permite que administradores gerenciem usuários por meio do Marketo [!DNL Sales Connect]: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Onde posso obter mais informações sobre o Adobe Admin Console?**

[https://helpx.adobe.com/br/enterprise/admin-guide.html](https://helpx.adobe.com/br/enterprise/admin-guide.html){target="_blank"}.

**Ainda entro na seção do administrador no Marketo para fazer alterações na conta do usuário para a minha conta?**

Não, você precisaria navegar até [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Como isso funciona com o Universal ID do Marketo?**

Quem foi integrado à identidade da Adobe pode acessar todas as assinaturas habilitadas para o IMS de maneira contínua por meio do alternador de assinaturas no produto.

**Isso funciona com o SSO?**

Sim. A integração do Marketo com o Adobe IMS é compatível com usuários que usam o Universal ID e o SSO. Agora, o SSO é orientado pelo Adobe IMS e configurado no nível da organização no Adobe Admin Console. [Saiba mais aqui](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}.

**Já fui integrado à identidade da Adobe e agora quero implementar o SSO. O que faço?**

Se você quiser implementar o logon único e a sua assinatura tiver sido integrada à identidade da Adobe sem o SSO implementado na organização da Adobe, envie um tíquete ao [Suporte do Marketo](https://nation.marketo.com/){target="_blank"} e especifique o tópico como “Marketo no Admin Console, implementação do SSO”.

**Como funciona a autorização de dispositivos?**

No momento, o Adobe IMS não conta com nada parecido com o recurso de autorização de dispositivos do Marketo.

**Ainda é possível usar o recurso de “Fazer logon na caixa de diálogo Convidar usuário” para tornar o logon de um usuário exclusivo com base em seu email?**

Não. O fluxo de trabalho de convite de usuários não está mais ativo quando uma assinatura é habilitada para o IMS; portanto, o recurso não é mais válido. A identidade da Adobe exige que a identidade de um usuário esteja vinculada a seu email.

**Para o Adobe IMS, temos a opção de usar a Adobe ID, Enterprise ID ou Federated ID?**

Sim, você determina o tipo de identidade a ser permitido pela sua organização. Mais informações podem ser encontradas aqui: [Visão geral das identidades](https://helpx.adobe.com/br/enterprise/using/identity.html) e aqui: [Configurar identidade](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}.

**Quais cartões de produto são compatíveis com o Adobe Admin Console?**

Os cartões de produto compatíveis são: Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect e Marketo Sales Insight Actions.

**E se o meu logon de usuário não corresponder ao meu email quando eu migrar para a identidade da Adobe?**

Os usuários atuais do Marketo Engage com logons diferentes de seus endereços de email não farão mais logon com essa credencial depois de migrados para uma identidade da Adobe. As identidades da Adobe sempre são autenticadas com o endereço de email de um usuário. Você pode atualizar o endereço de email de uma identidade da Adobe em [account.adobe.com](https://account.adobe.com){target="_blank"}.

**O que acontece após a migração para a identidade da Adobe se a minha assinatura usa configurações de restrição de IP?**

As suas restrições de IP atuais permanecerão ativas até o primeiro trimestre de 2026 (isso se aplica às assinaturas para as quais estavam ativas antes da migração). Essas restrições também se aplicam aos usuários com Adobe ID; portanto, os seus controles de acesso continuarão funcionando conforme esperado.

A partir do primeiro trimestre de 2026, as restrições de IP herdadas serão desativadas. A partir desse ponto, o acesso baseado em IP é gerenciado exclusivamente no Adobe Admin Console (AAC). Para manter o acesso seguro, é necessário configurar as restrições de IP no AAC. Para obter mais informações, consulte esta [publicação do blog da nação de marketing](https://nation.marketo.com/t5/product-blogs/updated-important-update-ip-restrictions-feature-transition/ba-p/358420){target="_blank"}.

**O que acontece após a migração para a identidade da Adobe se eu tiver usuários com uma função com a opção de “Contornar logon único”?**

O Adobe Admin Console inclui um diretório padrão de IDs empresariais. Os usuários fora dos domínios reivindicados nos diretórios de Federated IDs em uma organização da Adobe são atribuídos a esse diretório com o tipo de identidade “Adobe ID”. Esses usuários podem acessar o Marketo Engage sem passar pelo logon único (SSO), e a propriedade da licença permanece com a empresa, não com os indivíduos.

**Tenho mais de uma assinatura, mas nem todas estão com o logon único habilitado. O que acontece após a migração para a identidade da Adobe?**

Quando as assinaturas são integradas à identidade da Adobe, o logon único (SSO, na sigla em inglês) é configurado no nível da organização da Adobe. Isso significa que o SSO se aplica a todas as instâncias de produtos na organização da Adobe. Quando o SSO estiver configurado, ele será aplicado a todas as instâncias do Marketo nessa organização da Adobe. Anteriormente, o Marketo permitia ajustar essa configuração no nível da instância. Isso não é permitido pelo Adobe Identity Management System.

**Há alguma alteração necessária para CNAMEs, SPF ou DKIM que usamos atualmente para o Marketo Engage após a migração para a identidade da Adobe?**

Não, não há nenhum impacto nessas configurações.

**Como posso evitar que as sessões atinjam o tempo-limite?**

Em [Configurações avançadas](https://helpx.adobe.com/br/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}, você pode personalizar a vida útil máxima da sessão desejada (são necessárias permissões de administrador do sistema). É recomendável estabelecer essa configuração após a migração do produto, mas antes da migração de usuários.

**Agora, preciso entrar na Experience Cloud para acessar o Marketo Engage. Há uma maneira de simplificar esse fluxo?**

Sim. Você pode criar um marcador do navegador do link iniciado depois de clicar no botão **Iniciar** na página de entrada da instância do Marketo Engage para ignorar essa página a partir de agora.

![](assets/faq-1.png)
