---
description: Notas de versão - março de 2022 - Documentação da Marketo - Documentação do produto
title: Notas de versão - março de 2022
exl-id: 91826d56-a38e-44af-b798-17bfc016c311
source-git-commit: 85e04fb8a52a417982014bc4bb101b6044e53f84
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 1%

---

# Notas de versão: Março de 2022 {#release-notes-mar-22}

Os seguintes recursos estão incluídos na versão de 22 de março. Verifique sua edição do Adobe Marketo Engage para ver a disponibilidade dos recursos.

>[!AVAILABILITY]
>
>Recursos indicados por uma estrela (![star](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante de Marketo Engage para saber mais.

**_Versões trimestrais_**

Os seguintes recursos começarão a ser lançados em **11 de março de 2022**, com uma implantação em fases de cada recurso nas semanas seguintes (salvo indicação em contrário).

## Orquestração entre canais {#cross-channel-orchestration}

* **Bate-papo dinâmico**: Maximize todas as oportunidades em seu site, direcionando clientes potenciais e contas com conversas pró-ativas, envolventes e personalizadas 1:1. [Bate-papo dinâmico](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target=&quot;_blank&quot;} permite que os usuários do Marketo Engage comecem a utilizar o chat como parte essencial das experiências integradas entre canais para casos de uso de marketing e vendas B2B. Os recursos incluem: a capacidade de reservar reuniões diretamente no chat, roteamento de clientes potenciais, modelos iniciais, criação de conversas de arrastar e soltar e muito mais. O Dynamic Chat é incluído em todos os pacotes de Marketo Engage e será lançado para todos os usuários do Marketo Engage este ano.

* **Aprimoramento da Filtragem de Atividade de Bot de Email**: Como um aprimoramento da versão lançada anteriormente [Filtragem da atividade de bot de email](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md)recurso {target=&quot;_blank&quot;}, agora você pode aceitar o registro de atividades identificadas como bots. Em seguida, você pode filtrar e acionar ações com base em atividades identificadas como sendo executadas por bots.

## Experiência da próxima geração {#modern-ux}

* **Telas atualizadas na experiência de próxima geração**: Estamos fornecendo telas adicionais e atualizadas na experiência da próxima geração que oferecem melhorias atualizadas de design e usabilidade acessíveis por meio do switch de alternância:

   * Exibição de lista de formulários no Design Studio (incluindo novas ações em massa)

* **Importar Atualização do Fluxo de Trabalho do Programa**: O fluxo de trabalho do programa de importação está sendo entregue na experiência da próxima geração com melhorias atualizadas de design e usabilidade. Isso será uma alteração automática sem uma chave de alternância.

* **Controle de administração para o switch de alternância de experiência de próxima geração**: Gerencie a implantação da experiência de próxima geração de uma maneira que funcione para seus usuários com a capacidade de os administradores selecionarem quais tipos de usuário podem acessar o switch de alternância.

## Automação de experiência {#experience-automation}

* **Etapas do Fluxo de Autoatendimento (Beta)**: Expanda a conectividade entre o Marketo Engage e o resto da pilha com a capacidade de criar etapas de fluxo personalizadas para uso em Campanhas inteligentes. Os usuários e parceiros da Marketo podem aproveitar essa funcionalidade para permitir o uso de serviços da Web externos em campanhas em lote e executáveis, em contraste com webhooks, que só podem ser usados em campanhas do acionador.

* **Expiração do ativo**: Mantenha o controle de seus ativos e campanhas sensíveis ao tempo com a capacidade de agendar sua desativação automática em uma data e hora especificadas na experiência do usuário do Classic.

* **Substituição de prioridade da campanha inteligente**: Certifique-se de que o acionador de alta prioridade Campanhas inteligentes seja executado assim que possível com a capacidade de substituir a classificação de prioridade da campanha padrão. O acionador de prioridade mais baixa Campanhas inteligentes também pode ser reduzido com prioridade para liberar recursos de processamento para outras tarefas de alta prioridade.

## Melhorias da API {#api-enhancements}

* **Retornar Desativar Status de Rastreamento Aberto de Emails**: Permite a leitura do status de rastreamento aberto de emails por API
* **Recuperar linhas de assunto do conteúdo dinâmico do email**: Permite que os profissionais de marketing executem análises de linhas de assunto dinâmicas em ferramentas de BI
* **CRUD de Campos Personalizados do Membro do Programa**: Permite que os profissionais de marketing criem programaticamente campos personalizados de membros do programa
* **Exportação de objeto personalizado em massa atualizada no filtro**: Permite que os profissionais de marketing sincronizem programaticamente objetos personalizados
* **Configuração de início do cabeçalho de exposição para programas de email**: Permite que os profissionais de marketing configurem programas de email com início direto via API
* **Atualização seletiva de tag do programa**: Permite que os profissionais de marketing enviem atualizações de tags seletivas sem enviar todas as tags ao mesmo tempo
* **Campo actionResult de extração de atividade em massa**: Permite que os profissionais de marketing identifiquem quais atividades foram ignoradas ou falharam

**_Lançamento em todo o trimestre_**

Os seguintes recursos estão em um ciclo não trimestral e serão lançados nos próximos meses.

## Bizible {#bizible}

![(estrela)](assets/yellow-star.png)

* **Modelos BI**: A Bizible agora fornecerá artefatos de relatórios fundamentais e baixáveis e relatórios de amostra para o Tableau e o Power BI para permitir o rápido desenvolvimento de relatórios personalizados, adaptados às suas necessidades comerciais específicas.

## SalesConnect {#sales-connect}

![(estrela)](assets/yellow-star.png)

* **Limitação da conexão de email (GA)**: A Limitação da conexão de email permite que os administradores do Sales Connect configurem a taxa de envio de emails ao usar o Gmail ou o Exchange como seu canal de delivery, de modo que a taxa na qual os emails são entregues ao provedor de canal de delivery não exceda os limites impostos.

## Anúncios {#announcements}

* **Descontinuação do Marketo Sky**: Em março, o Marketo Sky não estará mais disponível à medida que concentramos nossos recursos no fornecimento da experiência do usuário da próxima geração. Em um esforço para manter o acesso à funcionalidade que é exclusiva do Marketo Sky hoje, estamos trazendo a Expiração de ativos e a Substituição de prioridade de campanha inteligente para a experiência clássica. [Clique aqui](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) para saber mais.

**_Webinar da versão do produto_**

[Webinar de lançamento do Marketo Engage de março e maio de 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target=&quot;_blank&quot;}
