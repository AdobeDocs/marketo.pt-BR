---
title: "2022"
description: 2022 - Documentação do Marketo - Documentação do produto
feature: Release Information
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
  - id: efc9a24a-a6a4-449d-a3e6-44f6c74dfd46
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: babcd0bfb6c16165488cabd075a9d75d2952016b
workflow-type: tm+mt
source-wordcount: 4311
ht-degree: 7%

---

# 2022

## Janeiro de 2022 {#january}

Os seguintes recursos estão incluídos na versão de janeiro de 2022. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

**_Versões Trimestrais_**

Os recursos a seguir serão lançados em **21 de janeiro de 2022**, com uma implantação em fases de cada recurso nas semanas seguintes (a menos que especificado de outra forma).

## Experiência de última geração

* **Screens atualizado na Experiência da Próxima Geração**: estamos fornecendo telas adicionais e atualizadas na experiência da próxima geração, que oferecem um design atualizado e aprimoramentos de usabilidade acessíveis via switch de alternância:

  * Detalhes de Ativo da Página de Aterrissagem no [!UICONTROL Design Studio]
  * Detalhes de ativos da landing page em [!UICONTROL atividades de marketing]

## [!DNL Microsoft Dynamics] Integração {#microsoft-dynamics-integration}

* **Sincronização do Tipo de Campo Multiselect Optionset Geralmente Disponível**: sincronize o tipo de campo multiselect optionset de [!DNL Microsoft Dynamics] para aproveitar em Smart Lists e Campanhas Inteligentes para um direcionamento de público mais granular. Os exemplos incluem: tópicos/produtos de interesse, modos de comunicação preferidos e muito mais. Esta nova sincronização está disponível para [!DNL Microsoft Dynamics] versão 9.X (incluindo o Dynamics 365 Online).

* **Autenticação de Servidor para Servidor para[!DNL Microsoft Dynamics 365 Online]**: para aumentar a segurança, ofereceremos suporte a S2S (Servidor para Servidor) como um modo adicional de autenticação para o usuário de sincronização do Marketo Engage no Azure Ative Diretory para acesso não interativo ao [!DNL Microsoft Dynamics 365 Online]. Isso permite empregar a autenticação multifator, pois todas as autenticações e logons serão baseados no OAuth (somente ID do cliente e segredo do cliente).

>[!NOTE]
>
>O modo S2S é baseado no usuário do aplicativo em vez do usuário licenciado, o que salva o uso de uma licença adicional.

## Administração {#administration}

