---
description: Notas de versão - maio de 2022 - Documentação do Marketo - Documentação do produto
title: Notas de versão - Maio de 2022
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# Notas de versão: maio de 2022 {#release-notes-may-22}

Abaixo você encontrará todos os recursos incluídos na versão de maio de 2022. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela (![star](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante da Marketo Engage para obter mais informações.

**_Versões Trimestrais_**

Os recursos a seguir serão lançados em **6 de maio de 2022**, com uma implantação em fases dos recursos restantes nas semanas seguintes (a menos que especificado de outra forma).

## Integração de CRM nativa {#native-crm-integration}

**[Integração nativa do Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} (disponibilidade limitada)**: melhore o engajamento com profissionais de saúde sincronizando a atividade entre o Veeva CRM e o Marketo Engage por meio da integração nativa. Essa integração permite que os profissionais de marketing criem experiências entre canais mais personalizadas e perfeitas para os profissionais de saúde. Entre em contato com o Gerente de sucesso do cliente se estiver interessado em participar.

## Orquestração entre canais {#cross-channel-orchestration}

**Eventos de Chatbot para[!DNL Dynamic Chat]**: aproveite dados de comportamento mais detalhados para visitantes da Web, como tempo na página, tempo no site e porcentagem de rolagem de página, para definir quando uma caixa de diálogo de chat deve ser exibida.

**PDF Embed para[!DNL Dynamic Chat]**: aumente o engajamento e compartilhe conteúdo significativo incorporando PDFs em caixas de diálogo de chat e meça o desempenho do conteúdo por meio do rastreamento de atividades de engajamento.

**Suporte de Idioma Estendido para[!DNL Dynamic Chat]**: A interface do usuário [!DNL Dynamic Chat] agora também estará disponível em francês, alemão, japonês, português e espanhol. As caixas de diálogo de bate-papo também podem ser configuradas nessas linguagens.

**Excluir URLs para[!DNL Dynamic Chat]**: controle em qual de suas páginas da Web [!DNL Dynamic Chat] aparece com a capacidade de excluir URLs específicas dos critérios de direcionamento.

**[Aprimoramentos na Filtragem de atividade de bot por email](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**: continue protegendo a integridade do seu banco de dados com a capacidade de identificar o comportamento de bot com base em Agentes de usuário de link oculto ou IPs e padrões de proximidade, além da identificação de correspondência na lista IAB existente. Visualize estatísticas de atividades de bot que permitem compreender o número de atividades de bot identificadas para cada tipo.

**[Cabeçalho STS para Links de Acompanhamento de Email](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**: atenda às práticas recomendadas de segurança com a capacidade de aplicar cabeçalhos de Segurança de Transporte Seguro para garantir que o tráfego para links rastreados esteja sempre seguro.

## Experiência de última geração {#modern-ux}

**Alternar alternância padrão para a experiência da próxima geração**: a alternância padrão será a nova experiência em todas as telas em que estiver disponível, facilitando a descoberta de designs e aprimoramentos de usabilidade atualizados pelos usuários.

**Tela atualizada na experiência da próxima geração**:

Estamos fornecendo a Exibição de Detalhes do Modelo de Email no [!UICONTROL Design Studio] na experiência de próxima geração, oferecendo um design atualizado e aprimoramentos de usabilidade acessíveis via switch de alternância.

## Automação de experiência {#experience-automation}

**Etapas de Fluxo de Autoatendimento (continuação da versão beta)**: expanda a conectividade entre o Marketo Engage e o restante da pilha com a capacidade de criar etapas de fluxo personalizadas para uso em Campanhas inteligentes. Tanto os usuários quanto os parceiros da Marketo Engage podem aproveitar essa funcionalidade para permitir o uso de serviços Web externos em campanhas acionadoras, em lote e executáveis (em contraste com webhooks que só podem ser usados em campanhas acionadoras).

## Aprimoramentos na API {#api-enhancements}

* **Acesso ampliado à API para assinaturas habilitadas para CRM**: estamos expandindo o acesso à API para assinaturas com sincronização de CRM habilitada para permitir que os usuários recuperem Empresas, Oportunidades e Vendedores da Marketo Engage.
* **Suporte para tipos de dados &quot;ocultos&quot; no Forms**: fornece a capacidade de gerenciar campos de formulário ocultos por meio da API.
* **Suporte a Vários Valores de Comparação para isNot Form via Regras**: gerencie a visibilidade dos campos de formulário com base no fato de o valor de outro campo não ser um dos valores de uma determinada lista.
* **Permitir configuração de Valores de Exibição e Enviados em Listas de Seleção Separadamente**: Defina separadamente o valor de exibição e o valor de envio em um campo. Por exemplo, mostrar o nome de um hotel, mas enviar uma ID interna para o back-end.
* **Permitir Configuração de Desabilitar Rastreamento Aberto em Criar ou Atualizar Email**: criar um email com rastreamento aberto desabilitado.

## Anúncios {#announcements}

**Exclusividade e Verificação de Email**: a partir de abril, a implantação da Verificação de Email começará. Nesse momento, os endereços de email de usuários do Marketo Engage exigirão verificação e exclusividade (isso não se aplica aos usuários somente da API). Os usuários autenticados do serviço de diretório terão seus emails verificados automaticamente quando a assinatura for habilitada com a Verificação de email.

A Verificação de email para assinaturas que usam o recurso &quot;[!UICONTROL Logon na Caixa de Diálogo de Convite de Usuário]&quot; ou que têm um único email associado a vários usuários coincidirá com o lançamento de maio. As assinaturas com um único email associado a vários usuários serão ativadas com a Verificação de email e exigirão que esses usuários resolvam o conflito e usem um email exclusivo por usuário. Quando o recurso &quot;Login no diálogo de usuário para convite&quot; estiver ativado, os usuários convidados por meio desse recurso precisarão ter um endereço de e-mail exclusivo. Para usuários somente API convidados por meio desse recurso, o endereço de email não precisa ser exclusivo.

**Alteração no Comportamento da Pasta de Arquivos Mortos**: com esta versão, a capacidade de criar novos ativos em pastas de Arquivos Mortos não estará mais disponível nos menus de contexto da árvore. As opções de menu para criar novos ativos estarão ocultas para todos os ativos. [Saiba mais aqui](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_Webinar de lançamento de produto_**

[Webinar da versão de março e maio de 2022 do Marketo Engage](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
