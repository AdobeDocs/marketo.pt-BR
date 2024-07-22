---
description: Notas de versão - Janeiro de 2021 - Documentação do Marketo - Documentação do produto
title: Notas de versão - Janeiro de 2021
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# Notas de versão: janeiro de 2021 {#release-notes-jan-21}

Os seguintes recursos estão incluídos na versão de janeiro de 2021. Verifique a edição do Marketo quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela (![(estrela)](assets/yellow-star.png)) são complementos pagos. Entre em contato com o representante da Marketo Engage para obter mais informações.

**_Versões Trimestrais_**

Os recursos a seguir serão lançados em **15 de janeiro de 2021**.

## Experiência do usuário de última geração {#next-generation-user-experience}

* Suporte para espaços de trabalho: a experiência de usuário de última geração do Marketo Engage reúne a aparência e a funcionalidade do Adobe Experience Cloud com inovações de produtividade para ajudar os profissionais de marketing a trabalhar de modo mais rápido e inteligente. Na versão mais recente, adicionamos suporte total para espaços de trabalho e partições, incluindo a capacidade de compartilhar pastas entre espaços de trabalho. A tela direita oferecerá um switch de alternância que permite a transição contínua entre experiências antigas e novas por recurso sem perder o contexto. [Saiba mais](https://nation.marketo.com/t5/The-modern-ux/modern-ux-FAQ/ba-p/307124) em Perguntas frequentes sobre a experiência da próxima geração na Nação de marketing.

## Personalization multicanal {#multi-channel-personalization}

* **[Fase de sincronização de público-alvo do Adobe Experience Cloud 3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: o recurso de sincronização de público-alvo existente do Adobe Experience Cloud (AEC) agora oferece suporte à sincronização de público-alvo B2B contínua e bidirecional do Marketo Engage para outros aplicativos da AEC, incluindo ofertas da Adobe Experience Platform (AEP) como Real-time Customer Data Platform e Adobe Experience Platform Ativation.  À medida que clientes em potencial são adicionados e removidos dos segmentos de público-alvo, o Marketo Engage sincronizará automaticamente o público atualizado nos aplicativos da AEC conectados. Use-o para aproveitar a orquestração de vários canais, o redirecionamento, a supressão de público-alvo, a personalização e os casos de uso de relatórios do Adobe na pilha de tecnologia da AEC.
* **[Sincronização contínua de público-alvo com Google, Facebook e LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**: a sincronização automatizada contínua com uma rede de anúncios pode ser habilitada em uma lista estática, atualizando a rede de anúncios como alterações de associação de lista sem a intervenção do usuário.
* **[Tokens para Campos Personalizados de Membros do Programa](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**: estendemos os recursos de campo personalizado de membros do programa para oferecer suporte à estrutura de token. Os profissionais de marketing podem inserir tokens de campos personalizados de membros do programa em emails, landing pages, mensagens SMS, notificações por push e webhooks. Use novos tokens em ações de fluxo de campanha para alterar valores de dados, criar uma tarefa ou um momento interessante.

## Páginas de aterrissagem e Forms {#landing-pages-and-forms}

* **API de Formulário**: obtenha informações de clientes potenciais ou acione campanhas de criação ao extrair dados de formulários que não sejam da Marketo. Formulários que não sejam da Marketo podem se integrar ao Marketo Engage por meio da API REST. A nova API oferece a capacidade de mimetizar o envio do formulário Marketo Engage com todas as funcionalidades associadas.
* **API de páginas de aterrissagem**: simplifique os fluxos de trabalho de edição e tradução em aplicativos integrados com a nova API de visualização de páginas de aterrissagem. Fornecedores de terceiros agora podem renderizar visualizações totalmente personalizadas de páginas de aterrissagem sem fazer logon no Marketo Engage.  A API de visualização de página de aterrissagem permite fluxos de trabalho de edição e localização completos em aplicativos integrados de terceiros.

## Marketing por e-mail {#email-marketing}

* **[Limites de recuperação de objetos personalizados aumentados](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**: os desenvolvedores de scripts do Velocity de email podem aumentar rapidamente o número de objetos personalizados para 100 por meio da substituição de autoatendimento. Os profissionais de marketing podem aumentar a eficácia das Campanhas inteligentes acessando um número maior de objetos personalizados de primeiro e segundo nível.

## Integração ao CRM do Salesforce {#salesforce-crm-integration}

* [Autenticação do Salesforce CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md): o protocolo OAuth 2.0 está disponível para operações de sincronização entre o Marketo Engage e o Salesforce CRM. Para novos assinantes, essa opção é ativada por padrão. Os assinantes atuais podem solicitar esse recurso entrando em contato com o Suporte da Marketo.
* [Painel de sincronização do Salesforce CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md): os administradores podem examinar rapidamente o status de sincronização do Salesforce CRM no painel. O período do relatório de desempenho de sincronização foi aumentado de 2 horas para 5 dias.
* **Exportação de metadados**: aprimorado para oferecer suporte a atributos de objeto de oportunidade, contas nomeadas, campos padrão e personalizados do membro do programa.

## Administração {#administration}

* **Página Minha Conta Atualizada**: examine as informações essenciais da assinatura na página Minha Conta. Os usuários com qualquer nível de acesso podem visualizar o nome da assinatura, o identificador do data center e a ID do Munchkin.

**_Liberando Durante o Trimestre_**

Os recursos a seguir estão em um ciclo não trimestral e serão lançados nos próximos meses.

## Sales Insight {#sales-insight}

![(estrela)](assets/yellow-star.png)

* **[Fluxos de trabalho de email de teste aprimorados (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**: aumente a eficiência da sua equipe de vendas com fluxos de trabalho de email de teste aprimorados do Sales Insight. Os vendedores podem enviar email de teste para endereços de email escolhidos antes de enviar emails em massa para até 200 recipients.
* **[Insights sobre o status do email (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**: os usuários veem uma mensagem de aviso quando estão tentando enviar um email para uma ID de email inválida ou para um endereço de email sem assinatura antes de enviar um email.  Os status do delivery de emails podem ser revisados na guia Email do Sales Insight.
* **Enviar emails em massa dos painéis [Conta](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) e [Oportunidade](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) (Salesforce CRM)**: melhore a eficiência do fluxo de trabalho do vendedor e envolva-se com uma conta inteira ou uma lista de contatos de oportunidade usando novos recursos de ação em massa. Envie emails ou adicione contatos às campanhas do Marketo Engage usando a nova opção suspensa nas guias conta ou oportunidade em vez de trabalhar com contatos individuais. Adicionar contatos de conta a uma lista de observação para serem notificados quando os clientes em potencial estiverem ativos.
* **[Sales Insight para integrações de CRM não-nativas do Salesforce](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**: as assinaturas do GA com integrações personalizadas do Salesforce CRM podem instalar o pacote Sales Insight e ajudar as equipes de vendas a priorizar e interagir com os clientes em potencial e oportunidades mais promissores.
* **[Melhorias nas melhores opções](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**: contate rapidamente os clientes em potencial na guia Melhores opções enviando um email ou adicionando-os a uma Campanha Marketo Engage. Exibir um cliente potencial no Marketo Engage ou adicioná-lo à sua lista de observação. As ações em massa e as opções de classificação na guia Melhores Opções economizam tempo e melhoram a eficiência da equipe de vendas.

## Sales Connect {#sales-connect}

![(estrela)](assets/yellow-star.png)

* **Limitação da Conexão de Email (BETA)**: melhore sua capacidade de entrega de email e dimensione sua comunicação de vendas 1:1 com a Limitação da Conexão de Email para o Sales Connect. Nossa nova tecnologia de controle gerencia automaticamente o tempo de envio de email para criar experiências perfeitas para usuários do Exchange e do Gmail. Diminuir ou eliminar o uso de aplicativos de envio de email de terceiros em massa.
* **Rastreamento de rejeição de conexão de email**: obtenha informações sobre a qualidade dos clientes potenciais e o desempenho dos modelos de email com o novo relatório de rejeição de email. Os usuários do Exchange e do Gmail podem optar por receber notificações de rejeição que serão agrupadas no Feed ativo, nas Pastas de email, no Template Analytics e no Campaign Analytics.
* **Configuração da página de perfil**: gerencie facilmente as preferências do usuário na nova página de perfil. Altere a senha, edite as configurações de idioma e geolocalização e revise os status de integrações em um único local.
* **Gerenciamento de modelos**: organize modelos de email de vendas em categorias com um novo recurso de arrastar e soltar para garantir acesso rápido a modelos relevantes e reduzir o tempo de pesquisa.
* **Atualizações da Experiência do Usuário do Sales Connect**: Personalize o layout de grade do Sales Connect redimensionando e reorganizando colunas. Suas preferências de exibição são salvas automaticamente.

**_Anúncios e desaprovações_**

* Todos os usuários devem atualizar para a versão mais recente do Sales Insight **antes de 15 de janeiro de 2021**. Se você não tiver concluído a atualização, será solicitado a fazê-lo ao fazer logon no aplicativo. Siga as instruções [neste guia](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). A versão atualizada inclui um patch para uma vulnerabilidade de segurança identificada. O patch foi originalmente lançado em 6 de abril de 2016. Observação: **Versões 1.4363 ou superior** não precisam executar uma atualização.
* A desativação do serviço Form 1.0 entrará em vigor na versão **maio 2021**. O serviço do Forms 1.0 será totalmente descontinuado, resultando na perda de funcionalidade de todos os ativos restantes do Forms 1.0 ainda em uso. Além disso, os envios de formulários feitos por meio de métodos não compatíveis, como POSTs de formulário programáticos para os endpoints leadCapture/save e leadCapture/save2, serão rejeitados. Para obter mais informações e correções, consulte [nossa publicação na Nação de marketing](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* Em 2021, o Marketo Engage fará alterações na estrutura de URLs para páginas de aterrissagem, formulários e ativos de imagens e arquivos. Para assinaturas Marketo Engage existentes, iniciaremos a implantação gradual em 1º de abril de 2021. Mais detalhes sobre a linha do tempo de implantação serão lançados em março de 2021. Para obter detalhes sobre como cada tipo de ativo afetado será alterado, consulte [nossa publicação na Nação de marketing](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Webinar de lançamento de produto_**

Quer saber mais sobre esses recursos e aprimoramentos? Certifique-se de [registrar-se agora](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) para se juntar a nós no dia 21 de janeiro às 13h (PT) / 16h (ET) para um webinário ao vivo com nossa equipe de produtos para aprofundar essas inovações.
