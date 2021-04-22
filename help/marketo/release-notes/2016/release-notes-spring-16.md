---
unique-page-id: 11370952
description: Notas de versão - Primeiro trimestre de 2016 - Documentos da Marketo - Documentação do produto
title: Notas de versão - Primavera de 16
exl-id: 0ca26acf-2ac2-418e-bc4e-9820f483fa71
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# Notas de versão: Primavera &#39;16 {#release-notes-spring}

Os seguintes recursos estão incluídos na versão do primeiro trimestre de 16. Clique nos links de título para exibir os artigos detalhados de cada recurso.

## [Email Insights](/help/marketo/product-docs/reporting/email-insights/email-insights-overview.md) {#email-insights}

O Email Insights é uma nova experiência histórica de análise de email de dados agregados — reprojetada e completa para proporcionar um desempenho extremamente rápido como parte do Project Orion. Ele apresenta um design de interface do usuário totalmente novo e otimizado para atender às necessidades e ao fluxo de trabalho dos profissionais de marketing de email.

>[!NOTE]
>
>Estamos lançando o Email Insights para os clientes em lotes, a partir de 3 de junho. Nosso objetivo é concluir isso nos próximos meses. Você será notificado por email quando estiver habilitado.

![](assets/two.png)

## [Seletor de modelos de e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-picker-overview.md) {#email-template-picker}

Crie belos emails usando nossos novos Modelos iniciais! Além disso, localize rapidamente seus modelos a partir de suas miniaturas ativas.

>[!NOTE]
>
>O Editor de email 2.0 (com o Seletor de modelo) será lançado gradualmente a partir de 3 de junho. Concluiremos o lançamento até 30 de junho. Ao contrário do Email Insights, você não será notificado quando tiver acesso. Para ver se o faz, siga as etapas em [this article](/help/marketo/product-docs/email-marketing/general/email-editor-2/transitioning-to-email-editor-2-0.md).

![](assets/5-29-home-starter-templates.png)

## [Edição de email — recriação de imagens](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-editing-re-imagined}

É isso mesmo, um novo editor de email! Use a funcionalidade leve de arrastar e soltar para adicionar e reordenar o conteúdo. Novos elementos, incluindo imagens, vídeos, variáveis e módulos, certamente melhorarão sua experiência de edição. Além disso, verifique o editor de código atualizado, visualizador e suporte ao pré-cabeçalho.

![](assets/17a-29-modules-next.png)

## [Mensagens no aplicativo móvel](/help/marketo/product-docs/mobile-marketing/in-app-messages/understanding-in-app-messages.md) {#mobile-in-app-messages}

Crie mensagens impressionantes no aplicativo para seu aplicativo diretamente no Marketo. Defina exatamente quem deve vê-lo e quando com o programa de mensagens no aplicativo. Monitore facilmente seu desempenho com o painel do programa.

![](assets/pasted-image-at-2016-05-24-09-45-am.png)

## [Sem trechos de rascunho](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/enable-no-draft-for-snippets.md) {#no-draft-snippets}

Foram-se os dias em que você precisa aprovar novamente tudo sempre que um trecho é atualizado! Com a opção Sem rascunho, todos os emails e landing pages usando um trecho receberão as atualizações do trecho e manterão seus status anteriores. Cada vez que você aprovar um trecho, terá a opção de executar Sem rascunho e atualizar tudo ou criar rascunhos. Cabe a você! O Sem rascunho estará disponível para todos os clientes e será controlado por uma nova permissão em Administração.

![](assets/image2016-5-16-15-3a41-3a17.png)

## [Página de aterrissagem, Modelo de página de aterrissagem e APIs de formulário](https://developers.marketo.com/blog/spring-2016-updates/) {#landing-page-landing-page-template-and-form-apis}

