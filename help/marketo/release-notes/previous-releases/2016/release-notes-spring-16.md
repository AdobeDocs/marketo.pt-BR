---
unique-page-id: 11370952
description: Notas de versão - Segundo trimestre de 2016 - Documentação do Marketo - Documentação do produto
title: Notas de versão - primavera de 2016
exl-id: 0ca26acf-2ac2-418e-bc4e-9820f483fa71
source-git-commit: 4fa7e733a824af8d2fc0e3ba824b25f9bb985ccf
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Notas de versão: primavera de 16 {#release-notes-spring}

Os seguintes recursos estão incluídos na versão da primavera de 16. Clique nos links de título para exibir artigos detalhados para cada recurso.

## [Email Insights](/help/marketo/product-docs/reporting/email-insights/email-insights-overview.md) {#email-insights}

Email Insights é uma experiência totalmente nova de análise de email de dados agregados históricos — reprojetada de ponta a ponta para desempenho ultrarrápido como parte do Projeto Orion. Ele apresenta um design de interface do usuário completamente novo otimizado para atender às necessidades e ao fluxo de trabalho dos profissionais de marketing por email.

>[!NOTE]
>
>Estamos lançando o Email Insights para clientes em lotes, a partir de 3 de junho. Nosso objetivo é completar isso nos próximos meses. Você será notificado por email quando estiver habilitado.

![](assets/two.png)

## [Seletor de modelos de e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-picker-overview.md) {#email-template-picker}

Crie belos emails usando nossos novos Modelos iniciais! Além disso, localize rapidamente seus modelos a partir das miniaturas em tempo real.

>[!NOTE]
>
>O Editor de email 2.0 (com o Seletor de modelos) será lançado gradualmente a partir de 3 de junho. Concluiremos a implantação até 30 de junho. Ao contrário do Email Insights, você não será notificado quando tiver acesso. Para ver se o faz, siga as etapas em [este artigo](/help/marketo/product-docs/email-marketing/general/email-editor-2/transitioning-to-email-editor-2-0.md).

![](assets/5-29-home-starter-templates.png)

## [Edição de email - recriado](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-editing-re-imagined}

Isso mesmo, um novo editor de email! Use a funcionalidade leve de arrastar e soltar para adicionar e reordenar o conteúdo. Novos elementos, incluindo imagens, vídeos, variáveis e módulos, certamente melhorarão sua experiência de edição. Verifique também o editor de código, o pré-visualizador e o suporte de pré-cabeçalho atualizados.

![](assets/17a-29-modules-next.png)

## [Mensagens no aplicativo móvel](/help/marketo/product-docs/mobile-marketing/in-app-messages/understanding-in-app-messages.md) {#mobile-in-app-messages}

Crie mensagens impressionantes no aplicativo para seu aplicativo diretamente no Marketo. Defina exatamente quem deve vê-la e quando com o programa de mensagens no aplicativo. Monitore facilmente seu desempenho com o painel do programa.

![](assets/pasted-image-at-2016-05-24-09-45-am.png)

## [Nenhum trecho de rascunho](/help/marketo/product-docs/administration/users-and-roles/enable-no-draft-for-snippets.md) {#no-draft-snippets}

Foram-se os dias em que você precisa reaprovar tudo sempre que um trecho for atualizado! Com o Sem rascunho, todos os emails e landing pages que usam um trecho receberão as atualizações do trecho e manterão seus status anteriores. Cada vez que aprovar um trecho, você terá a opção de executar Sem rascunho e atualizar tudo ou criar rascunhos. Depende de você! O recurso Sem rascunho estará disponível para todos os clientes e será controlado por uma nova permissão no Administrador.

![](assets/image2016-5-16-15-3a41-3a17.png)

## [Página de aterrissagem, modelo de página de aterrissagem e APIs de formulário](https://developers.marketo.com/blog/spring-2016-updates/) {#landing-page-landing-page-template-and-form-apis}

As APIs REST do Marketo agora oferecem suporte ao controle sobre páginas de aterrissagem, modelos de páginas de aterrissagem e formulários do Marketo. Agora os usuários podem criar, atualizar conteúdo, aprovar e excluir esses ativos diretamente por meio da API REST do Marketo.

## [INCLUIR NA LISTA DE PERMISSÕES IP para acesso à API](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md) {#ip-allowlisting-for-api-access}

Semelhante ao recurso de incluir na lista de permissões de IP para logons de usuário do Marketo, os administradores do Marketo agora podem configurar um incluo na lista de permissões de endereços IP que podem acessar as APIs SOAP e REST do Marketo, bloqueando o acesso de endereços IP não autorizados. Isso fornece uma camada adicional de segurança para a instância do Marketo e garante que o acesso à API só possa ocorrer de dentro da rede da organização. Detalhes sobre como configurar isso estão disponíveis no [Site de documentação do Marketo](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md).

## [Novo Conector de sincronização do Microsoft Dynamics de alta velocidade](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#new-high-speed-microsoft-dynamics-sync-connector}

Construído sobre a arquitetura Orion, o novo conector do Dynamics de alta velocidade fornece velocidades até 20 vezes mais rápidas para a sincronização inicial e até 5 vezes mais rápidas para a sincronização incremental. Todos os novos clientes serão integrados a esse conector na data de lançamento e, gradualmente, o implantaremos para os clientes existentes durante o período de lançamento do verão.

**Atualizar dados para novos campos**: agora você pode habilitar novos campos de sincronização a qualquer momento, e todos os valores de dados para esse campo serão atualizados do Dynamics CRM para o Marketo. Não há mais preocupações sobre a necessidade de selecionar todos os campos durante a configuração inicial. Se você desabilitar um campo de sincronização existente e reabilitá-lo posteriormente, todos os valores de dados desse campo serão atualizados do Dynamics CRM para o Marketo.

**Sincronizar Cliente Potencial como Contato**: a ação de fluxo Sincronizar cliente potencial com o Microsoft tem uma nova opção para sincronizar como um cliente potencial ou contato.

![](assets/image2016-5-19-8-3a59-3a9.png)

**Guia Admin de Erros de Sincronização**: Procurar, pesquisar ou exportar clientes potenciais (e outros objetos) que apresentaram falha na sincronização com detalhes como operação, direção, código de erro e mensagem de erro.

![](assets/sync-errors.png)

**Microsoft Dynamics 2016**: o Conector é totalmente certificado para as versões Online e No local do Dynamics 2016.

**As atualizações de plug-ins agora estão documentadas:** Consulte a [artigo documentos de atualizações do plug-in](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md).

## [Nome amigável da instância](/help/marketo/product-docs/administration/settings/edit-subscription-settings.md) {#friendly-instance-name}

Hoje, é difícil diferenciar entre instâncias do Marketo, por exemplo, instâncias de sandbox e produção. Esse recurso permite saber em quais instâncias você está trabalhando atualmente.

![](assets/image2016-5-16-15-3a57-3a14.png)

## [Acesso limitado por tempo para assinaturas](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md) {#limited-time-access-for-subscriptions}

Hoje, os usuários são convidados a assinar o Marketo por um período indefinido. Esse recurso permite que administradores convidem usuários para assinaturas por um período de tempo limitado, por exemplo, 2 semanas ou 1 mês.

![](assets/image2016-5-16-15-3a59-3a52.png)

## [Grade de Objetos Personalizados](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) {#custom-objects-grid}

Agora é possível exibir o número de registros e campos de todos os objetos personalizados publicados.

![](assets/custom-objects-grid.png)

## Atividades personalizadas {#custom-activities}

Agora, os administradores do Marketo podem definir e gerenciar seus tipos de atividades personalizadas por meio do Marketo Custom Activity Definition Modeler. Semelhante ao Modelador de objeto personalizado do Marketo (e em conjunto com ele), os administradores agora podem estender o modelo de dados para atender às suas necessidades comerciais exatas. Detalhes sobre como usar essa funcionalidade estão disponíveis no [Site de documentação do Marketo](/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md).
