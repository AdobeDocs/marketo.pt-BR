---
unique-page-id: 12983280
description: Notas de versão - Último trimestre de 2017 - Documentação do Marketo - Documentação do produto
title: Notas de versão - Último trimestre de 2017
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 11%

---

# Notas de versão: outono de 17 {#release-notes-fall}

Os seguintes recursos estão incluídos na versão do último trimestre de 2017. Verifique a edição do Marketo quanto à disponibilidade de recursos.

Clique nos links de título para exibir artigos detalhados para cada recurso. Observação: alguns dos recursos incluídos nesta versão não têm artigos associados. Se um tópico tiver vários subtítulos, os links serão colocados lá.

## Confiabilidade do sistema {#system-reliability}

Fizemos melhorias adicionais na infraestrutura principal do Marketo, incluindo melhor sequenciamento, menos incompatibilidades e melhora a estabilidade do Munchkin.

## Carimbo de sincronização SFDC {#sfdc-sync-performance}

Aproveite a sincronização mais avançada e rápida no Marketo e Salesforce. As alterações de dados que exigem atualizações em massa em contas ou leads podem ser divididas em filas paralelas para evitar backlogs. Agora, os eventos e as tarefas também são sincronizados até 50% mais rápido.

## Melhorias no desempenho de análises {#analytics-performance-improvements}

As melhorias recentes na infraestrutura oferecem maior tempo de atividade e estabilidade nas ferramentas de análise e relatórios do Marketo, permitindo criar relatórios ad hoc mais rapidamente.

## [Fuso horário do destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

Com esse novo recurso, agora é possível reter e entregar emails de acordo com fusos horários locais. Os programas de email e de engajamento podem ser configurados para serem entregues nos fusos horários dos destinatários, eliminando a necessidade de criar vários programas. Envie uma vez e a Marketo manterá o email automaticamente até o horário local correto. Erga as métricas de email, observe as práticas locais e economize tempo usando um único programa globalmente.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Se você ainda não conseguir ativar o Fuso horário do destinatário em seus programas de email e engajamento, não entre em pânico! Estamos habilitando gradualmente esse recurso para todos os clientes.

## [Analisar os e-mails de amostra por segmento](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

O Marketo tem uma nova opção para escolher um segmento ao enviar emails de amostra para revisão. Não é mais necessário determinar manualmente a qual segmento um lead pertence, facilitando o envio de emails com conteúdo dinâmico para segmentos diferentes.

## [Perguntas personalizadas para geração de leads do LinkedIn](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

Personalize seus formulários de geração de leads do LinkedIn para coletar atributos personalizados dos leads. Agora é possível fazer até três perguntas personalizadas por formulário, escolher entre uma entrada de texto de linha única ou perguntas de múltipla escolha e mapear de volta aos campos de cliente potencial do Marketo.

## Integração do Slack {#slack-integration}

Lançamos dois recursos como parte de nossa nova integração de Slack:

* Notificações do sistema: receba notificações Slack sobre eventos importantes na instância do Marketo, como alertas sobre status atuais da campanha e qualquer problema que exija atenção imediata.
* Momentos interessantes: quando um Marketo Insight é acionado por um indivíduo conhecido de uma conta de vendas, os proprietários principais podem ser notificados por meio do Slack. As notificações incluem informações de cliente potencial, bem como detalhes sobre a conta de vendas.

## Aprimoramentos de ABM {#abm-enhancements}

**[Mostrar contas sem contatos](https://docs.marketo.com/x/fKCt)**

O Marketo ABM agora sincroniza e exibe contas do CRM sem contatos. Inclua novas contas sem histórico de vendas ou marketing anterior e rastreie o progresso correspondendo clientes em potencial subsequentes às contas.

## Análises do ContentAI {#contentai-analytics}

**[Novo filtro para lista de contas ABM](https://docs.marketo.com/x/1BPG)**

Visualize e compare o desempenho do conteúdo nas Listas de contas do ABM para otimizar o conteúdo existente. A IA de conteúdo mostra:

* principal conteúdo exibido
* principais conteúdos convertidos
* Conteúdo sugerido habilitado por IA para atividades de marketing

## Aprimoramentos de personalização da web {#web-personalization-enhancements}

**[Tokens para campanhas on-line](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Os tokens agora estão disponíveis para uso em campanhas da Web. Aproveite os tokens para fornecer mensagens e conteúdo personalizados para aumentar a participação em suas campanhas da Web.

![](assets/image2017-11-16-11-3a25-3a7.png)

**[Imagens do estúdio de desenvolvimento no editor de campanhas on-line](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Economize tempo reutilizando ativos criativos e imagens em vários canais no Marketo.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Integração  {#integration}

**[API de visualização de e-mail](https://developers.marketo.com/rest-api/assets/emails/)**

Agora você pode visualizar remotamente emails fora do Marketo, simplificando o processo de localização de conteúdo de email e reduzindo erros.

**[Substituir a API HTML](https://developers.marketo.com/rest-api/assets/emails/)**

Os desenvolvedores podem atualizar o conteúdo de HTML dos ativos de email remotamente, permitindo que trabalhem em um único sistema para manter os ativos.
