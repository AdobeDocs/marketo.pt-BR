---
description: Noções básicas sobre a assinatura do Marketo e a migração de usuários para o Adobe Admin Console - Documentação do Marketo - Documentação do produto
title: Noções básicas sobre assinatura do Marketo e migração de usuários para o Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: 179fe78c35c04617df47b61d88322f82feab746a
workflow-type: tm+mt
source-wordcount: '1323'
ht-degree: 0%

---

# Noções básicas sobre assinatura do Marketo e migração de usuários para o Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

O Adobe está aprimorando a forma como você gerencia as assinaturas e os usuários da Adobe Marketo Engage, aumentando a produtividade para você e para a sua organização. Como parte dessa alteração, o Adobe está migrando suas assinaturas de Marketo Engage e usuários para o Adobe Admin Console. Essa é uma migração necessária e não afetará nenhum fluxo de trabalho de marketing, conteúdo, integrações ou ativos.

Saiba como você pode usar o Adobe Admin Console para gerenciar os direitos de Adobe em toda a organização com o [Guia do administrador de equipes e empresas](https://helpx.adobe.com/br/enterprise/admin-guide.html){target="_blank"}.

## O que está mudando? {#what-is-changing}

Como parte da migração, sua assinatura e o gerenciamento de usuários passarão do aplicativo do Marketo para o Adobe Admin Console.

* **Os administradores do sistema gerenciarão assinaturas no Adobe Admin Console**. Veja todos os seus produtos Adobe em um único console.

* **Os administradores de produtos gerenciarão os usuários e seu acesso no Adobe Admin Console**. Adicione e remova usuários para todas as suas assinaturas Adobe.

* **Os usuários entrarão com a Identidade do Adobe**. O Adobe migrará os usuários existentes para o Adobe Admin Console. Os usuários farão logon nas assinaturas do Marketo usando sua nova Identidade de Adobe - seja um Adobe ID ou Adobe Federated ID (SSO).

* **Não há alterações na maneira como você gerencia todas as outras funcionalidades** no próprio aplicativo Marketo Engage, incluindo gerenciamento de recursos, funções de usuário, espaços de trabalho, funcionalidade e comportamento.

## Cronograma da Jornada de migração {#migration-journey-timeline}

Primeiro, o Adobe migrará suas assinaturas do Marketo Engage para o Adobe Admin Console e, em seguida, migrará todos os usuários existentes com endereços de email verificados. Se você for um Administrador do sistema ou um Administrador de produto do Marketo, receberá emails orientando sobre a jornada de migração. Esta é uma linha do tempo do que você pode esperar:

### Migração de assinatura concluída {#subscription-migration-complete}

Os administradores do sistema receberão um email quando a migração da assinatura para o Adobe Admin Console for concluída.

Os administradores de sistema podem precisar concluir algumas etapas necessárias antes de começar a migração do usuário para minimizar o impacto para os usuários do Marketo:

* Se seus usuários do Marketo atualmente fizerem logon com SSO, você precisará configurar o SSO no Adobe Admin Console para que seus usuários possam continuar a fazer logon com SSO. Se os usuários do Marketo não utilizarem o SSO no momento, mas você quiser configurá-lo no Adobe Admin Console, faça isso neste momento da jornada de migração.

* Se você já gerencia outros produtos Adobe no seu Adobe Admin Console, o Adobe pode solicitar seu consentimento para migrar automaticamente os usuários para o seu console existente. Clique no botão &quot;Introdução&quot; no email para navegar até a página de consentimento.

Não há alterações no gerenciamento de usuários no momento. Embora os produtos da Marketo apareçam no Admin Console, os administradores do Marketo continuarão a gerenciar usuários na área de administração do Marketo e os usuários continuarão a fazer logon com sua identidade da Marketo até que a migração de usuários seja concluída. Durante esse período, os produtos Marketo não podem ser administrados no Admin Console até que a migração do usuário comece. Isso inclui a instância de Dynamic Chat associada à assinatura.

>[!NOTE]
>
>Se você não usa SSO atualmente, mas está pensando em implementá-lo, sugerimos fazê-lo antes que a migração de usuário ocorra. Se você quiser implementar o Logon único e sua assinatura tiver sido integrada ao Adobe Identity sem o SSO implementado na Adobe Org, envie um tíquete para [Suporte ao Marketo](https://nation.marketo.com/){target="_blank"} e especifique o tópico como &quot;Marketo no Admin Console, implementação de SSO&quot;.

### Agendar migração de usuário {#schedule-user-migration}

Depois que o administrador do sistema concluir os pré-requisitos descritos na seção anterior, o Adobe agendará automaticamente a migração do usuário com 30 dias de antecedência e se comunicará com os administradores de produto da Marketo para gerenciar a migração do usuário.

Os administradores de produto do Marketo irão:

* Receba um e-mail com a data agendada de início da migração de usuário com 30 dias de antecedência.

* Obtenha acesso ao Console de migração do Marketo, localizado na área de Administração do Marketo, onde eles têm a opção de alterar a data de migração de uma assinatura.

>[!NOTE]
>
>Devido à complexidade da migração, as alterações de data são restritas a não mais de 30 dias além da data agendada. Enviar um email para `marketocares@marketo.com` se você precisar de uma data posterior.

* Consulte um banner em Meu Marketo exibindo uma contagem regressiva para a Data de início da migração do usuário.

* Receba um email de lembrete um dia antes da Data de início da migração do usuário.

### Dia de Preparação de Usuários para Migração {#prepare-users-for-migration-day}

Como administrador de produto do Marketo, é recomendável garantir que todos os usuários estejam preparados para o dia da migração.

* Marcar [verificação de email](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"} Status de todos os usuários na área de administração do Marketo. Incentive os usuários que não verificaram seus endereços de email a fazê-lo e ajude-os a resolver quaisquer desafios na conclusão do processo de verificação.

* Prepare todos os usuários para a migração futura para o Adobe Identity.

>[!NOTE]
>
>À medida que os usuários migram, eles recebem um email do Adobe notificando-os sobre a alteração na maneira como fazem logon no Marketo. Os usuários serão convidados a aceitar um convite para fazer logon usando a Identidade do Adobe pela primeira vez, seja fazendo logon com uma Adobe ID existente ou configurando uma nova com o mesmo endereço de email.

>[!IMPORTANT]
>
>Se um usuário do Marketo Engage não verificar seu endereço de email, ele não será migrado para uma Adobe ID e perderá o acesso à assinatura do Marketo após a conclusão da migração para a assinatura. Para recuperar o acesso, um administrador de produto do Marketo precisaria adicioná-los como um novo usuário.

### O que esperar no dia da migração {#what-to-expect-on-migration-day}

Todas as assinaturas do Marketo com fuso horário dos EUA serão migradas a partir da meia-noite, hora padrão do Pacífico, da data de início da migração. A migração de usuário para todas as outras assinaturas começará à meia-noite do fuso horário especificado da assinatura.

**O Adobe migra automaticamente os administradores do Marketo primeiro**. Quando os administradores do Marketo migrarem para a Identidade do Adobe, eles receberão a função de administrador de produto do Adobe no aplicativo do Marketo, juntamente com quaisquer outras funções que tenham tido anteriormente.

**Se sua assinatura do Marketo tiver menos de 75 usuários e não tiver SSO no Marketo e/ou em sua Adobe Org**, o Adobe migrará automaticamente o restante dos usuários. Esse fluxo de trabalho tem como objetivo fornecer o mais alto nível de automação para minimizar a sobrecarga para os usuários do Adobe Marketo. Nenhuma ação da sua parte é necessária para executar a migração.

**Se sua assinatura do Marketo tiver mais de 75 usuários ou tiver SSO no Marketo e/ou em sua Adobe Org**, os Administradores de produtos da Marketo terão acesso à área Migração de usuários de autoatendimento do Console de migração do Marketo, localizada na área de Administração do Marketo. Para aqueles que precisam de maior controle durante o processo de migração do usuário, os administradores de produto do Marketo poderão começar a selecionar usuários para migrar em lotes ou todos de uma só vez. Depois que os usuários são selecionados, os administradores têm a opção de &quot;Migrar agora&quot; ou &quot;Agendar migração&quot; para uma data posterior, proporcionando aos administradores o máximo de flexibilidade e controle sobre quais usuários são migrados quando.

>[!NOTE]
>
>Não haverá perda de acesso ao produto durante a migração do usuário. Se um usuário fizer logon durante o tempo em que for migrado, ele será desconectado e receberá uma solicitação para fazer logon novamente em minutos usando a Identidade do Adobe após a conclusão da migração.

À medida que os usuários são migrados, eles recebem um email do Adobe notificando-os sobre a alteração na maneira como fazem logon no Marketo. Os usuários serão convidados a aceitar um convite para fazer logon usando a Identidade do Adobe pela primeira vez, seja fazendo logon com uma Adobe ID existente ou configurando uma nova Adobe ID usando o mesmo endereço de email.

Mais informações podem ser encontradas em [Migrar para a identidade do Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}, [User Sign-in with Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}, and [Adobe Identity Management FAQ](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

## Migração de usuário concluída {#user-migration-complete}

O Adobe notificará todos os administradores de sistema e administradores de produto por email depois que todos os administradores e usuários forem migrados. No momento, todos os usuários da Marketo para essa assinatura farão logon no Marketo usando a Identidade do Adobe, e os Administradores de produto gerenciarão os usuários somente no Adobe Admin Console.

## Obter suporte {#get-support}

Para obter suporte adicional em relação à sua assinatura ou migração de usuário, envie um email para `marketocares@marketo.com`.

>[!MORELIKETHIS]
>
>* [Migrar para a identidade do Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}
>* [Logon do usuário com o Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}
>* [Perguntas frequentes sobre o Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}