* **[Regras de validação de formulários](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**: mantêm a integridade do banco de dados com a capacidade de bloquear o envio de formulários do Marketo Engage por domínios de email problemáticos ou indesejáveis. O painel Regra de validação de formulário global permite que os administradores definam uma inclui na lista de bloqueios de formulário ou habilitem uma lista predefinida de domínios de consumidores livres para bloquear formulários.

* **[Segurança de Cabeçalho de Página de Aterrissagem](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**: os administradores podem gerenciar cabeçalhos de Segurança de Transporte Restrita e Opções de X-Frame em seus domínios de página de aterrissagem para aplicar requisitos de segurança rigorosos.

**_Liberando Durante o Trimestre_**

Os recursos a seguir estão em um ciclo não trimestral e serão lançados nos próximos meses.

## Conector de destino do AEP Marketo Engage - Criar novos leads {#aep-marketo-engage-destination-connector}

Os clientes do Marketo Engage que também usam o Adobe Experience Platform (AEP) podem maximizar seu banco de dados com a capacidade de enviar registros de novas pessoas para o Marketo Engage a partir do AEP por meio do conector de destino do AEP. Ao enviar segmentos de público do AEP para o Marketo Engage, as pessoas dentro do segmento que ainda não existe no banco de dados do Marketo Engage [podem ser adicionadas automaticamente a ele](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## [!DNL Sales Insight]

![(estrela)](assets/yellow-star.png)

**[!DNL Sales Insight]para [!DNL Salesforce] CRM**

* **Nova Coluna de Tipo para [!UICONTROL Melhores Opções]**: os vendedores obterão insights mais rápidos com uma nova coluna denominada &quot;Tipo&quot; para diferenciar clientes potenciais e contatos na página [!UICONTROL Melhores Opções].

* **[!DNL Salesforce]Atualização da API da Plataforma**: Em resposta à [!DNL Salesforce] desativação das versões 21.0 a 30.0 da API da Plataforma [!DNL Salesforce], o pacote [!DNL Sales Insight] foi atualizado com as APIs mais recentes.

* **Marca Atualizada**: todas as [!DNL Sales Insight] páginas estão sendo atualizadas para se alinharem à marca da Adobe.

**[!DNL Sales Insight]para[!DNL Microsoft Dynamics]**

* **Layout de conta atualizado**: os vendedores podem obter uma visão coletiva das principais atividades, como atividades de email, atividades da Web, momentos interessantes e alterações de pontuação para todos os contatos em uma conta.

## [!DNL Sales Connect]

![(estrela)](assets/yellow-star.png)

* **Resultados e Motivos de Chamadas**: compreenda e rastreie com mais detalhes os esforços de saída de suas equipes de vendas com resultados de chamadas e opções de motivo de chamadas novas e totalmente personalizáveis. Além desses novos campos, estamos introduzindo uma nova governança para impor a seleção do motivo da chamada e do resultado enquanto os vendedores fazem chamadas, uma nova governança para habilitar ou desabilitar os motivos e resultados da chamada e um novo campo personalizado Motivo da Chamada e Resultado da Chamada [!DNL Salesforce] Atividade para registrar dados em [!DNL Salesforce]. [Clique aqui](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) para saber mais.

* Personalização do Detalhe da Atividade **[!DNL Salesforce]**: capture mais dados da atividade de vendas e da tarefa em [!DNL Salesforce] personalizando quais informações são adicionadas ao campo de assunto da tarefa [!DNL Salesforce] quando uma atividade de vendas é registrada em [!DNL Salesforce] de [!DNL Sales Connect]. [Clique aqui](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) para saber mais.

## Anúncios

* **Descontinuação do Marketo Sky**: em março, o Marketo Sky não estará mais disponível, pois concentraremos nossos recursos no fornecimento da experiência de usuário da próxima geração. Em um esforço para manter o acesso a uma funcionalidade exclusiva do Marketo Sky hoje, estamos trazendo a Expiração de ativos e a Substituição de prioridade da Campanha inteligente para a experiência principal em março. [Clique aqui](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) para saber mais.

* **Descontinuação de Pontos de Extremidade de Formulário**: as POSTs de formulário programático sem suporte para o ponto de extremidade leadCapture/save2 serão rejeitadas pelos Marketo Engage Forms. [Clique aqui](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) para saber mais.

* **Logon na Caixa de Diálogo Convidar Usuário**: em março, o recurso opcional existente &quot;Logon na Caixa de Diálogo Convidar Usuário&quot; será descontinuado. O recurso &quot;[!UICONTROL Logon na Caixa de Diálogo de Usuário Convidar]&quot; foi substituído pelo recurso de Universal ID, que é necessário para a futura Integração do Sistema do Adobe Identity Management e foi habilitado em agosto de 2021 em todas as assinaturas. Como resultado da desativação, o Marketo Engage aplicará somente um usuário a ser associado por endereço de email em uma assinatura.

**Domínios Marketo Engage - [!DNL Sales Insight] Configuração**: para domínios Marketo Engage que não têm certificado SSL provisionado e https://, as chamadas falharão com um erro de handshake SSL. Portanto, esses domínios serão encerrados. Como resultado, [!DNL Sales Insight] usuários com uma configuração mais antiga apontando para qualquer um desses domínios podem encontrar erros de texto explicativo do sistema nas páginas de cliente potencial, contato, conta, painéis de oportunidade ou global da Marketo. Recomendamos que você atualize sua [configuração do Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) em [!DNL Salesforce] se encontrar esse erro. Você só precisa atualizar as credenciais do Marketo Engage realçadas na seção &quot;[!DNL Marketo Sales Insight] Config&quot; do documento.

**_Webinar de lançamento de produto_**

[Webinário da versão de janeiro de 2022 do Marketo Engage](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)

## Março de 2022 {#march}

Os seguintes recursos estão incluídos na versão de março de 2022. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

**_Versões Trimestrais_**

Os recursos a seguir serão lançados em **11 de março de 2022**, com uma implantação em fases de cada recurso nas semanas seguintes (a menos que especificado de outra forma).

## Orquestração entre canais

* **[!DNL Dynamic Chat]**: maximize todas as oportunidades em seu site direcionando clientes em potencial e contas com conversas proativas, envolventes e personalizadas 1:1. O [Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} permite que os usuários do Marketo Engage comecem a aproveitar o chat como parte essencial das experiências integradas entre canais para casos de uso de marketing e vendas B2B. Os recursos incluem: a capacidade de reservar reuniões diretamente no chat, roteamento de leads, modelos iniciais, criação de conversas com o método arrastar-e-soltar e muito mais. O Dynamic Chat está incluído em todos os pacotes do Marketo Engage e será lançado para todos os usuários do Marketo Engage este ano.

* **Aprimoramento da Filtragem de atividade de bot por email**: como aprimoramento do recurso [Filtragem de atividade de bot por email](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"} lançado anteriormente, agora é possível aceitar atividades de registro identificadas como bots. Em seguida, você pode filtrar e acionar ações com base em atividades identificadas como executadas por bots.

## Experiência de última geração

* **Screens atualizado na Experiência da Próxima Geração**: estamos fornecendo telas adicionais e atualizadas na experiência da próxima geração, que oferecem um design atualizado e aprimoramentos de usabilidade acessíveis via switch de alternância:

  * Exibição de Lista de Formulários no [!UICONTROL Design Studio] (incluindo novas ações em massa)

* **Atualização do Fluxo de Trabalho do Programa de Importação**: o fluxo de trabalho do programa de importação está sendo fornecido na experiência de próxima geração com um design atualizado e melhorias na usabilidade. Essa será uma alteração automática sem um switch de alternância.

* **Controle de Administração para o Switch de alternância da experiência da próxima geração**: gerencie a implantação da experiência da próxima geração de uma forma que funcione para seus usuários com a capacidade de os administradores selecionarem quais tipos de usuários poderão acessar o switch de alternância.

## Automação de experiência

* **Etapas de Fluxo de Autoatendimento (Beta)**: expanda a conectividade entre o Marketo Engage e o restante da pilha com a capacidade de criar etapas de fluxo personalizadas para uso em Campanhas Inteligentes. Tanto os usuários quanto os parceiros da Marketo podem aproveitar essa funcionalidade para permitir o uso de serviços Web externos em campanhas em lote e executáveis, em contraste com webhooks, que só podem ser usados em campanhas de acionador.

* **Expiração do ativo**: mantenha o controle dos ativos e campanhas com detecção de hora com a capacidade de agendar a desativação automática em uma data e hora especificadas na experiência do usuário do Classic.

* **Substituição de Prioridade de Campanha Inteligente**: certifique-se de que as Campanhas Inteligentes de acionador de alta prioridade sejam executadas o mais rápido possível com a capacidade de substituir a classificação de prioridade de campanha padrão. As Campanhas inteligentes de acionador de prioridade mais baixa também podem ter prioridade mais baixa para liberar recursos de processamento para outras tarefas de prioridade mais alta.

## Aprimoramentos na API

* **Retornar o Status de Rastreamento Aberto de Emails**: permite a leitura do status de rastreamento aberto de emails via API
* **Recuperar linhas de assunto do conteúdo dinâmico do email**: permite que os profissionais de marketing analisem linhas de assunto dinâmicas nas ferramentas de BI
* **Campos Personalizados de Membros do Programa CRUD**: permite que os profissionais de marketing criem programaticamente campos personalizados de membros do programa
* **Exportação de Objeto Personalizado em Massa atualizadaNo Filtro**: permite que os profissionais de marketing sincronizem objetos personalizados de forma programática
* **Expor a configuração Head Start para programas de email**: permite aos profissionais de marketing configurar programas de email com head start via API
* **Atualização Seletiva de Marca de Programa**: permite aos profissionais de marketing enviar atualizações seletivas de marca sem enviar todas as marcas ao mesmo tempo
* **Campo actionResult de Extração de Atividade em Massa**: permite que os profissionais de marketing identifiquem quais atividades foram ignoradas ou falharam

**_Liberando Durante o Trimestre_**

Os recursos a seguir estão em um ciclo não trimestral e serão lançados nos próximos meses.

## [!DNL Bizible] {#bizible}

![(estrela)](assets/yellow-star.png)

* **Modelos de BI**: [!DNL Bizible] agora fornecerá artefatos de relatórios fundamentais e baixáveis, além de relatórios de amostra para Tableau e Power BI, para permitir o rápido desenvolvimento de relatórios personalizados adaptados às suas necessidades comerciais específicas.

## [!DNL Sales Connect]

![(estrela)](assets/yellow-star.png)

* **Limitação da Conexão de Email (GA)**: a Limitação da Conexão de Email permite que administradores do [!DNL Sales Connect] configurem a taxa de envio de emails ao usar o Gmail ou o [!DNL Exchange] como canal de entrega, para que a taxa na qual os emails sejam entregues ao provedor de canal de entrega não exceda os limites impostos.

## Anúncios

* **Descontinuação do Marketo Sky**: em março, o Marketo Sky não estará mais disponível, pois concentraremos nossos recursos no fornecimento da experiência de usuário da próxima geração. Em um esforço para manter o acesso a uma funcionalidade exclusiva do Marketo Sky hoje, estamos trazendo a Expiração de ativos e a Substituição de prioridade da Campanha inteligente para a experiência Clássica. [Clique aqui](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) para saber mais.

**_Webinar de lançamento de produto_**

[Webinário da versão de março e maio de 2022 do Marketo Engage](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## Maio de 2022 {#may}

Abaixo você encontrará todos os recursos incluídos na versão de maio de 2022. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

**_Versões Trimestrais_**

Os recursos a seguir serão lançados em **6 de maio de 2022**, com uma implantação em fases dos recursos restantes nas semanas seguintes (a menos que especificado de outra forma).

## Integração de CRM nativa {#native-crm-integration}

**[Integração nativa do Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} (disponibilidade limitada)**: melhore o engajamento com profissionais de saúde sincronizando a atividade entre o Veeva CRM e o Marketo Engage por meio da integração nativa. Essa integração permite que os profissionais de marketing criem experiências entre canais mais personalizadas e perfeitas para os profissionais de saúde. Entre em contato com o Gerente de sucesso do cliente se estiver interessado em participar.

## Orquestração entre canais

**Eventos de Chatbot para[!DNL Dynamic Chat]**: aproveite dados de comportamento mais detalhados para visitantes da Web, como tempo na página, tempo no site e porcentagem de rolagem de página, para definir quando uma caixa de diálogo de chat deve ser exibida.

**PDF Embed para[!DNL Dynamic Chat]**: aumente o engajamento e compartilhe conteúdo significativo incorporando PDFs em caixas de diálogo de chat e meça o desempenho do conteúdo por meio do rastreamento de atividades de engajamento.

**Suporte de Idioma Estendido para[!DNL Dynamic Chat]**: A interface do usuário [!DNL Dynamic Chat] agora também estará disponível em francês, alemão, japonês, português e espanhol. As caixas de diálogo de bate-papo também podem ser configuradas nessas linguagens.

**Excluir URLs para[!DNL Dynamic Chat]**: controle em qual de suas páginas da Web [!DNL Dynamic Chat] aparece com a capacidade de excluir URLs específicas dos critérios de direcionamento.

**[Aprimoramentos na Filtragem de atividade de bot por email](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**: continue protegendo a integridade do seu banco de dados com a capacidade de identificar o comportamento de bot com base em Agentes de usuário de link oculto ou IPs e padrões de proximidade, além da identificação de correspondência na lista IAB existente. Visualize estatísticas de atividades de bot que permitem compreender o número de atividades de bot identificadas para cada tipo.

**[Cabeçalho STS para Links de Acompanhamento de Email](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**: atenda às práticas recomendadas de segurança com a capacidade de aplicar cabeçalhos de Segurança de Transporte Seguro para garantir que o tráfego para links rastreados esteja sempre seguro.

## Experiência de última geração

**Alternar alternância padrão para a experiência da próxima geração**: a alternância padrão será a nova experiência em todas as telas em que estiver disponível, facilitando a descoberta de designs atualizados e aprimoramentos de usabilidade pelos usuários.

**Tela atualizada na experiência da próxima geração**:

Estamos fornecendo a Exibição de Detalhes do Modelo de Email no [!UICONTROL Design Studio] na experiência de próxima geração, oferecendo um design atualizado e aprimoramentos de usabilidade acessíveis via opção de alternância.

## Automação de experiência

**Etapas de Fluxo de Autoatendimento (continuação da versão beta)**: expanda a conectividade entre o Marketo Engage e o restante da pilha com a capacidade de criar etapas de fluxo personalizadas para uso em Campanhas inteligentes. Tanto os usuários quanto os parceiros da Marketo Engage podem aproveitar essa funcionalidade para permitir o uso de serviços Web externos em campanhas acionadoras, em lote e executáveis (em contraste com webhooks que só podem ser usados em campanhas acionadoras).

## Aprimoramentos na API

* **Acesso ampliado à API para assinaturas habilitadas para CRM**: estamos expandindo o acesso à API para assinaturas com sincronização de CRM habilitada para permitir que os usuários recuperem Empresas, Oportunidades e Vendedores da Marketo Engage.
* **Suporte para tipos de dados &quot;ocultos&quot; no Forms**: fornece a capacidade de gerenciar campos de formulário ocultos por meio da API.
* **Suporte a Vários Valores de Comparação para isNot Form via Regras**: gerencie a visibilidade dos campos de formulário com base no fato de o valor de outro campo não ser um dos valores de uma determinada lista.
* **Permitir configuração de Valores de Exibição e Enviados em Listas de Seleção Separadamente**: Defina separadamente o valor de exibição e o valor de envio em um campo. Por exemplo, mostrar o nome de um hotel, mas enviar uma ID interna para o back-end.
* **Permitir Configuração de Desabilitar Rastreamento Aberto em Criar ou Atualizar Email**: criar um email com rastreamento aberto desabilitado.

## Anúncios

**Exclusividade e Verificação de Email**: a partir de abril, a implantação da Verificação de Email começará. Nesse momento, os endereços de email de usuários do Marketo Engage exigirão verificação e exclusividade (isso não se aplica aos usuários somente da API). Os usuários autenticados do serviço de diretório terão seus emails verificados automaticamente quando a assinatura for habilitada com a Verificação de email.

A Verificação de email para assinaturas que usam o recurso &quot;[!UICONTROL Logon na Caixa de Diálogo de Convite de Usuário]&quot; ou que têm um único email associado a vários usuários coincidirá com o lançamento de maio. As assinaturas com um único email associado a vários usuários serão ativadas com a Verificação de email e exigirão que esses usuários resolvam o conflito e usem um email exclusivo por usuário. Quando o recurso &quot;Logon na caixa de diálogo de usuário do convite&quot; estiver habilitado, os usuários convidados por meio desse recurso precisarão ter um endereço de email exclusivo. Para usuários somente API convidados por meio desse recurso, o endereço de email não precisa ser exclusivo.

**Alteração no Comportamento da Pasta de Arquivos Mortos**: com esta versão, a capacidade de criar novos ativos em pastas de Arquivos Mortos não estará mais disponível nos menus de contexto da árvore. As opções de menu para criar novos ativos estarão ocultas para todos os ativos. [Saiba mais aqui](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_Webinar de lançamento de produto_**

[Webinário da versão de março e maio de 2022 do Marketo Engage](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## Junho de 2022 {#june}

Abaixo você encontrará todos os recursos incluídos na versão de junho de 2022. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

Os recursos a seguir serão lançados em **24 de junho de 2022**, com uma implantação em fases dos recursos restantes nas semanas seguintes (a menos que especificado de outra forma).

## Ambiente de dados de marketing

* **Expor campos CreatedAt/UpdatedAt para Objetos Personalizados**: oferece a capacidade de inspecionar esses campos na tela de Detalhes da pessoa para obter insight adicionais.

## Orquestração entre canais

* **Usabilidade de Stream Designer aprimorada para[!DNL Dynamic Chat]**: adicione cartões diretamente da tela Stream Designer sem a necessidade de arrastar e soltar. A interface do [!DNL Dynamic Chat] também foi aprimorada para oferecer melhor visibilidade do conteúdo em cartões individuais.

* **Regras Avançadas de Roteamento de Compromissos para[!DNL Dynamic Chat]**: [!DNL Dynamic Chat] oferece mais opções de roteamento de compromissos direcionados. Especifique quais compromissos de agente devem ser encaminhados com base nos atributos do Marketo Engage, garantindo que os clientes potenciais sejam encaminhados aos agentes apropriados.

* **Relatórios de Caixa de Diálogo Avançada para[!DNL Dynamic Chat]**: visualize o desempenho de suas campanhas do [!DNL Dynamic Chat] com mais detalhes usando visualizações de dados totalmente novas para métricas de envolvimento e conversão.

* **Dessincronizar Atributos do Marketo Engage Não Utilizados para[!DNL Dynamic Chat]**: Dessincronize os atributos do Marketo Engage da sua assinatura do [!DNL Dynamic Chat] que não são utilizados, ajudando a facilitar a limpeza dos dados e permitindo que os atributos alternativos sejam sincronizados conforme necessário.

## Experiência da próxima geração

**Novos Modos de Exibição de Alternância**: os modos de exibição abaixo agora estão disponíveis na Experiência da Próxima Geração:

* [Exibição de detalhes do email](https://experienceleague.adobe.com/en/docs/marketo/using/home?lang=pt-BR){target="_blank"}
* [Exibição da lista de emails](https://experienceleague.adobe.com/en/docs/marketo/using/home?lang=pt-BR){target="_blank"}

## Automação de experiência

* **Exclusões de Regra de Validação do Campo de Formulário Global**: exclua formulários específicos das Regras de Validação do Formulário Global para que as centrais de assinaturas e outros fluxos de trabalho críticos comerciais possam aceitar todos os valores.

* **Etapas de fluxo de autoatendimento**: expanda a conectividade entre o Marketo Engage e o restante da pilha com a capacidade de criar etapas de fluxo personalizadas para uso em Campanhas inteligentes. Os usuários e parceiros da Marketo Engage podem aproveitar essa funcionalidade para permitir o uso de serviços Web externos em Campanhas de acionador, em lote e de executável, em contraste com Webhooks, que só podem ser usados em Campanhas de acionador.

* **Rastreamento de link agnóstico de protocolo do Munchkin**: estenda o suporte ao rastreamento de links `tel` e `mailto` com o Munchkin para rastrear um conjunto expandido de comportamentos da Web.

* **Métodos HTTP adicionais para webhooks**: especifique PUT, PATCH e DELETE como tipos de solicitação para interagir com serviços Web.

## [!DNL Sales Insight]

![(estrela)](assets/yellow-star.png)

* Conjunto de Permissões **[!DNL Sales Insight]em[!DNL Salesforce]**: Os administradores podem fornecer acesso de [!DNL Sales Insight] a um conjunto limitado de pessoas no nível de usuário, em vez do nível de perfil, por meio do conjunto de permissões do Aplicativo Marketo, que faz parte do pacote [!DNL Sales Insight] [!DNL Salesforce].

* **Atualização do Meu Bloco do Marketo - [!DNL Sales Insight] Ações**: os Administradores do Marketo (e os usuários que eles designarem) agora podem navegar rapidamente para a instância de Ações do [!DNL Sales Insight] por meio de um novo bloco de Ações do [!DNL Sales Insight], localizado na página Meu Marketo.

## [!DNL Sales Connect]

![(estrela)](assets/yellow-star.png)

* **[!DNL Salesforce]Atualização da API**: com a versão do verão de 2022 do [!DNL Salesforce], as versões herdadas da API de 21 a 30 não serão mais suportadas pelo [!DNL Salesforce]. Com esta versão do Marketo Engage, todas as [!DNL Sales Connect] solicitações que usam versões de API herdadas foram atualizadas para permanecer em uma versão com suporte. Para obter detalhes completos sobre os planos de aposentadoria da API [!DNL Salesforce], clique [aqui](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}.

## Aprimoramentos na API

* **Novos recursos de filtragem para API de Extração de Membro de Programa em Massa**: filtre por status de associação de programa, updatedAt, cadência ou conteúdo esgotado para refinar o conjunto de dados extraído.

* **Aprimoramento da API de Extração de Membro de Programa em Massa**: especifique até 10 programas durante a criação do trabalho para melhorar a taxa de transferência.

## Anúncios

* **Substituição do Forms - Forms 1.0, ponto de extremidade de captura/salvamento de clientes potenciais e versões sem script de formulários**: o suporte para ativos do Forms 1.0 será completamente removido do Marketo Engage até outubro de 2022. Todos os ativos existentes do Forms 1.0 deixarão de funcionar. Os formulários do Marketo Engage exigirão que o JavaScript seja carregado nas páginas de aterrissagem e sites.

**_Webinar de lançamento de produto_**

[Webinário da versão de junho e agosto de 2022 do Marketo Engage](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## Agosto de 2022 {#august}

Abaixo você encontrará todos os recursos incluídos na versão de agosto de 2022. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

Os recursos a seguir iniciaram uma implantação em fases em **26 de agosto de 2022**.

## Orquestração entre canais

* Habilitar/Desabilitar Todas as Caixas de Diálogo Publicadas de Uma Vez para [!DNL Dynamic Chat]**: habilite/desabilite globalmente todas as caixas de diálogo publicadas de uma só vez na página Configuração, pressionando um botão.

* **Avatares personalizados para[!DNL Dynamic Chat]**: carregue um avatar de chatbot personalizado para que ele possa ser personalizado para sua marca.

* **Transcrições de chat para[!DNL Dynamic Chat]**: visualize as transcrições de chat para cada conversa a fim de obter uma insight mais profunda sobre o que interessa a cada visitante da Web.

## Experiência da próxima geração

* **Marca da Adobe**: aparência e comportamento atualizados para editores e página de detalhes da pessoa com a nova marca Adobe Experience Cloud.

* **Exibir a Hierarquia de Pastas da Pasta de Destino na Caixa de Diálogo de Movimentação**: a exibição da hierarquia de pastas para cada pasta facilita a movimentação de ativos e reduz a probabilidade de colocá-los na pasta errada.

* **[Screens Atualizado na Experiência da Próxima Geração](https://experienceleague.adobe.com/en/docs/marketo/using/home?lang=pt-BR){target="_blank"}**: estamos fornecendo telas adicionais e atualizadas na experiência da próxima geração, que oferecem um design atualizado e melhorias de usabilidade acessíveis através do switch de alternância:

  * Detalhes do trecho
  * Detalhes de &quot;Imagens e arquivos&quot;

>[!NOTE]
>
>A exceção é mover um ativo para uma pasta em um programa em Atividades de marketing. Essa ação de mover não exibirá a hierarquia de pastas, pois as pastas em um programa não podem ter nomes duplicados.

## Automação de experiência

* **[Etapas de Fluxo de Autoatendimento - Melhorias na Importação de Programas](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/flow-step-service.md){target="_blank"}**: suporte aprimorado para a importação de programas com etapas de fluxo personalizadas, onde agora você pode usar várias instâncias do mesmo provedor de serviços e importar programas que tenham etapas de fluxo compatíveis com esses provedores de serviços.

* **[!DNL Munchkin]- Rastreamento de link expandido**: estenda o suporte ao rastreamento de links `tel` e `mailto` com o Munchkin para rastrear um conjunto expandido de comportamentos da Web.

* **Visibilidade do cabeçalho personalizado do Webhook**: os cabeçalhos personalizados do Webhook agora são exibidos na guia [!UICONTROL Admin] > [!UICONTROL Webhooks] para melhorar a visibilidade.

* **CAPTCHA**: avalie a validade de envios de formulário [usando reCAPTCHA v3](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"} para pontuar o tráfego de formulário de entrada. Crie fluxos de trabalho de marketing para excluir, colocar em quarentena ou excluir automaticamente tráfego de bot suspeito.

* **Permissão para Aprovar o Formulário**: nova permissão para controlar quais designers podem aprovar alterações em um formulário de acordo com outros ativos do [!UICONTROL Design Studio]. Isso impede que outros designers enviem alterações para formulários sem que outra pessoa com permissão de aprovação as revise.

* **Sempre Executar Repetição da Campanha Após Mesclagem Anônima**: a mesclagem anônima de clientes potenciais ocorre antes da repetição da campanha, portanto, os filtros de campo personalizados se comportam de forma confiável quando a repetição anônima da campanha é feita.

## Ambiente de dados de marketing

* **Corrigir truncamento de Objeto Personalizado &quot;[!UICONTROL Usado por]&quot; campos** na interface do usuário: agora é mais fácil identificar campos de objeto personalizado que estão &quot;em uso&quot; para que você possa excluir campos de um Objeto Personalizado quando necessário.

## Aprimoramentos na API

* **Novos Recursos de Filtragem para API de Extração de Membro de Programa em Massa**: filtre por status de associação de programa, updatedAt, cadência ou conteúdo esgotado para refinar o conjunto de dados extraído.

## [!DNL Sales Insight]

![(estrela)](assets/yellow-star.png)

* **[[!DNL Sales Insight] Integração com o [!DNL Dynamic Chat]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}**: visualize as atividades do [!DNL Dynamic Chat] no painel [!DNL Sales Insight] e aproveite esse novo ponto de dados em seu esforço de prospecção.

## Anúncios

**_Webinar de lançamento de produto_**

[Webinário da versão de junho e agosto de 2022 do Marketo Engage](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## Outubro de 2022 {#october}

Abaixo você encontrará todos os recursos incluídos na versão de outubro de 2022. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os seguintes recursos se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **sábado, 14 de outubro de 2022**, com uma implementação gradual dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique abaixo cada recurso para obter seu status.

### Ambiente de dados de marketing

</br>

* **Sincronização de Campo Personalizado de Membro do Programa**: capacidade de sincronizar bidirecionalmente campos extensíveis capturados para um membro do programa (por exemplo, preferências de participante durante o registro do evento, como alimentação, sessões, controles etc.) com campos de membro do Campaign no Salesforce.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md">Sincronizar campos personalizados de membros de programas</a></td>
  </tr>
  </tbody>
</table>

* **Integração do Adobe Privacy Service**: harmonize com o Privacy Service para automatizar a conformidade com as regulamentações de privacidade de dados em todos os produtos da Experience Cloud. Atualmente, esse serviço está disponível somente para clientes do Marketo Engage que integraram o Adobe Identity Management System.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">Adobe Identity Management</a></td>
  </tr>
  </tbody>
</table>

### Experiência da próxima geração

</br>

* **Screens atualizado na Experiência da Próxima Geração**: estamos fornecendo telas adicionais e atualizadas na experiência da próxima geração, que oferecem um design atualizado e aprimoramentos de usabilidade acessíveis via switch de alternância:

  * Detalhes do modelo de página de destino
  * Lista de modelos de email

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/home?lang=pt-BR">Botão de alternância</a></td>
  </tr>
  </tbody>
</table>

* **Aprimorado Usado pela guia em Detalhes do modelo de email**: na nova experiência do, você verá informações adicionais relacionadas aos ativos que usam o modelo de email, incluindo Status do ativo, Última modificação e Última modificação por. Também é possível pesquisar, classificar e filtrar a lista de usados por ativos.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>

* **Modais de filtro de ativo de relatório**: novo design para modelos de configuração de relatório exibindo uma nova árvore de ativos no menu de configuração e um filtro para Data de criação e modificação.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>

### Aprimoramentos na API

</br>

* **Importação de Cliente Potencial em Massa: associação de Vendedor**: paridade com a API REST de Cliente Potencial para poder associar clientes potenciais a Vendedores durante o processo de importação de cliente potencial em massa, reduzindo a complexidade e o número de chamadas de API necessárias.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/mapi/#tag/Bulk-Import-Leads">Importação de leads em massa</a></td>
  </tr>
  </tbody>
</table>

### Sales Insight

</br>

![(estrela)](assets/yellow-star.png)

* **Integração do Sales Insight com o Dynamic Chat**: o Painel de Insights agora inclui atividades do Dynamic Chat na Grade Inteligente junto com um resumo semanal e cartões de detalhes.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Integração ao Dynamic Chat</a></td>
  </tr>
  </tbody>
</table>

## Recursos da versão Agile

Os seguintes recursos seguem um formato Agile e são lançados em várias datas antes ou depois da data de lançamento padrão. Verifique abaixo cada recurso para obter seu status.

* **Fluxos de Caixa de Diálogo de Organização Automática para Dynamic Chat**: Melhore sua tela de Caixa de Diálogo lotada organizando tudo na tela em um formato limpo e fácil de ler com o pressionamento de um botão por meio da Organização Automática.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-icons">Ícones de Designer de fluxo</a></td>
  </tr>
  </tbody>
</table>

* **Links de Reunião para Dynamic Chat**: opção para incluir automaticamente um link de Equipes ou Reunião para Google e Outlook em cada convite de calendário enviado aos visitantes.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md">Calendário</a></td>
  </tr>
  </tbody>
</table>

* **Suporte a tipos de dados adicionais para o Dynamic Chat**: três novos tipos de dados (booleano, inteiro, flutuante) permitem que você aproveite mais campos existentes do Marketo Engage no Dynamic Chat para coisas como direcionamento com base em pontuações ou fazer perguntas aos visitantes sim/não.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>

## Anúncios

* **Forms 1.0**: a descontinuação do Forms 1.0 será concluída com a versão de outubro. Os ativos do Forms 1.0 não poderão mais enviar dados para o Marketo Engage e retornarão erros se forem tentados.

* **No-Script Forms**: o Forms não funcionará mais quando o Javascript estiver desabilitado no navegador. O envio do formulário exigirá que o Javascript esteja habilitado.
