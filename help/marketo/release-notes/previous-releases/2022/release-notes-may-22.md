---
description: Notas de versão - maio de 2022 - Documentação do Marketo - Documentação do produto
title: Notas de versão - maio de 2022
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# Notas de versão: maio de 2022 {#release-notes-may-22}

Abaixo você encontrará todos os recursos incluídos na versão de maio de 2022. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Recursos indicados por uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o representante da Marketo Engage para obter mais informações.

**_Versões trimestrais_**

Os recursos a seguir começarão a ser lançados em **6 de maio de 2022**, com uma implantação em fases dos recursos restantes nas semanas subsequentes (a menos que especificado de outra forma).

## Integração de CRM nativa {#native-crm-integration}

**[Integração nativa do Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} (disponibilidade limitada)**: melhore o engajamento com profissionais de saúde sincronizando a atividade entre o Veeva CRM e o Marketo Engage por meio de integração nativa. Essa integração permite que os profissionais de marketing criem experiências entre canais mais personalizadas e perfeitas para os profissionais de saúde. Entre em contato com a equipe de conta do Adobe (seu gerente de conta) se estiver interessado em participar.

## Orquestração entre canais {#cross-channel-orchestration}

**Eventos de Chatbot para Dynamic Chat**: aproveite dados de comportamento mais detalhados para visitantes da Web, como tempo na página, tempo no site e porcentagem de rolagem da página, para definir quando uma caixa de diálogo de chat deve ser exibida.

**PDF incorporado para Dynamic Chat**: aumente o engajamento e compartilhe conteúdo significativo incorporando PDF em caixas de diálogo de chat e meça o desempenho do conteúdo por meio do rastreamento de atividades de engajamento.

**Suporte estendido de idioma para o Dynamic Chat**: a interface do usuário do Dynamic Chat agora também estará disponível em francês, alemão, japonês, português e espanhol. As caixas de diálogo de bate-papo também podem ser configuradas nessas linguagens.

**Excluir URLs do Dynamic Chat**: controle qual dos Dynamic Chat das suas páginas da Web aparece com a capacidade de excluir URLs específicos dos critérios de direcionamento.

**[Melhorias na filtragem de atividade de bot por email](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**: continue protegendo a integridade do banco de dados com a capacidade de identificar o comportamento do bot com base em Agentes do usuário de link oculto ou IPs e padrões de proximidade, além da identificação de correspondência da lista IAB existente. Visualize estatísticas de atividades de bot que permitem compreender o número de atividades de bot identificadas para cada tipo.

**[Cabeçalho STS para links de rastreamento de email](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**: atenda às práticas recomendadas de segurança com a capacidade de aplicar cabeçalhos Secure Transport Security para garantir que o tráfego para links rastreados esteja sempre seguro.

## Experiência de última geração {#modern-ux}

**Alternar switch padrão para a experiência da próxima geração**: o switch de alternância será padrão para a nova experiência em todas as telas em que estiver disponível, facilitando para os usuários a descoberta dos designs atualizados e das melhorias de usabilidade.

**Tela atualizada na experiência da próxima geração**:

Oferecemos Exibição de detalhes do modelo de email no Design Studio na experiência de última geração, oferecendo um design atualizado e aprimoramentos de usabilidade acessíveis por meio de switch de alternância.

## Automação de experiência {#experience-automation}

**Etapas de fluxo de autoatendimento (beta contínuo)**: expanda a conectividade entre o Marketo Engage e o restante da pilha com a capacidade de criar etapas de fluxo personalizadas para uso em Campanhas inteligentes. Os usuários e parceiros do Marketo Engage podem aproveitar essa funcionalidade para permitir o uso de serviços Web externos em campanhas acionadoras, em lote e executáveis (em contraste com webhooks que só podem ser usados em campanhas acionadoras).

## Aprimoramentos na API {#api-enhancements}

* **Acesso estendido à API para assinaturas habilitadas para CRM**: estamos expandindo o acesso à API para assinaturas com uma sincronização de CRM habilitada para permitir que os usuários recuperem Empresas, Oportunidades e Vendedores do Marketo Engage.
* **Suporte para tipos de dados &quot;ocultos&quot; no Forms**: fornece a capacidade de gerenciar campos de formulário ocultos por meio da API.
* **Suporte a vários valores de comparação para isNot Form via regras**: gerencie a visibilidade dos campos de formulário com base no fato de o valor de outro campo não ser um dos valores em uma determinada lista.
* **Permitir configuração de Valores de Exibição e Enviados em Selecionar Listas Separadamente**: Defina o valor de exibição e o valor enviado em um campo separadamente. Por exemplo, mostrar o nome de um hotel, mas enviar uma ID interna para o back-end.
* **Permitir configuração de Desabilitar rastreamento aberto ao criar ou atualizar email**: crie um email com o rastreamento de abertura desativado.

## Anúncios {#announcements}

**Verificação e exclusividade de email**: a partir de abril, a implantação da Verificação de email será iniciada. Nesse ponto, os endereços de email do usuário do Marketo Engage exigirão verificação e exclusividade (isso não se aplica aos usuários somente da API). Os usuários autenticados do serviço de diretório terão seus emails verificados automaticamente quando a assinatura for habilitada com a Verificação de email.

A verificação de email para assinaturas que usam o recurso &quot;Logon na caixa de diálogo Convidar usuário&quot; ou que têm um único email associado a vários usuários coincidirá com a versão de maio. As assinaturas com um único email associado a vários usuários serão ativadas com a Verificação de email e exigirão que esses usuários resolvam o conflito e usem um email exclusivo por usuário. Quando o recurso &quot;Logon na caixa de diálogo de usuário do convite&quot; estiver habilitado, os usuários convidados por meio desse recurso precisarão ter um endereço de email exclusivo. Para usuários somente API convidados por meio desse recurso, o endereço de email não precisa ser exclusivo.

**Arquivar mudança de comportamento da pasta**: com esta versão, a capacidade de criar novos ativos nas pastas Arquivar não estará mais disponível nos menus de contexto da árvore. As opções de menu para criar novos ativos estarão ocultas para todos os ativos. [Saiba mais aqui](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_Webinário de lançamento do produto_**

[Webinário da versão de março e maio de 2022 do Marketo Engage](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