As APIs REST do Marketo agora oferecem suporte ao controle de páginas iniciais, modelos de páginas de aterrissagem e formulários do Marketo. Agora os usuários podem criar, atualizar o conteúdo, aprovar e excluir esses ativos diretamente da API REST do Marketo.

## [INCLUIR NA LISTA DE PERMISSÕES IP para acesso à API](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md) {#ip-allowlisting-for-api-access}

Semelhante ao recurso de  de IP incluir na lista de permissões para logons de usuários da Marketo, os administradores da Marketo agora podem configurar uma lista de permissões de endereços IP que podem acessar as APIs SOAP e REST da Marketo, bloqueando o acesso de endereços IP não autorizados. Isso fornece uma camada adicional de segurança para a instância do Marketo e garante que o acesso à API só possa ocorrer a partir da rede da organização. Detalhes sobre como configurar isso estão disponíveis no [site de documentação do Marketo](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md).

## [Novo Microsoft Dynamics Sync Connector de Alta Velocidade](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#new-high-speed-microsoft-dynamics-sync-connector}

Construído na arquitetura do Orion, o novo conector de dinâmica de alta velocidade fornece velocidades até 20 vezes mais rápidas para sincronização inicial e até 5 vezes mais rápidas para sincronização incremental. Todos os novos clientes serão integrados a esse conector na data de lançamento e nós o implementaremos gradualmente aos clientes existentes durante o período de lançamento do verão.

**Atualizar dados para novos campos**: Agora é possível ativar novos campos de sincronização em qualquer momento e todos os valores de dados para esse campo serão atualizados do Dynamics CRM para o Marketo. Não há mais preocupações sobre a necessidade de selecionar todos os campos durante a configuração inicial. Se você desativar um campo de sincronização existente e reativá-lo posteriormente, todos os valores de dados para esse campo serão atualizados do Dynamics CRM para o Marketo.

**Sincronizar lead como contato**: A ação de fluxo Sincronizar lead para a Microsoft tem uma nova opção para sincronizar como um lead ou contato.

![](assets/image2016-5-19-8-3a59-3a9.png)

**Guia Admin** de Erros de Sincronização: Pesquise, pesquise ou exporte leads (e outros objetos) que não foram sincronizados com detalhes como operação, direção, código de erro e mensagem de erro.

![](assets/sync-errors.png)

**Microsoft Dynamics 2016**: O Connector é totalmente certificado para as versões online e local do Dynamics 2016.

**As atualizações de plug-in agora estão documentadas:** consulte o artigo sobre atualizações de  [plug-in nos documentos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md).

## [Nome da Instância Amigável](/help/marketo/product-docs/administration/settings/edit-subscription-settings.md) {#friendly-instance-name}

Hoje, é difícil diferenciar entre instâncias do Marketo, por exemplo, sandbox e instâncias de produção. Esse recurso permite saber em quais instâncias você está trabalhando no momento.

![](assets/image2016-5-16-15-3a57-3a14.png)

## [Acesso por tempo limitado para assinaturas](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md) {#limited-time-access-for-subscriptions}

Atualmente, os usuários são convidados para a assinatura da Marketo por um período indefinido. Esse recurso permite que os administradores convidem usuários para assinaturas por um período limitado, por exemplo, 2 semanas ou 1 mês.

![](assets/image2016-5-16-15-3a59-3a52.png)

## [Grade de Objetos Personalizados](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) {#custom-objects-grid}

Agora, é possível exibir o número de registros e campos para todos os objetos personalizados publicados.

![](assets/custom-objects-grid.png)

## Atividades personalizadas {#custom-activities}

Agora, os administradores do Marketo podem definir e gerenciar seus tipos de atividade personalizados por meio do modelador de Definição de atividade personalizada do Marketo. Assim como (e em conjunto com) o Marketo Custom Object Modeler, os administradores agora podem estender o modelo de dados para atender às necessidades exatas dos negócios. Detalhes sobre como usar essa funcionalidade estão disponíveis no [site de documentação do Marketo](/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md).
