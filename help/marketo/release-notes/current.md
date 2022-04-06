---
description: Current Release Notes - Marketo Docs - Product Documentation
title: Notas de versão atuais
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 2ac0ef0b715eb2acd03fe2c5ad4cfee8daeef4f6
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Notas de versão: Maio de 2022 {#release-notes-may-22}

Abaixo você encontrará todos os recursos incluídos na versão de 22 de maio. Verifique sua edição do Adobe Marketo Engage para ver a disponibilidade dos recursos.

>[!AVAILABILITY]
>
>Recursos indicados por uma estrela (![star](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante de Marketo Engage para saber mais.

**_Versões trimestrais_**

The following features will start to be released on **May 6, 2022**, with a phased rollout of remaining features over the subsequent weeks (unless specified otherwise).

## Integração de CRM nativo {#native-crm-integration}

**Integração de Veva Nativa ao CRM (disponibilidade limitada)**: Melhore o envolvimento com os profissionais de saúde sincronizando a atividade entre o VRM Veeva e o Marketo Engage por meio da integração nativa. Essa integração permite que os profissionais de marketing criem experiências mais personalizadas e contínuas entre canais para os profissionais de saúde. Please contact your Customer Success Manager if you&#39;re interested in participating.

## Orquestração entre canais {#cross-channel-orchestration}

**Eventos de chatbot para chat dinâmico**: Utilize dados de comportamento mais detalhados para visitantes da Web, como tempo na página, tempo no site e porcentagem de rolagem da página para definir quando uma caixa de diálogo de bate-papo deve ser exibida.

**Incorporar PDF para bate-papo dinâmico**: Aumente o engajamento e compartilhe conteúdo significativo incorporando PDF às caixas de diálogo de bate-papo e meça o desempenho do conteúdo por meio do rastreamento da atividade de engajamento.

**Extended Language Support for Dynamic Chat**: The Dynamic Chat user interface will now also be available in French, German, Japanese, Portuguese, and Spanish. Chat dialogues can also be configured in these languages.

**Excluir URLs para bate-papo dinâmico**: Controlar em quais de suas páginas da Web o Dynamic Chat é exibido com a capacidade de excluir URLs específicos dos critérios de direcionamento.

**Email Bot Activity Filtering Enhancements**: Continue to protect the health of your database with the ability to identify bot behavior based on hidden link User Agents or IPs and proximity patterns, in addition to the existing IAB list match identification. Visualize estatísticas de atividades de bot que permitem compreender o número de atividades de bot identificadas para cada tipo.

**Cabeçalho STS para links de rastreamento de email**: Atender às práticas recomendadas de segurança com a capacidade de aplicar cabeçalhos de Segurança de Transporte Seguro para garantir que o tráfego para links rastreados seja sempre seguro.

## Experiência da próxima geração {#next-generation-experience}

**Toggle Switch Defaulted to the Next-Generation Experience**: The toggle switch will be default to the new experience in all screens where it&#39;s available, making it easier for users to discover the updated designs and usability enhancements.

**Updated Screen in the Next-Generation Experience**:

Estamos fornecendo a Exibição de detalhes do modelo de email no Design Studio na experiência da próxima geração, oferecendo melhorias atualizadas de design e usabilidade acessíveis por meio do switch de alternância.

## Automação de experiência {#experience-automation}

**Self-Service Flow Steps (continued beta)**: Expand connectivity between Marketo Engage and the rest of your stack with the ability to author customized flow steps for use in Smart Campaigns. Os usuários e parceiros do Marketo Engage podem aproveitar essa funcionalidade para permitir o uso de serviços da Web externos em campanhas acionadoras, em lote e executáveis (em contraste com webhooks que só podem ser usados em campanhas acionadoras).

## Melhorias da API {#api-enhancements}

* **Acesso à API expandido para assinaturas ativadas por CRM**: Estamos expandindo o acesso à API para assinaturas que têm uma sincronização de CRM ativada para permitir que os usuários recuperem empresas, oportunidades e pessoas de vendas do Marketo Engage.
* **Suporte para tipos de dados &quot;ocultos&quot; no Forms**: Fornece a capacidade de gerenciar campos de formulário ocultos por meio da API.
* **Oferece suporte a valores de comparação múltiplos para isNot Form via Rules**: Gerencie a visibilidade de campos de formulário com base no fato de o valor de outro campo não ser um dos valores em uma determinada lista.
* **Permitir configuração de Exibir e Valores Enviados em Selecionar Listas Separadamente**: Defina o valor de exibição e o valor enviado em um campo separadamente. For example, show the name of a hotel, but submit an Internal ID to the backend.
* **Permitir configuração de desativação do rastreamento aberto ao criar ou atualizar email**: Crie um email com o rastreamento aberto desativado.

## Anúncios {#announcements}

**Verificação de email e exclusividade**: A partir de abril, a implementação da Verificação de email será iniciada. At that point, Marketo Engage user email addresses will require verification and uniqueness (this does not apply to API-only users). Directory service authenticated users will automatically have their emails verified when their subscription is enabled with Email Verification.

Email Verification for subscriptions using the “Login in Invite User Dialog” feature or that have a single email associated with multiple users will coincide with the May release. Subscriptions that have a single email associated with multiple users will be enabled with Email Verification and will require those users to resolve the conflict and use a unique email per user. When the ‘Login in Invite User Dialog’ feature is enabled, users invited via this feature will need to have a unique email address. For API-only users invited via this feature, the email address does not need to be unique.

**_Webinar da versão do produto_**

Junte-se a nós em 11 de maio de 2022, às 9h PT / 12h ET para um [webinário ao vivo](https://engage.marketo.com/2022_March_May_Release_Webinar_RegistrationPage.html){target=&quot;_blank&quot;} hospedado pela nossa equipe de produtos, onde você pode aprender a usar todas as inovações de produtos mais recentes.
