---
description: Notas de versão - Janeiro de 2021 - Documentação da Marketo - Documentação do produto
title: Notas de versão - Janeiro de 2021
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# Notas de versão: Jan 2021 {#release-notes-jan-21}

Os seguintes recursos estão incluídos na versão de 21 de janeiro de 2012. Verifique sua edição do Marketo para ver a disponibilidade dos recursos.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela ( ![(star)](assets/star-yellow.svg)) são complementos pagos. Entre em contato com seu representante de Marketo Engage para saber mais.

**_Versões trimestrais_**

Os seguintes recursos serão lançados em **15 de janeiro de 2021**.

## Experiência do usuário de próxima geração {#next-generation-user-experience}

* Suporte para espaços de trabalho: A experiência do usuário de Marketo Engage da próxima geração reúne a aparência do Adobe Experience Cloud com inovações de produtividade para ajudar profissionais de marketing a trabalhar de forma mais rápida e inteligente. Na versão mais recente, adicionamos suporte total para espaços de trabalho e partições, incluindo a capacidade de compartilhar pastas em espaços de trabalho. A tela do lado direito oferecerá uma alternância de alternância para permitir a transição perfeita entre experiências antigas e novas por recurso, sem perder o contexto. [Saiba ](https://nation.marketo.com/t5/The-Next-Generation-Experience/Next-Generation-Experience-FAQ/ba-p/307124) mais sobre as perguntas frequentes sobre a experiência da próxima geração na Marketing Nation.

## Personalização de vários canais {#multi-channel-personalization}

* **[Adobe Experience Cloud Audience Sync Fase 3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: O recurso atual de Sincronização de público-alvo da Adobe Experience Cloud (AEC) agora oferece suporte à sincronização contínua de público-alvo B2B bidirecional do Marketo Engage para outros aplicativos da AEC, incluindo ofertas da Adobe Experience Platform (AEP) como a Plataforma de dados do cliente em tempo real e a Adobe Experience Platform Ativation.  À medida que os leads são adicionados e removidos para seus segmentos de público-alvo, o Marketo Engage sincronizará automaticamente o público-alvo atualizado em todos os aplicativos AEC conectados. Use-o para aproveitar os casos de uso de orquestração multicanal, re-direcionamento, supressão de público-alvo, personalização e relatórios do Adobe na sua pilha de tecnologia do AEC.
* **[Sincronização contínua de público-alvo com o Google, Facebook e LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**: A sincronização continuamente automatizada com uma rede de anúncios pode ser ativada em uma lista estática, atualizando a rede de anúncios como alterações de associação à lista sem exigir a intervenção do usuário.
* **[Tokens para Campos](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)** Personalizados do Membro do Programa: Estendemos os recursos de campo personalizado do membro do programa para oferecer suporte à estrutura de token. Os profissionais de marketing podem inserir tokens de campos personalizados de membros do programa em emails, landing pages, mensagens SMS, notificações por push e webhooks. Use novos tokens em ações de fluxo de campanha para alterar valores de dados, criar uma tarefa ou um momento interessante.

## Páginas de aterrissagem e Forms {#landing-pages-and-forms}

* **API** de formulário: Puxe as informações do lead ou acione campanhas de criação enquanto extrai dados de formulários que não são da Marketo. Formulários não Marketo podem ser integrados com o Marketo Engage por meio da API REST. A nova API fornece a capacidade de imitar o envio de formulário Marketo Engage com todas as funcionalidades associadas.
* **API** de páginas de aterrissagem: Simplifique os fluxos de trabalho de edição e tradução em aplicativos integrados com a nova API de visualização de página de aterrissagem. Fornecedores de terceiros agora podem renderizar visualizações totalmente personalizadas de páginas de aterrissagem sem fazer logon no Marketo Engage.  A API de visualização da página de aterrissagem permite fluxos de trabalho completos de edição e localização em aplicativos integrados de terceiros.

## Marketing por e-mail {#email-marketing}

* **[Limites De Recuperação De Objetos Personalizados Aumentados](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**: Os desenvolvedores de scripts do Velocity de email podem aumentar rapidamente o número de objetos personalizados para 100 por meio da substituição de autoatendimento. Os profissionais de marketing podem aumentar a eficácia das Campanhas inteligentes acessando um maior número de objetos personalizados de primeiro e segundo nível.

## Integração ao CRM do Salesforce {#salesforce-crm-integration}

* [Autenticação](/help/marketo/product-docs/crm-sync/salesforce-sync/setting-up-oauth-2-0.md) do Salesforce CRM: O protocolo OAuth 2.0 está disponível para operações de sincronização entre o Marketo Engage e o Salesforce CRM. Para novos assinantes, essa opção é ativada por padrão. Os assinantes atuais podem solicitar esse recurso entrando em contato com o Suporte da Marketo.
* [Painel de Sincronização do Salesforce CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md): Os administradores podem revisar rapidamente o status de sincronização do Salesforce CRM no painel. O intervalo do relatório de desempenho de sincronização foi aumentado de 2 horas para 5 dias.
* **Exportação** de metadados: Aprimorado para oferecer suporte a atributos de objetos da oportunidade, contas nomeadas, campos padrão e personalizados do membro do programa.

## Administração {#administration}

* **Página** da minha conta atualizada: Revise as informações essenciais da assinatura na página Minha conta. Os usuários com qualquer nível de acesso podem visualizar o nome da assinatura, o identificador do data center e a ID do Munchkin.

**_Lançamento em todo o trimestre_**

Os seguintes recursos estão em um ciclo não trimestral e serão lançados nos próximos meses.

## Sales Insight {#sales-insight}

![(estrela)](assets/star-yellow.svg)

* **[Workflows de email de teste aprimorado (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**: Aumente a eficiência de sua equipe de vendas com fluxos de trabalho de email aprimorados do teste de Insight de vendas. Os vendedores podem enviar emails de teste para endereços de email selecionados antes de enviar emails em massa para até 200 recipients.
* **[Insights sobre o status de email (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**: Os usuários veem uma mensagem de aviso quando tentam enviar um email para uma ID de email inválida ou um endereço de email que não tenha assinado antes de enviar um email.  Os status do delivery de emails podem ser revisados na guia email do Sales Insight.
* **Enviar emails em massa a partir de Painéis  [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) de Conta e  [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) Oportunidade (Salesforce CRM)**: Melhore a eficiência do fluxo de trabalho do vendedor e envolva-se com uma conta inteira ou com uma lista de contatos de oportunidade usando novos recursos de ação em massa. Envie emails ou adicione contatos a campanhas do Marketo Engage usando a nova opção suspensa nas guias conta ou oportunidade, em vez de trabalhar com contatos individuais. Adicione contatos de conta a uma lista de controle para ser notificado quando os clientes em potencial ficarem ativos.
* **[Insight de vendas para integrações](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)** não nativas do Salesforce CRM: As assinaturas GA com integrações personalizadas do Salesforce CRM podem instalar o pacote Sales Insight e ajudar as equipes de vendas a priorizar e interagir com os clientes potenciais e as oportunidades mais promissoras.
* **[Melhorias](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)** de melhor desempenho: Entre em contato rapidamente com clientes potenciais da guia Melhor Economia ao enviá-los por e-mail ou adicioná-los a uma Campanha do Marketo Engage. Exiba um lead no Marketo Engage ou adicione-o à sua lista de controle. As ações em massa e as opções de classificação na guia Melhor Economia economizam tempo e melhoram a eficiência da equipe de vendas.

## SalesConnect {#sales-connect}

![(estrela)](assets/star-yellow.svg)

* **Limitação da conexão de email (BETA)**: Melhore sua capacidade de fornecimento de email e dimensione sua comunicação de vendas 1:1 com o Limite de conexão de email para conexão de vendas. Nossa nova tecnologia de limitação gerencia automaticamente o tempo de envio de emails para criar experiências ininterruptas para usuários do Exchange e Gmail. Diminua ou elimine o uso de aplicativos de envio de email em massa de terceiros.
* **Acompanhamento** de Rejeição da Conexão de Email: Obtenha informações sobre a qualidade do lead e o desempenho do modelo de email com o novo relatório de devolução de email. Os usuários do Exchange e do Gmail podem optar por receber notificações de devolução que serão acumuladas no Feed ao vivo, Pastas de email, Análises de modelo e Análises de campanha.
* **Configuração** da página de perfil: Gerencie com facilidade as preferências do usuário na nova página de perfil. Altere a senha, edite as configurações de localização geográfica e idioma e revise os status de integrações em um único local.
* **Gerenciamento** de modelos: Organize modelos de email de vendas em categorias com um novo recurso de arrastar e soltar para garantir acesso rápido a modelos relevantes e reduzir o tempo de pesquisa.
* **Atualizações** da experiência do usuário do Sales Connect: Personalize o layout da grade do Sales Connect redimensionando e reorganizando as colunas. Suas preferências de exibição são salvas automaticamente.

**_Anúncios e desaprovações_**

* Todos os usuários devem atualizar para a versão mais recente do Sales Insight **antes de 15 de janeiro de 2021**. Se você não tiver concluído a atualização, será solicitado a fazer isso ao fazer logon no aplicativo. Siga as instruções [neste guia](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). A versão atualizada inclui um patch para uma vulnerabilidade de segurança identificada. O patch foi lançado originalmente em 6 de abril de 2016. Observação: **As versões 1.4363 ou superior** não precisam executar uma atualização.
* A desaprovação do serviço do Formulário 1.0 entrará em vigor na versão **maio de 2021**. O serviço Forms 1.0 será totalmente descontinuado, resultando na perda de funcionalidade de quaisquer ativos restantes do Forms 1.0 que ainda estejam em uso. Além disso, os envios de formulários feitos por meio de métodos não suportados, como POSTs de formulários programáticos para os endpoints leadCapture/save e leadCapture/save2, serão rejeitados. Para obter mais informações e remediar, consulte [nossa publicação na Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* Em 2021, o Marketo Engage fará alterações na estrutura do URL para landing pages, formulários, imagens e arquivos de ativos. Para assinaturas Marketo Engage existentes, começaremos a implantação gradual em 1º de abril de 2021. Mais detalhes sobre a linha do tempo de lançamento serão lançados em março de 2021. Para obter detalhes sobre como cada tipo de ativo afetado será alterado, consulte [nossa publicação na Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Webinar da versão do produto_**

Quer saber mais sobre esses recursos e aprimoramentos? Certifique-se de [registrar-se agora](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) para se juntar a nós em 21 de janeiro às 13:00 PT / 4:00 PM ET para obter um webinário em tempo real com nossa equipe de produtos para aprofundar essas inovações.
