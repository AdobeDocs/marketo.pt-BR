---
title: 2019
description: 2019 - Documentação do Marketo - Documentação do produto
feature: Release Information
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
  - id: de9e3aa9-f002-4fe1-897b-09ee3c55114b
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
  - id: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: bbbea26f-9621-49eb-9ab8-e06fb3bbce8c
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 4d4669f3239b43afbcbd660644c8d1a35734a556
workflow-type: tm+mt
source-wordcount: 2528
ht-degree: 3%

---

# 2019

## Inverno de 2019 {#winter}

Os seguintes recursos estão incluídos na versão Winter &#39;19. Verifique a edição do Marketo quanto à disponibilidade de recursos.

Clique nos links de título para exibir artigos detalhados para cada recurso, se disponíveis.

>[!NOTE]
>
>O [!DNL Facebook] agora exige uma conta do Business Manager para aproveitar sua integração com o Público-alvo personalizado. Seu [!DNL Facebook] serviço LaunchPoint *deve* estar associado a uma conta do Business Manager ou **sua integração não funcionará mais após 14 de janeiro de 2019**. Para configurar uma conta do Business Manager, consulte a [[!DNL Facebook] Ajuda](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>A Microsoft está enviando todos os clientes online para a atualização para a versão mais recente do [!DNL Microsoft Dynamics]. Se você estiver integrando sua instância do Marketo com o [!DNL Dynamics Online], será necessário [atualizar para a versão mais recente da Solução da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) antes de **31 de janeiro de 2019** para garantir que sua integração continue funcionando.

>[!NOTE]
>
>O Marketo está atualizando a versão do OAuth para o GoToWebinar de 1.0 para 2.0. O suporte para OAuth 1.0 será descontinuado em janeiro de 2019. Se você for um cliente do GoToWebinar, precisará autenticar novamente seus logons por meio do LaunchPoint (na área de Administração) até **31 de janeiro de 2019** para garantir que sua integração continue funcionando. Para obter mais detalhes, consulte nossa [página da Comunidade](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Melhorias da plataforma principal {#core-platform-enhancements}

**[Email CC para emails do Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Inclua até cinco endereços por destinatário para CC nos e-mails enviados através do Marketo.

**API**

* **Suporte a domínio de várias marcas para a API de ativos:** Aprovar e clonar ativos produz os mesmos resultados na API e na interface.
* **Suporte de email CC para a API de ativos**: os usuários que clonam, aprovam e processam emails por meio da API manterão a paridade com as configurações da interface do usuário.

**[[!DNL Munchkin] v155 (Beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Modo Somente API**: os usuários agora podem determinar quando e como rastrear membros de seus bancos de dados, permitindo que aplicativos Web de página única façam chamadas explicitamente quando quiserem gravar uma visita de página da Web, em vez de depender do rastreamento automático do Marketo.
* **Gerenciamento de recusa**: gerencie facilmente recusas combinando o domínio do cookie de recusa com o domínio do cookie de rastreamento [!DNL Munchkin].
* **Parâmetro de Decisor de Nível de Domínio**: domínios de duas letras (ou seja, &quot; [website.io](https://website.io)&quot;) rastrearão automaticamente no Marketo sem requisitos de configuração adicionais.

## Marketo Sales Engage {#marketo-sales-engage}

* **[!DNL Salesforce]Perfil Personalizado**: o Sales Engage agora oferece suporte a perfis personalizados ilimitados.

* **[!DNL Salesforce]Personalização**: ao remover campos de atividade personalizados não críticos, os usuários podem configurar o Sales Engage na plataforma de CRM com mais eficiência.
* **Serviço de Email**: aproveite uma melhor capacidade de entrega, além de melhor rastreamento de respostas, funcionalidade de email agendado e funcionalidade de email em massa conectando-se ao [!DNL Microsoft Outlook] (pelo Office365 ou no local, pela guia Conexão de Email).
* **Novas Configurações de Administrador**: Duas páginas de administrador foram adicionadas para otimizar sua instância do Sales Engage

   * O *Gerenciamento de Equipe* dá suporte a um processo de configuração de conta simples permitindo que os administradores editem assinaturas e equipes.
   * As *Configurações de administração do Salesforce* ajudam as equipes a configurar a sincronização do SFDC de forma mais rápida e fácil do que nunca.

* **Plug-in do OWA para[!DNL Windows]**: com um único suplemento, todos os clientes do [!DNL Windows Office365] terão suporte no Sales Engage, fornecendo a capacidade de usar o Feed Ativo no Outlook. O novo plug-in estará disponível na Microsoft Store.
* **Pusher de atividades**: sincronizar o Sales Engage com a plataforma principal do Marketo para aproveitar os insights de marketing em tempo real.

## [!DNL Marketo Sky] {#marketo-sky}

>[!NOTE]
>
>As versões do [!DNL Marketo Sky] ocorrem com mais frequência. Os seguintes recursos e aprimoramentos devem ser lançados no final do quarto trimestre/início do primeiro trimestre. Para obter mais detalhes e atualizações, consulte nossa [documentação da Sky](https://help.marketo.com/).

* **Experiência padrão opcional**: os usuários do Marketo podem definir [!DNL Marketo Sky] como sua experiência padrão se tiverem recebido acesso de um Administrador.

* **Minha Marketo recriada**: personalize sua experiência adicionando widgets que forneçam informações críticas, notificações e links para suas áreas visitadas com mais frequência.

* **Exibições de lista e páginas de detalhes do Design Studio**: aproveite um nível aumentado de organização e precisão com exibições de lista filtráveis e pesquisáveis de emails, páginas de aterrissagem e formulários. As Páginas de detalhes do ativo fornecem informações importantes sobre cada ativo, incluindo quais programas o ativo é usado, o número de snippets que estão sendo usados e muito mais.

* **Pesquisa global**: a Marketo agora oferece uma função de pesquisa global mais rápida e robusta em toda a plataforma. As consultas de pesquisa agora são executadas em todos os espaços de trabalho acessíveis e podem pesquisar ativos (ativos e arquivados), rótulos, campanhas e programas. Os resultados da pesquisa são fornecidos por meio de uma sobreposição e cada resultado inclui sua trilha de localização de arquivo para especificar onde o ativo está.

* **Interface do Usuário Aprimorada**: Novos ícones, modais e botões, além de uma nova paleta de cores para refletir a atualização de nossa marca e tornar o [!DNL Marketo Sky] ainda mais impressionante e funcional.

* **Aprimoramentos na Usabilidade do Programa de Email**: continuamos a avançar para a paridade na funcionalidade do Programa de Email entre nossa plataforma clássica de Gerenciamento de Cliente Potencial do Marketo e a nova experiência [!DNL Marketo Sky].
* **Programas Event-With-Webinar**: os programas Event-With-Webinar agora estão disponíveis em [!DNL Marketo Sky] (observação: somente GoToWebinar terá suporte nesta versão, com mais integrações estabelecidas ao longo do tempo).

## Marketing baseado em contas {#account-based-marketing}

**[Segmentação e filtragem com base em persona do ABM](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personalize suas campanhas do ABM para personalidades específicas em contas nomeadas. O recurso Persona ABM cria um título de cargo padrão com base na segmentação de clientes potenciais e permite a configuração de segmentações de persona adicionais.

## Analytics {#analytics}

**[!DNL Bizible]**

* **Campos Calculados Personalizados**: Use qualquer atributo [!DNL Bizible] para criar campos personalizados que possam ser usados para segmentação e relatórios do painel.

* **Certificação SOC II de Tipo II**: a nova certificação de segurança e privacidade se baseia na capacitação de Tipo I do início deste ano.

## [!DNL Web Personalization] {#web-personalization}

**[Adicione subdomínios nas configurações de conta](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Para gerenciar domínios e subdomínios com mais eficiência, os usuários agora podem adicionar subdomínios às configurações de conta RTP.

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**O MME Software Development Kit (SDK) para Android foi atualizado**

Atualizamos nosso SDK for Android para uma estrutura mais moderna, estável e escalável, que contém mais flexibilidade e novos recursos de engenharia. Os desenvolvedores de aplicativos do Android agora podem usar diretamente o [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) da Google com este novo SDK.

* [Instruções para o desenvolvedor](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Perguntas frequentes do desenvolvedor](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Os desenvolvedores de aplicativos **devem** atualizar para a nova versão antes de 31 de março de 2019. Se você não atualizar seu SDK até 31 de março de 2019, qualquer novo usuário que baixar seu aplicativo após essa data não poderá receber notificações por push até que você atualize para a versão mais recente do SDK. A atualização do SDK não exigirá que os usuários atuais do aplicativo móvel baixem novamente uma nova versão do aplicativo.

## Atualizações adicionais {#additional-updates}

**Plataforma de webinário extensível**

Além do lançamento de nosso produto, nossa equipe de parceiros está trabalhando em uma nova estrutura que permite que os provedores de webinários criem e mantenham suas próprias integrações com o Marketo, fornecendo mais flexibilidade na atualização e no aprimoramento de suas soluções, além de permitir que os profissionais de marketing aproveitem ao máximo as integrações escolhidas.

Planejamos lançar nossa nova plataforma com provedores caso a caso. Para obter mais informações, consulte os [detalhes do programa](https://www.marketo.com/why-marketo/partners/technology/) ou entre em contato com o seu contato da Marketo.

## Segundo trimestre de 2019 {#spring}

Os seguintes recursos estão incluídos na versão da primavera de 19. Verifique a edição do Marketo quanto à disponibilidade de recursos.

Clique nos links de título para exibir artigos detalhados para cada recurso, se disponíveis.

***Versões Trimestrais_**

Os recursos a seguir foram lançados em 15 de março de 2019.

## Melhorias da plataforma principal {#core-platform-enhancements}

* **Lista de espera:** Novo status de programa/evento para lista de espera de um membro quando você deseja [colocá-los em espera](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md) até que uma vaga seja aberta. Isso se aplica aos canais associados aos programas de Eventos no Marketo Classic, e aos programas de Eventos e Eventos com Webinar no [!DNL Marketo Sky]. Por padrão, Lista de espera tem o mesmo valor de etapa que Registrado.
* **[Limite de Comunicação Personalizado](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md)**: Agora os administradores podem definir limites de comunicação diários ou semanais personalizados.
* **[APIs de ativos de campanha inteligente](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**: enriqueça sua análise fora do Marketo com a recuperação de registros de campanha inteligente por data e ID atualizadas.
* **Links de Rastreamento HTTPS para Email:** Para clientes que compraram &quot;Domínios Seguros para Links de Rastreamento&quot;, os links de rastreamento com marca agora podem ser exibidos em seus emails como HTTPS.
* **Atualizações do Powerpack de Entrega de email**: capacidade de sinalizar e comentar sobre resultados de teste específicos, compartilhar resultados com as partes interessadas por meio de uma URL e rastrear alterações para ver a evolução de um email à medida que as partes interessadas editam o conteúdo.

Marketing baseado em contas

**[AccountAI](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md)** Agora disponível. O recurso AccountAI emprega inteligência artificial para revelar as contas que você deve objetivar em sua estratégia de ABM.

<br> 

**_Versões Não Trimestrais_**

Espera-se que os seguintes recursos sejam lançados ao longo do primeiro trimestre e no início do segundo trimestre de 2019.

## [!DNL Marketo Sky] {#marketo-sky}

* **Funcionalidade completa do programa de email**: envie emails, crie testes A/B e acompanhe os resultados em uma experiência simples.
* **Funcionalidade do Smart Campaign**: aproveite a estabilidade aprimorada em uma nova interface de usuário, já que a funcionalidade do Smart Campaign continua sendo lançada no Sky.
* **Gerenciar o Design Studio Assets**: adição da capacidade de gerenciar Modelos, Imagens, Forms, Trechos, Arquivos, Emails e Páginas de Aterrissagem em massa a partir das exibições de lista do Design Studio.
* **Entregar no Painel de Fuso Horário do Destinatário**: entenda o comportamento do cliente com relatórios para emails enviados usando o recurso Entregar no Fuso Horário do Destinatário no Sky.

## Marketo Sales Engage {#marketo-sales-engage}

* **Auditoria Aprimorada**: nova visibilidade de todas as pessoas, emails e [conteúdo](/help/marketo/product-docs/marketo-sales-connect/templates/view-template-list-as-another-user.md) em uma instância com capacidade adicional de [encerrar campanhas existentes](/help/marketo/product-docs/marketo-sales-connect/campaigns/view-campaigns-list-as-another-user.md)criadas por outros usuários.
* **[Gerenciamento de Cancelamento de Assinatura](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/marketo-unsubscribe-check.md)**: maximize a capacidade de entrega e a conformidade com a capacidade de [bloquear domínios de email](/help/marketo/product-docs/marketo-sales-connect/admin/blocked-domains.md) para que sejam contatados. O Marketo também fará referência cruzada com o banco de dados de clientes potenciais para cancelamentos de inscrição antes de enviar um email.

## [!DNL Bizible] da Marketo {#bizible-by-marketo}

* **[!DNL Bizible]Aprimoramentos dos recursos do Discover**: Os novos recursos de segmentação de painel permitem que os profissionais de marketing entendam melhor o desempenho.
* **Suporte a Várias Moedas**: alterne entre sua moeda corporativa e qualquer moeda local com a nova funcionalidade de conversão automática de moeda de [!DNL Bizible], criada em tabelas de moeda do CRM.
* **Custos de campanha do CRM**: meça o gasto e o ROI de atividades de marketing offline com a capacidade de obter automaticamente dados de custo do objeto de campanha do CRM.

## Junho de 2019 {#june}

Os seguintes recursos estão incluídos na versão de junho de 2019. Verifique a edição do Marketo quanto à disponibilidade de recursos.

**_Versões Trimestrais_**

Os recursos a seguir foram lançados em 14 de junho de 2019.

## Principais serviços do Marketo {#marketo-core-services}

* **Soma de Verificação de Arquivo de Extração em Massa**: verifique se um arquivo completo foi recuperado comparando o hash do arquivo à cadeia de caracteres de soma de verificação dos trabalhos de extração concluídos.
* **Migração automatizada do Email 1.0 para o Email 2.0**: o Email 2.0 é totalmente compatível com emails e modelos do Email 1.0. Aproveite novos recursos, como a capacidade de agrupar elementos de conteúdo (imagens, texto etc.) nos módulos do, defina variáveis como Sequência, Cor, Imagem, etc. nos modelos do e utilize modelos iniciais totalmente responsivos. Também inclui um Seletor visual de modelo de email.

>[!CAUTION]
>
>A partir de 18 de junho de 2019, o Email 1.0 não estará mais disponível. Você pode saber mais sobre o Email 2.0 e a descontinuação do Email 1.0 [aqui](https://nation.marketo.com/docs/DOC-7038).

## Marketing baseado em contas {#account-based-marketing}

* **[!DNL LinkedIn]Correspondência de Conta (BETA)** : um novo recurso ABM agora está disponível na versão beta, oferecendo a capacidade de enviar listas de contas conhecidas e de espaço em branco diretamente do Marketo para o LinkedIn. Essa funcionalidade é incluída automaticamente para todos os clientes do Marketo ABM.

<br> 

**_Liberando Durante o Trimestre_**

Espera-se que os seguintes recursos sejam lançados ao longo do segundo trimestre e até ao início do terceiro trimestre de 2019.

## [!DNL Marketo Sky] {#marketo-sky}

* As **Limitações de eventos** e as **Metas de eventos** geralmente estão disponíveis em [!DNL Marketo Sky] no complemento Eventos Premium.

   * Limites de evento: otimize a experiência do cliente para seus eventos e webinários com limites de registro, redirecionamentos de página e funcionalidade de lista de espera.
   * Metas do evento: defina metas de registro e participação no evento e acompanhe o progresso em tempo real.

* **Links de Navegação Completos**: habilitamos a navegação para todos os aplicativos com permissão, como Hootsuite, Calendário e muito mais.
* **Email, Página de Aterrissagem, Trecho, Formulário, Imagem e Exibições da Lista de Arquivos**: Exiba, pesquise e execute ações em massa em qualquer um dos seus ativos no Design Studio.
* **Página de detalhes de imagem, arquivo e trecho**: obtenha detalhes rápidos sobre seus ativos com metadados como _criado às/por_ e ações como _excluir_ e _aprovar_.
* **Widget de postagens do blog da comunidade**: acesse postagens recentes da comunidade no My Marketo.
* **Widget de expiração em breve**: adicione o widget &quot;Expirando em breve&quot; ao painel Meu Marketo para ver quais campanhas e páginas de aterrissagem estão definidas para expirar em seguida.
* **Mais Cartões de Lista Inteligente**: segmente e direcione adequadamente com cartões de lista inteligente adicionais, incluindo a etapa de fluxo &quot;Criar Tarefa&quot;, as regras de lista inteligente de CRM e muito mais.
* **Página de detalhes do desafiante/campeão de email**: veja dados como critérios de vitória, criados em, etc., dos seus testes de desafiante/campeão de email.

## Marketo [!DNL Sales Connect] {#marketo-sales-connect}

* **Ações em massa na [!DNL Salesforce] Personalização**: maximize a produtividade enviando emails e adicionando contatos a campanhas em massa com a Personalização do [!DNL Salesforce].
* **Configurações - [!DNL Salesforce] Página para Administradores e Não Administradores**: gerencie sua instância do [!DNL Sales Connect] com uma exibição clara da instância do [!DNL Salesforce] conectada ao [!DNL Sales Connect], bem como de Minhas atualizações de Email para [!DNL Salesforce]. As configurações aprimoradas de sincronização para administradores, não administradores e toda a equipe de sincronização serão lançadas nos próximos meses.
* **Configurações - Página de integração**: um local central para todas as suas integrações, para que você possa aproveitar ao máximo o nosso ecossistema aberto.
* **Configurações - Página de Perfil**: exiba e atualize os detalhes da sua conta, altere sua senha e verifique o status da implementação da sua instância nesta nova página de perfil.

* **Modelos de email do sistema**: recursos de design, capacidade de resposta e internacionalização atualizados.

## [!DNL Bizible] da Marketo {#bizible-by-marketo}

* **Suporte a Várias Moedas para[!DNL Dynamics]**: [!DNL Bizible] agora se adapta às tabelas de moeda [!DNL Microsoft Dynamics], para que você possa facilmente alternar entre moedas corporativas e locais. (Observação: o suporte para o SFDC foi lançado no primeiro trimestre de 2019.)
* **Integração com o Drift**: entenda como as conversas com o Drift afetam a jornada do cliente. [!DNL Bizible] também irá obter endereços de email de conversas para criar um novo cliente potencial ou conectar o ponto de contato a um cliente potencial existente.
* A **Localização**: [!DNL Bizible] agora está disponível em todos os idiomas com suporte da Marketo (inglês, japonês, alemão, espanhol, francês e português).

_&#x200B;**Webinar sobre a versão do produto**&#x200B;_ Assista à gravação do nosso webinário sobre as inovações da versão de 19 de junho [aqui](https://engage.marketo.com/Marketo-June-Product-Release-2019-On-Demand.html).

## Agosto de 2019 {#august}

Os seguintes recursos estão incluídos na versão de agosto de 2019. Verifique a edição do Marketo quanto à disponibilidade de recursos.

**_Versões Trimestrais_**

Os recursos a seguir foram lançados em 16 de agosto de 2019.

## Marketo Engage principal {#core-marketo-engage}

* **Estrutura de webinário extensível**: economize tempo com a nova estrutura de webinário pronta para uso da Marketo (introduzida nas notas de versão do inverno de 19) que transmite dados facilmente de provedores de webinário para o Marketo e vice-versa. Evento e Zoom agora estão disponíveis nessa nova estrutura.
* **Atualização da API do Smart Campaign**: gerencie recursos inteligentes de ciclo de vida da campanha conforme completamos a interface CRUD (criar, ler, atualizar, excluir).
* **Alteração na API de Cabeçalhos de Email**: a API de Cabeçalho de Email de Atualização não requer mais que um email tenha um modelo anexado para atualizar campos de cabeçalho, como linha de assunto.

**Account-Based Marketing** ![(estrela)](assets/yellow-star.png)

* **[!DNL LinkedIn]Correspondência de Conta**, anteriormente em beta, agora está disponível de modo geral.
* **AccountAI** está sendo oficialmente remarcada como **Account Profiling**.

<br> 

**_Liberando Durante o Trimestre_**

Os recursos a seguir estão em um ciclo não trimestral e serão lançados durante o terceiro trimestre e até o início do quarto trimestre de 2019.

**[!DNL Marketo Sales Connect]** ![(estrela)](assets/yellow-star.png)

* **Aprimoramento do Layout da Página de Pessoas:** gerencie seus grupos e pessoas por meio de importações de listas e ações em massa no novo layout da página de pessoas.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela ( ![(estrela)](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante da Marketo para obter mais informações.

>[!NOTE]
>
>**Descontinuação do TLS 1.0 e 1.1**: para alinhar-se ao padrão de segurança de classe mundial da Adobe, descontinuaremos o suporte ao TLS 1.0 e 1.1 a partir de 13 de dezembro de 2019. Os sistemas integrados com o Marketo que não estiverem em conformidade com o protocolo 1.2 poderão perder acesso aos serviços da Marketo Engage.
>
>**Para manter o acesso ao Marketo Engage, verifique se todos os sistemas cliente são compatíveis com TLS 1.2 antes de 13 de dezembro de 2019**. Você encontra informações mais detalhadas [aqui](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).

**_Webinar de versão do produto_** [Junte-se a nós](https://engage.marketo.com/August_19_Release_Webinar.html) em 28 de agosto às 1:00PM PT / 4:00PM ET para um webinário ao vivo hospedado por nossa equipe de produtos e saiba mais sobre os recursos incluídos nesta versão.
