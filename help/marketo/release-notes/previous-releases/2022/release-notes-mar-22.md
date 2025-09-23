---
description: Notas de versão - março de 2022 - Documentação do Marketo - Documentação do produto
title: Notas de versão - Março de 2022
exl-id: 91826d56-a38e-44af-b798-17bfc016c311
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 4%

---

# Notas de versão: março de 2022 {#release-notes-mar-22}

Os seguintes recursos estão incluídos na versão de março de 2022. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

**_Versões Trimestrais_**

Os recursos a seguir serão lançados em **11 de março de 2022**, com uma implantação em fases de cada recurso nas semanas seguintes (a menos que especificado de outra forma).

## Orquestração entre canais {#cross-channel-orchestration}

* **[!DNL Dynamic Chat]**: maximize todas as oportunidades em seu site direcionando clientes em potencial e contas com conversas proativas, envolventes e personalizadas de 1:1. O [Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} permite que os usuários do Marketo Engage comecem a aproveitar o chat como parte essencial das experiências integradas entre canais para casos de uso de marketing e vendas B2B. Os recursos incluem: a capacidade de reservar reuniões diretamente no chat, roteamento de leads, modelos iniciais, criação de conversas com o método arrastar-e-soltar e muito mais. O Dynamic Chat está incluído em todos os pacotes do Marketo Engage e será lançado para todos os usuários do Marketo Engage este ano.

* **Aprimoramento da Filtragem de atividade de bot por email**: como aprimoramento do recurso [Filtragem de atividade de bot por email](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"} lançado anteriormente, agora é possível aceitar atividades de registro identificadas como bots. Em seguida, você pode filtrar e acionar ações com base em atividades identificadas como executadas por bots.

## Experiência de última geração {#modern-ux}

* **Screens atualizado na Experiência da Próxima Geração**: estamos fornecendo telas adicionais e atualizadas na experiência da próxima geração, que oferecem um design atualizado e aprimoramentos de usabilidade acessíveis via switch de alternância:

   * Exibição de Lista de Formulários no [!UICONTROL Design Studio] (incluindo novas ações em massa)

* **Atualização do Fluxo de Trabalho do Programa de Importação**: o fluxo de trabalho do programa de importação está sendo fornecido na experiência de próxima geração com um design atualizado e melhorias na usabilidade. Essa será uma alteração automática sem um switch de alternância.

* **Controle de Administração para o Switch de alternância da experiência da próxima geração**: gerencie a implantação da experiência da próxima geração de uma forma que funcione para seus usuários com a capacidade de os administradores selecionarem quais tipos de usuários poderão acessar o switch de alternância.

## Automação de experiência {#experience-automation}

* **Etapas de Fluxo de Autoatendimento (Beta)**: expanda a conectividade entre o Marketo Engage e o restante da pilha com a capacidade de criar etapas de fluxo personalizadas para uso em Campanhas Inteligentes. Tanto os usuários quanto os parceiros da Marketo podem aproveitar essa funcionalidade para permitir o uso de serviços Web externos em campanhas em lote e executáveis, em contraste com webhooks, que só podem ser usados em campanhas de acionador.

* **Expiração do ativo**: mantenha o controle dos ativos e campanhas com detecção de hora com a capacidade de agendar a desativação automática em uma data e hora especificadas na experiência do usuário do Classic.

* **Substituição de Prioridade de Campanha Inteligente**: certifique-se de que as Campanhas Inteligentes de acionador de alta prioridade sejam executadas o mais rápido possível com a capacidade de substituir a classificação de prioridade de campanha padrão. As Campanhas inteligentes de acionador de prioridade mais baixa também podem ter prioridade mais baixa para liberar recursos de processamento para outras tarefas de prioridade mais alta.

## Aprimoramentos na API {#api-enhancements}

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

## [!DNL Sales Connect] {#sales-connect}

![(estrela)](assets/yellow-star.png)

* **Limitação da Conexão de Email (GA)**: a Limitação da Conexão de Email permite que administradores do [!DNL Sales Connect] configurem a taxa de envio de emails ao usar o Gmail ou o [!DNL Exchange] como canal de entrega, para que a taxa na qual os emails sejam entregues ao provedor de canal de entrega não exceda os limites impostos.

## Anúncios {#announcements}

* **Descontinuação do Marketo Sky**: em março, o Marketo Sky não estará mais disponível, pois concentraremos nossos recursos no fornecimento da experiência de usuário da próxima geração. Em um esforço para manter o acesso a uma funcionalidade exclusiva do Marketo Sky hoje, estamos trazendo a Expiração de ativos e a Substituição de prioridade da Campanha inteligente para a experiência Clássica. [Clique aqui](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) para saber mais.

**_Webinar de lançamento de produto_**

[Webinar da versão de março e maio de 2022 do Marketo Engage](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
