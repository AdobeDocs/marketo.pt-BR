---
unique-page-id: 17727823
description: Notas de versão - inverno de 19 - Documentos do Marketo - Documentação do produto
title: Notas de versão - inverno de 19
translation-type: tm+mt
source-git-commit: 9d8a6d9880de5d2af211906c2410f2057c1f454d
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---


# Notas de versão: Inverno de 19 {#release-notes-winter}

Os seguintes recursos estão incluídos na versão de inverno de 19. Verifique sua edição do Marketo para ver a disponibilidade dos recursos.

Clique nos links de título para exibir os artigos detalhados de cada recurso, se disponível.

>[!NOTE]
>
>O Facebook agora requer uma conta do Business Manager para aproveitar sua integração com o Público-alvo personalizado. Seu serviço do Facebook LaunchPoint *deve* ser associado a uma conta do Business Manager ou **sua integração não funcionará mais após 14 de janeiro de 2019**. Para configurar uma conta do Business Manager, consulte a [Ajuda do Facebook](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>A Microsoft está enviando todos os clientes online para atualizarem para a versão mais recente do Microsoft Dynamics. Se estiver integrando sua instância do Marketo com o Dynamics Online, será necessário [atualizar para a versão mais recente da solução Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) antes de **31 de janeiro de 2019** para garantir que sua integração continue funcionando.

>[!NOTE]
>
>O Marketo está atualizando a versão OAuth para GoToWebinar de 1.0 para 2.0. O suporte para OAuth 1.0 será descontinuado em janeiro de 2019. Se você for um cliente do GoToWebinar, precisará autenticar novamente seus logons por meio do LaunchPoint (na área de administração) em **31 de janeiro de 2019** para garantir que sua integração continue funcionando. Para obter mais detalhes, consulte nossa [Página da comunidade](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Aprimoramentos da plataforma principal {#core-platform-enhancements}

**[Email CC para emails do Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Inclua até cinco endereços CC por recipient em emails enviados pelo Marketo.

**API**

* **Suporte a domínio de multimarcas para API de ativos:** a aprovação e a clonagem de ativos produzem os mesmos resultados na API e na interface do usuário.
* **Suporte CC por email para API** de ativos: Os usuários que clonam, aprovam e processam emails por meio da API manterão a paridade com as configurações da interface do usuário.

**[Munchkin v155 (Beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Modo** somente API: Agora, os usuários podem determinar quando e como rastrear membros de seu banco de dados, permitindo que aplicativos da Web de página única chamem explicitamente quando desejam registrar uma visita à página da Web, em vez de depender do rastreamento automático do Marketo.
* **Gerenciamento** de não participação: Gerencie facilmente as opções de não participação, combinando o domínio do cookie de não participação com o domínio do cookie de rastreamento do Munchkin.
* **Parâmetro** do Decider em Nível de Domínio: Domínios com duas letras (ou seja, &quot;  [site.io](https://website.io)&quot;) será rastreado automaticamente no Marketo sem requisitos de configuração adicionais.

## Marketo Sales Engage {#marketo-sales-engage}

* **Perfil** personalizado do Salesforce: O Sales Engage agora oferece suporte a perfis personalizados ilimitados.

* **Personalização do Salesforce**: Ao remover campos de atividade personalizados não críticos, os usuários podem configurar o Engajamento de vendas na plataforma CRM com mais eficiência.
* **Serviço** de email: Aproveite melhor capacidade de entrega, além de Rastreamento de resposta aprimorado, funcionalidade de Email agendado e funcionalidade de email em massa ao se conectar ao Microsoft Outlook (por meio do Office365 ou no local, por meio da guia Conexão de email).
* **Novas configurações** de administrador: Duas páginas de administrador foram adicionadas para otimizar sua instância do Sales Engage

   * _O_ Gerenciamento de equipe oferece suporte a um processo de configuração de conta simples, permitindo que os administradores editem assinaturas e equipes.
   * _As equipes de_ Configurações de Administração do Salesforce configuram a sincronização do SFDC de forma mais rápida e fácil do que nunca.

* **Plug-in OWA para Windows**: Com um único suplemento, todos os clientes do Windows Office365 serão suportados no Sales Engage, fornecendo a capacidade de usar o Feed em tempo real no Outlook. O novo plug-in estará disponível na Microsoft Store.
* **Empurrador** de atividades: Sincronize o envolvimento de vendas com a plataforma principal do Marketo para aproveitar os insights de marketing em tempo real.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>As liberações de Marketo Sky ocorrem com mais frequência. Espera-se que os seguintes recursos e aprimoramentos sejam lançados durante o último trimestre/primeiro trimestre. Para obter mais detalhes e atualizações, verifique nossa [documentação do Sky](https://help.marketo.com/).

* **Experiência** padrão opcional: Os usuários do Marketo podem definir o Marketo Sky como sua experiência padrão se tiverem recebido acesso de um Administrador.

* **Reimaginado Meu Marketo**: Personalize sua experiência adicionando widgets que fornecem informações críticas, notificações e links para suas áreas visitadas com mais frequência.

* **Exibições de lista do Design Studio e páginas** de detalhes: Desfrute de um maior nível de organização e precisão com exibições de lista de emails, landing pages e formulários filtráveis e pesquisáveis. As Páginas de detalhes do ativo fornecem informações importantes sobre cada ativo, incluindo quais programas o ativo é usado, o número de trechos que estão sendo usados e muito mais.

* **Pesquisa** global: O Marketo agora oferece uma função de pesquisa global mais rápida e robusta em toda a plataforma. Agora, as consultas de pesquisa são executadas em todos os espaços de trabalho acessíveis e podem pesquisar ativos (ativos e arquivados), rótulos, campanhas e programas. Os resultados da pesquisa são fornecidos por uma sobreposição e cada resultado inclui sua trilha de localização de arquivo para especificar onde o ativo permanece.

* **Interface** do usuário aprimorada: Novos ícones, modais e botões, juntamente com uma nova paleta de cores para refletir a atualização da marca e tornar o Marketo Sky ainda mais impressionante e funcional.

* **Aprimoramentos de usabilidade do programa de email**: Continuamos avançando em direção à paridade na funcionalidade do Programa de email entre nossa plataforma clássica de Gerenciamento de clientes potenciais do Marketo e a nova experiência do Marketo Sky.
* **Programas** Event-With-Webinar: Os programas Event-With-Webinar agora estão disponíveis no Marketo Sky (observação: somente o GoToWebinar será suportado nesta versão, com outras integrações estabelecidas ao longo do tempo).

## Marketing baseado em conta {#account-based-marketing}

**[Segmentação e filtragem baseadas em personalização do ABM](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personalize suas campanhas do ABM para personas específicas em contas nomeadas. O recurso ABM Persona cria um título de trabalho padrão com base na segmentação de lead e permite a configuração de segmentações de persona adicionais.

## Analytics {#analytics}

**Bizible**

* **Campos** calculados personalizados: Use qualquer atributo Bizible para criar campos personalizados que podem ser usados para relatórios e segmentação de painel.

* **Certificação** SOC II Tipo II: A nova certificação de segurança e privacidade baseia-se na acreditação de Tipo I a partir do início deste ano.

## Personalização da Web {#web-personalization}

**[Adicionar subdomínios nas configurações da conta](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Para gerenciar domínios e subdomínios com mais eficiência, os usuários agora podem adicionar subdomínios às configurações da conta RTP.

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**Kit de desenvolvimento de software (SDK) do MME atualizado para Android**

Atualizamos nosso SDK para Android para uma estrutura mais moderna, estável e escalável que contém mais flexibilidade e novos recursos de engenharia. Os desenvolvedores de aplicativos Android agora podem usar diretamente o [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) do Google com este novo SDK.

* [Instruções do desenvolvedor](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Perguntas frequentes do desenvolvedor](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Os desenvolvedores de aplicativos **devem** atualizar para a nova versão antes de 31 de março de 2019. Se você não atualizar seu SDK até 31 de março de 2019, qualquer novo usuário que baixar seu aplicativo após essa data não poderá receber notificações por push até que você atualize para a versão mais recente do SDK. A atualização do SDK não exigirá que os usuários atuais do aplicativo móvel baixem novamente uma nova versão do aplicativo.

## Atualizações adicionais {#additional-updates}

**Plataforma de webinars extensível**

Além do lançamento de nossos produtos, nossa equipe de parceiros está trabalhando em uma nova estrutura que permite que os provedores de webinars criem e mantenham suas próprias integrações com o Marketo, fornecendo mais flexibilidade na atualização e no aprimoramento de suas soluções e permitindo que os profissionais de marketing aproveitem ao máximo as integrações escolhidas.

Planejamos lançar nossa nova plataforma com provedores caso a caso. Para obter mais informações, consulte os [detalhes do programa](https://www.marketo.com/why-marketo/partners/technology/) ou entre em contato com o Marketo.
