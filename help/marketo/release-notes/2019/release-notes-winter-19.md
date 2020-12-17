---
unique-page-id: 17727823
description: Notas de versão - Winter '19 - Marketo Docs - Documentação do produto
title: Notas de versão - inverno de 1919
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '1112'
ht-degree: 0%

---


# Notas de versão: inverno de 19 {#release-notes-winter}

Os seguintes recursos estão incluídos na versão de inverno de 1919. Verifique sua edição de marketing para ver a disponibilidade de recursos.

Clique nos links de título para artigos detalhados de visualização para cada recurso, se disponível.

>[!NOTE]
>
>O Facebook agora requer uma conta do Business Manager para aproveitar sua integração com a Audiência personalizada. Seu serviço do Facebook LaunchPoint *deve* ser associado a uma conta do Business Manager, ou **sua integração não funcionará mais após 14 de janeiro de 2019**. Para configurar uma conta do Business Manager, consulte [Ajuda do Facebook](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>A Microsoft está forçando todos os clientes online a atualizarem para a versão mais recente do Microsoft Dynamics. Se você estiver integrando sua instância do Marketo ao Dynamics Online, precisará [atualizar para a versão mais recente da solução Marketo](../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md) antes de **31 de janeiro de 2019** para garantir que sua integração continuará funcionando.

>[!NOTE]
>
>O Marketo está atualizando a versão OAuth para GoToWebinar de 1.0 para 2.0. O suporte para o OAuth 1.0 será substituído em janeiro de 2019. Se você for um cliente GoToWebinar, precisará autenticar novamente seus logons pelo LaunchPoint (na área Admin) em **31 de janeiro de 2019** para garantir que sua integração continuará funcionando. Para obter mais detalhes, consulte nossa [página da comunidade](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Aprimoramentos da plataforma principal {#core-platform-enhancements}

** [Email CC para e-mails de marketing](../../product-docs/email-marketing/general/email-cc.md)**

Inclua até cinco endereços CC por recipient em emails enviados pelo Marketo.

**API**

* **Suporte a domínio com várias marcas para API de ativos:** a aprovação e clonagem de ativos produzem os mesmos resultados na API e na interface do usuário.
* **Suporte CC por email para API** de ativos: Os usuários que clonam, aprovam e processam emails por meio da API manterão a paridade com as configurações da interface do usuário.

** [Munchkin v155 (Beta)](http://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Modo** somente API: Agora, os usuários podem determinar quando e como rastrear membros de seu banco de dados permitindo que aplicativos da Web de página única façam uma chamada explícita quando desejam gravar uma visita da página da Web em vez de depender do rastreamento automático do Marketo.
* **Gerenciamento** de não participação: Gerencie com facilidade as opções de não participação ao combinar o domínio do cookie de opção de não participação com o domínio do cookie de rastreamento Munchkin.
* **Parâmetro** Decider de Nível de Domínio: Domínios de duas letras (ou seja, &quot;  [website.io](http://website.io)&quot;) será rastreado automaticamente no Marketo sem requisitos adicionais de configuração.

## Marketing to Sales Engate {#marketo-sales-engage}

* **Perfil** personalizado do Salesforce: O Sales Engage agora oferece suporte a perfis personalizados ilimitados.

* **Personalização** do Salesforce: Ao remover campos de atividade personalizados não críticos, os usuários podem configurar o Sales Engage na plataforma CRM com mais eficiência.
* **Serviço** de e-mail: Aproveite melhor a entrega, além de melhor Rastreamento de resposta, funcionalidade de e-mail agendado e funcionalidade de e-mail em massa ao conectar-se ao Microsoft Outlook (por meio do Office365 ou On-Prem, por meio da guia Conexão de e-mail).
* **Novas configurações** de administrador: Duas páginas administrativas foram adicionadas para otimizar sua instância do Sales Engage

   * *O* Gerenciamento de equipe suporta um processo de configuração de conta contínua ao permitir que os administradores editem subscrições e equipes.
   * *As equipes de* Configurações administrativas do Salesforce configuram sua sincronização SFDC mais rápida e fácil do que nunca.

* **Plug-in OWA para Windows**: Com um único suplemento, todos os clientes do Windows Office365 terão suporte no Sales Engage, proporcionando a capacidade de usar o Feed ao vivo no Outlook. O novo plug-in estará disponível na Microsoft Store.
* **Atividade Pusher**: Sincronize o envolvimento de vendas com a plataforma principal de marketing para aproveitar insights de marketing em tempo real.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>As liberações de Marketo Sky ocorrem com maior frequência. Espera-se que os seguintes recursos e aprimoramentos sejam lançados durante o último trimestre do primeiro trimestre. Para obter mais detalhes e atualizações, consulte nossa [documentação do Sky](https://help.marketo.com/hc/en-us/articles/360012858573).

* **Experiência** padrão opcional: Os usuários do Marketing Cloud podem definir o Marketo Sky como sua experiência padrão se tiverem recebido acesso de um Administrador.

* **Reimaginei Meu Marketo**: Personalize sua experiência adicionando widgets que fornecem informações críticas, notificações e links para as áreas visitadas com mais frequência.

* **Visualizações de Lista do Design Studio e páginas** de detalhes: Desfrute de um maior nível de organização e precisão com visualizações de lista filtráveis e pesquisáveis de emails, landings page e formulários. As Páginas de detalhes do ativo fornecem informações principais sobre cada ativo, incluindo quais programas o ativo é usado, o número de snippets que estão sendo usados e muito mais.

* **Pesquisa** global: O Marketo agora oferta uma função de pesquisa global mais rápida e robusta em toda a plataforma. Query de pesquisa agora são executados em todos os espaços de trabalho acessíveis e podem pesquisar ativos (ativos e arquivados), rótulos, campanhas e programas. Os resultados da pesquisa são fornecidos por meio de uma sobreposição e cada resultado inclui sua trilha de localização de arquivo para especificar onde o ativo vive.

* **Interface** do usuário aprimorada: Novos ícones, módulos e botões, juntamente com uma nova paleta de cores para refletir a atualização da nossa marca e tornar o Marketo Sky ainda mais impressionante e funcional.

* **Aprimoramentos** de utilização de Programas de email: Continuamos avançando para a paridade na funcionalidade do Programa de email entre nossa plataforma clássica de gerenciamento líder de marketing e a nova experiência do Marketo Sky.
* **Programas** evento Com Webinar: Programas de evento com Webinar agora estão disponíveis no Marketo Sky (observação: somente GoToWebinar será suportado nesta versão, com outras integrações estabelecidas ao longo do tempo).

## Marketing baseado em conta {#account-based-marketing}

** [Segmentação e filtragem baseadas no ABM Persona](../../product-docs/account-based-marketing/using-personas.md)**

Personalize suas campanhas do ABM para pessoas específicas em contas nomeadas. O recurso ABM Persona cria um cargo padrão com base na segmentação de lead e permite a configuração de segmentações personalizadas adicionais.

## Analytics {#analytics}

**Bizíblia**

* **Campos** Calculados Personalizados: Use qualquer atributo Bizible para criar campos personalizados que possam ser usados para relatórios e segmentação de painéis.

* **Certificação** SOC II Tipo II: A nova certificação de segurança e privacidade baseia-se na acreditação Tipo I desde o início deste ano.

## Personalização da Web {#web-personalization}

**[Adicionar subdomínios nas configurações da conta](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Para gerenciar domínios e subdomínios com mais eficiência, os usuários agora podem adicionar subdomínios às configurações de conta RTP.

## Marketing Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**Kit de desenvolvimento de software (SDK) do MME atualizado para Android**

Atualizamos nosso SDK para Android para uma estrutura mais moderna, estável e escalável que contém mais flexibilidade e novos recursos de engenharia. Os desenvolvedores de aplicativos Android agora podem usar diretamente o [Firebase Cloud Messaging](http://firebase.google.com/docs/cloud-messaging/) (FCM) do Google com esse novo SDK.

* [Instruções do desenvolvedor](http://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Perguntas frequentes do desenvolvedor](http://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>Os desenvolvedores de aplicativos **devem** atualizar para a nova versão antes de 31 de março de 2019. Se você não atualizar seu SDK até 31 de março de 2019, qualquer novo usuário que baixar seu aplicativo após essa data não poderá receber notificações por push até que você atualize para a versão mais recente do SDK. A atualização do SDK não exigirá que os usuários atuais do aplicativo móvel baixem novamente uma nova versão do aplicativo.

## Atualizações adicionais {#additional-updates}

**Plataforma de Webinar extensível**

Além do nosso lançamento de produtos, nossa equipe de parceiros está trabalhando em uma nova estrutura que permite que os provedores de webinars criem e mantenham suas próprias integrações com o Marketo, proporcionando mais flexibilidade na atualização e no aprimoramento de suas soluções e, ao mesmo tempo, permitindo que os profissionais de marketing aproveitem ao máximo suas integrações escolhidas.

Pretendemos lançar nossa nova plataforma com provedores caso a caso. Para obter mais informações, consulte nossos [detalhes do programa](https://www.marketo.com/why-marketo/partners/technology/) ou entre em contato com o seu comerciante.
