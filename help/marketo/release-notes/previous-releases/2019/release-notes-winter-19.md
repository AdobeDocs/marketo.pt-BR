---
unique-page-id: 17727823
description: Notas de versão - Winter '19 - Marketo Docs - Documentação do produto
title: Notas de versão - inverno de 19
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
feature: Release Information
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 3%

---

# Notas de versão: inverno de 19 {#release-notes-winter}

Os seguintes recursos estão incluídos na versão Winter &#39;19. Verifique a edição do Marketo quanto à disponibilidade de recursos.

Clique nos links de título para exibir artigos detalhados para cada recurso, se disponíveis.

>[!NOTE]
>
>O facebook agora exige uma conta do Business Manager para aproveitar a integração Personalizada de público-alvo. Seu serviço Facebook LaunchPoint *deve* estar associado a uma conta do Business Manager ou **sua integração não funcionará mais após 14 de janeiro de 2019**. Para configurar uma conta do Business Manager, consulte [Ajuda do facebook](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>A Microsoft está enviando todos os clientes online para atualizarem para a versão mais recente do Microsoft Dynamics. Se você estiver integrando sua instância do Marketo com o Dynamics Online, será necessário [atualize para a versão mais recente da solução da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) antes **31 de janeiro de 2019** para garantir que sua integração continue funcionando.

>[!NOTE]
>
>O Marketo está atualizando a versão do OAuth para o GoToWebinar de 1.0 para 2.0. O suporte para OAuth 1.0 será descontinuado em janeiro de 2019. Se você for um cliente do GoToWebinar, precisará autenticar novamente seus logons por meio do LaunchPoint (na área de Administrador) **31 de janeiro de 2019** para garantir que sua integração continue funcionando. Para obter mais detalhes, consulte nossa [Página da comunidade](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Melhorias da plataforma principal {#core-platform-enhancements}

**[Email CC para emails do Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Inclua até cinco endereços por destinatário para CC nos e-mails enviados através do Marketo.

**API**

* **Suporte de domínio de várias marcas para a API de ativos:** A aprovação e a clonagem de ativos produzem os mesmos resultados na API e na interface.
* **Suporte de CC por email para a API de ativos**: os usuários que clonam, aprovam e processam emails por meio da API manterão a paridade com as configurações da interface do usuário.

**[Munchkin v155 (Beta)](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/lead-tracking)**

* **Modo somente API**: agora os usuários podem determinar quando e como rastrear membros de seu banco de dados, permitindo que aplicativos Web de página única façam chamadas explicitamente quando quiserem gravar uma visita de página da Web, em vez de depender do rastreamento automático do Marketo.
* **Gerenciamento de recusa**: gerencie facilmente as opções de não participação, associando o domínio de cookie de opção de não participação ao domínio de cookie de rastreamento Munchkin.
* **Parâmetro de decisão no nível do domínio**: domínios de duas letras (ou seja, &quot; [website.io](https://website.io)&quot;) rastreará automaticamente no Marketo sem requisitos de configuração adicionais.

## Marketo Sales Engage {#marketo-sales-engage}

* **Perfil personalizado do Salesforce**: o Sales Engage agora oferece suporte a perfis personalizados ilimitados.

* **Personalização do Salesforce**: ao remover campos de atividade personalizados não críticos, os usuários podem configurar o Sales Engage na plataforma CRM com mais eficiência.
* **Serviço de e-mail**: Aproveite a melhor capacidade de entrega, além do rastreamento de resposta aprimorado, da funcionalidade de email agendado e da funcionalidade de email em massa conectando-se ao Microsoft Outlook (pelo Office365 ou no local, pela guia Conexão de email).
* **Novas Configurações de Administração**: duas páginas de administrador foram adicionadas para otimizar a instância do Sales Engage

   * _Gerenciamento de Equipe_ O oferece suporte a um processo simples de configuração de conta permitindo que administradores editem assinaturas e equipes.
   * _Configurações do administrador do Salesforce_ O ajuda as equipes a configurar a sincronização do SFDC de forma mais rápida e fácil do que nunca.

* **Plug-in OWA para Windows**: com um único suplemento, todos os clientes do Windows Office 365 terão suporte no Sales Engage, fornecendo a capacidade de usar o Feed ativo no Outlook. O novo plug-in estará disponível na Microsoft Store.
* **Pusher de atividades**: sincronizar o Sales Engage com a plataforma principal do Marketo para aproveitar os insights de marketing em tempo real.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>As liberações de Marketo Sky ocorrem com mais frequência. Os seguintes recursos e aprimoramentos devem ser lançados no final do quarto trimestre/início do primeiro trimestre. Para obter mais detalhes e atualizações, consulte nossa [Documentação do Sky](https://help.marketo.com/).

* **Experiência padrão opcional**: os usuários do Marketo podem definir o Marketo Sky como sua experiência padrão se tiverem recebido acesso de um administrador.

* **Refez a imagem do meu Marketo**: personalize sua experiência adicionando widgets que fornecem informações críticas, notificações e links para suas áreas visitadas com mais frequência.

* **Exibições de lista e páginas de detalhes do Design Studio**: aproveite um maior nível de organização e precisão com exibições de lista filtráveis e pesquisáveis de emails, páginas de aterrissagem e formulários. As Páginas de detalhes do ativo fornecem informações importantes sobre cada ativo, incluindo quais programas o ativo é usado, o número de snippets que estão sendo usados e muito mais.

* **Pesquisa global**: o Marketo agora oferece uma função de pesquisa global mais rápida e robusta na plataforma. As consultas de pesquisa agora são executadas em todos os espaços de trabalho acessíveis e podem pesquisar ativos (ativos e arquivados), rótulos, campanhas e programas. Os resultados da pesquisa são fornecidos por meio de uma sobreposição e cada resultado inclui sua trilha de localização de arquivo para especificar onde o ativo está.

* **Interface do usuário aprimorada**: novos ícones, modais e botões, juntamente com uma nova paleta de cores para refletir a atualização de nossa marca e tornar o Marketo Sky ainda mais impressionante e funcional.

* **Aprimoramentos de usabilidade do programa de email**: Continuamos a avançar para a paridade na funcionalidade do Programa de email entre nossa plataforma clássica de Gerenciamento de leads da Marketo e a nova experiência Marketo Sky.
* **Programas De Evento Com Webinário**: os programas Event-With-Webinar agora estão disponíveis no Marketo Sky (observação: somente GoToWebinar será compatível nesta versão, com mais integrações estabelecidas ao longo do tempo).

## Marketing baseado em contas {#account-based-marketing}

**[Segmentação e filtragem com base em persona do ABM](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personalize suas campanhas do ABM para personalidades específicas em contas nomeadas. O recurso Persona ABM cria um título de cargo padrão com base na segmentação de clientes potenciais e permite a configuração de segmentações de persona adicionais.

## Analytics {#analytics}

**Bizible**

* **Campos calculados personalizados**: use qualquer atributo do Bizible para criar campos personalizados que possam ser usados para relatórios e segmentação de painel.

* **Certificação SOC II Tipo II**: a nova certificação de segurança e privacidade se baseia na capacitação de Tipo I do início deste ano.

## Personalização na Web {#web-personalization}

**[Adicione subdomínios nas configurações de conta](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Para gerenciar domínios e subdomínios com mais eficiência, os usuários agora podem adicionar subdomínios às configurações de conta RTP.

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**Atualização do SDK (Software Development Kit, kit de desenvolvimento de software) MME para Android**

Atualizamos nosso SDK para Android para uma estrutura mais moderna, estável e escalável, que contém mais flexibilidade e novos recursos de engenharia. Google Os desenvolvedores de aplicativos com Android agora podem usar diretamente o [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) com esse novo SDK.

* [Instruções para o desenvolvedor]https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android)

>[!NOTE]
>
>Desenvolvedores de aplicativos **deve** atualização para a nova versão antes de 31 de março de 2019. Se você não atualizar seu SDK até 31 de março de 2019, qualquer novo usuário que baixar seu aplicativo após essa data não poderá receber notificações por push até que você atualize para a versão mais recente do SDK. A atualização do SDK não exigirá que os usuários atuais do aplicativo móvel baixem novamente uma nova versão do aplicativo.

## Atualizações adicionais {#additional-updates}

**Plataforma de webinário extensível**

Além do lançamento de nosso produto, nossa equipe de parceiros está trabalhando em uma nova estrutura que permite que os provedores de webinários criem e mantenham suas próprias integrações com o Marketo, fornecendo mais flexibilidade na atualização e no aprimoramento de suas soluções, além de permitir que os profissionais de marketing aproveitem ao máximo as integrações escolhidas.

Planejamos lançar nossa nova plataforma com provedores caso a caso. Para obter mais informações, consulte nossa [detalhes do programa](https://www.marketo.com/why-marketo/partners/technology/) ou entre em contato com o contato da Marketo.
