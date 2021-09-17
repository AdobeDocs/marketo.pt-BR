---
unique-page-id: 12983280
description: Notas de versão - Último trimestre de 2017 - Documentos da Marketo - Documentação do produto
title: Notas de versão - Último trimestre de 2017
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
source-git-commit: cbfa6110e85c185a5b65342052f168d9715f2f6a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Notas de versão: Último trimestre de 1917 {#release-notes-fall}

Os seguintes recursos estão incluídos na versão lançada no último trimestre de 1917. Verifique sua edição do Marketo para ver a disponibilidade dos recursos.

Clique nos links de título para exibir os artigos detalhados de cada recurso. Observação: Alguns dos recursos incluídos nesta versão não têm artigos associados. Se um tópico tiver várias subposições, as vinculações serão colocadas lá.

## Confiabilidade do sistema {#system-reliability}

Fizemos melhorias adicionais na infraestrutura principal do Marketo, incluindo melhor sequenciamento, menos incompatibilidades e melhoria da estabilidade do Munchkin.

## Carimbo de sincronização SFDC {#sfdc-sync-performance}

Aproveite a sincronização mais rica e rápida entre o Marketo e o Salesforce. As alterações de dados que exigem atualizações em massa em contas ou leads podem ser divididas em filas paralelas para evitar registros retroativos. Eventos e tarefas agora também sincronizam até 50% mais rápido.

## Melhorias no desempenho de análises {#analytics-performance-improvements}

Melhorias recentes na infraestrutura oferecem maior tempo de atividade e estabilidade nas ferramentas de relatórios e análises da Marketo, permitindo que você crie relatórios ad hoc mais rapidamente.

## [Fuso horário do destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

Com esse novo recurso, agora você pode reter e enviar emails de acordo com os fusos horários locais. Os programas de email e de envolvimento podem ser configurados para serem entregues nos fusos horários dos recipients, eliminando a necessidade de criar vários programas. Enviar uma vez e o Marketo automaticamente manterá o email até o horário local correto. Incentive as métricas de email, observe as práticas locais e economize tempo usando um único programa globalmente.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Se você ainda não conseguir ativar o Fuso horário do destinatário em seus programas de email e de envolvimento, não entre em pânico! Estamos permitindo gradualmente esse recurso a todos os clientes.

## [Analisar os e-mails de amostra por segmento](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

O Marketo tem uma nova opção para selecionar um segmento ao enviar emails de amostra para revisão. Não é mais necessário determinar manualmente a qual segmento um cliente potencial pertence, facilitando o envio de emails com conteúdo dinâmico para segmentos diferentes.

## [Perguntas personalizadas para geração de leads do LinkedIn](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

Personalize seus formulários de geração de leads do LinkedIn para coletar atributos personalizados dos leads. Agora é possível fazer até três perguntas personalizadas por formulário, escolher entre entrada de texto de uma única linha ou perguntas de múltipla escolha e mapear de volta para os campos de lead do Marketo.

## Integração do Slack {#slack-integration}

Lançamos dois recursos como parte da nova integração do Slack:

* Notificações do sistema: Obtenha notificações do Slack sobre eventos importantes em sua instância do Marketo, como alertas sobre os status atuais da campanha e quaisquer problemas que exijam atenção imediata.
* Momentos interessantes: Quando um Marketo Insight é acionado por um indivíduo conhecido de uma conta de vendas, os proprietários de leads podem ser notificados por meio do Slack. As notificações incluem informações de cliente potencial, bem como detalhes sobre a conta de vendas.

## Aprimoramentos de ABM {#abm-enhancements}

**[Mostrar contas sem contatos](https://docs.marketo.com/x/fKCt)**

O Marketo ABM agora sincroniza e exibe contas CRM sem contatos. Inclua novas contas sem histórico de vendas ou marketing anterior e rastreie o progresso ao corresponder leads subsequentes às contas.

## Análises do ContentAI {#contentai-analytics}

**[Novo filtro para lista de contas ABM](https://docs.marketo.com/x/1BPG)**

Exiba e compare o desempenho do conteúdo em Listas de contas do ABM para otimizar o conteúdo existente. O ContentAI mostra:

* conteúdo principal exibido
* conteúdo mais convertido
* Conteúdo sugerido alimentado por IA para atividades de marketing

## Aprimoramentos de personalização da web {#web-personalization-enhancements}

**[Tokens para campanhas on-line](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Agora, tokens estão disponíveis para uso em campanhas da Web. Aproveite os tokens para fornecer mensagens e conteúdo personalizados para aumentar a participação em suas campanhas da Web.

![](assets/image2017-11-16-11-3a25-3a7.png)

**[Imagens do estúdio de desenvolvimento no editor de campanhas on-line](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Economize tempo reutilizando ativos e imagens criativas em vários canais no Marketo.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Integração  {#integration}

**[API de visualização de e-mail](https://developers.marketo.com/rest-api/assets/emails/)**

Agora é possível visualizar remotamente o email fora do Marketo, simplificando o processo de localização do conteúdo do email e reduzindo erros.

**[Substituir a API HTML](https://developers.marketo.com/rest-api/assets/emails/)**

Os desenvolvedores podem atualizar o conteúdo HTML de ativos de email remotamente, permitindo que eles trabalhem em um único sistema para manter ativos.
