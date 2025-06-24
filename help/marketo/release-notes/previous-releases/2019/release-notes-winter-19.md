---
unique-page-id: 17727823
description: Notas de versão - Winter '19 - Marketo Docs - Documentação do produto
title: Notas de versão - inverno de 19
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 3%

---

# Notas de versão: inverno de 19 {#release-notes-winter}

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

   * O _Gerenciamento de Equipe_ dá suporte a um processo de configuração de conta simples permitindo que os administradores editem assinaturas e equipes.
   * As _Configurações de administração do Salesforce_ ajudam as equipes a configurar a sincronização do SFDC de forma mais rápida e fácil do que nunca.

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

Atualizamos nosso SDK for Android para uma estrutura mais moderna, estável e escalável, que contém mais flexibilidade e novos recursos de engenharia. Os desenvolvedores de aplicativos do Android agora podem usar diretamente o [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) do Google com este novo SDK.

* [Instruções para o desenvolvedor](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Perguntas frequentes do desenvolvedor](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Os desenvolvedores de aplicativos **devem** atualizar para a nova versão antes de 31 de março de 2019. Se você não atualizar seu SDK até 31 de março de 2019, qualquer novo usuário que baixar seu aplicativo após essa data não poderá receber notificações por push até que você atualize para a versão mais recente do SDK. A atualização do SDK não exigirá que os usuários atuais do aplicativo móvel baixem novamente uma nova versão do aplicativo.

## Atualizações adicionais {#additional-updates}

**Plataforma de webinário extensível**

Além do lançamento de nosso produto, nossa equipe de parceiros está trabalhando em uma nova estrutura que permite que os provedores de webinários criem e mantenham suas próprias integrações com o Marketo, fornecendo mais flexibilidade na atualização e no aprimoramento de suas soluções, além de permitir que os profissionais de marketing aproveitem ao máximo as integrações escolhidas.

Planejamos lançar nossa nova plataforma com provedores caso a caso. Para obter mais informações, consulte os [detalhes do programa](https://www.marketo.com/why-marketo/partners/technology/) ou entre em contato com o seu contato da Marketo.
