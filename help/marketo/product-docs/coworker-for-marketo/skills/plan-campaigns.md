---
description: Use o CX Enterprise Coworker for Marketo Engage para transformar um resumo da campanha em um plano de programa estruturado que abranja lógica de público-alvo, emails, tokens e verificações de controle de qualidade.
title: Planejar campanhas
source-git-commit: e72db83a5f1f3c58a29da7c4b4b1bbb79a61b596
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 0%
---
# Planejar campanhas {#plan-campaigns}

Transforme um resumo da campanha em um plano de implementação estruturado para o Marketo Engage. O plano de campanhas descreve a estrutura do programa, a lógica do público-alvo, os emails, as campanhas inteligentes, os tokens, os relatórios e as verificações de pré-ativação. A saída é um relatório baixável que aparece no painel do espaço de trabalho.

>[!NOTE]
>
>- Essa habilidade gera planos de implementação para programas do Marketo Engage (documentos estruturados que informam a um sistema humano ou de automação exatamente como criar uma campanha). Não cria nada no Marketo Engage. Há uma habilidade separada para [criar programas](/help/marketo/product-docs/coworker-for-marketo/skills/build-programs.md){target="_blank"}.
>- Esta habilidade é guiada por [Regras Organizacionais](/help/marketo/product-docs/coworker-for-marketo/organizational-rules.md){target="_blank"}.

## Pré-requisitos {#prerequisites}

- Para um plano de programa, forneça um resumo da campanha com as informações disponíveis, como metas da campanha, público-alvo, mensagens, linha do tempo e métricas de sucesso.
- Para melhorar um resumo ou plano existente, forneça o documento e descreva as alterações desejadas.
- Para começar sem um resumo, solicite um resumo de amostra ou peça um plano com base em um cenário de campanha comum.

## Como usar {#how-to-use}

1. Em Meu Marketo, clique no bloco **[!UICONTROL CX Enterprise Coworker para Marketo Engage]**.

1. Selecione a habilidade **[!UICONTROL Planejar campanhas]** e clique em **[!UICONTROL Usar esta habilidade]**.

1. Escolha o que deseja fazer:
   - Planejar um programa a partir de um resumo da campanha.
   - Gere um resumo de campanha de exemplo.
   - Polonês, um resumo existente.
   - Revise um plano de configuração existente.

1. Forneça o resumo ou documento. Inclua quaisquer alterações específicas, requisitos de campanha ou convenções organizacionais.

1. Revise o relatório gerado no painel espaço de trabalho. Abra-o para analisar os detalhes ou baixar o relatório.

1. Revise e aprove o plano de configuração antes de criar o programa no Marketo Engage.

## Opções de habilidade {#skill-options}

### Planejar um programa {#plan-a-program}

Um plano de programa traduz os requisitos da campanha em instruções para a criação do programa. Dependendo do resumo, pode incluir:

- **Visão geral do programa**: nome da campanha, objetivos, público-alvo e linha do tempo.
- **Estrutura de pastas:** pastas locais recomendadas para emails, Campanhas inteligentes e relatórios.
- **Smart Lists:** Lógica de segmentação, definições de filtros e exclusões necessárias.
- **Configuração de email:** linhas de assunto, texto de pré-cabeçalho, estrutura de conteúdo, detalhes do remetente e elementos de conformidade.
- **Campanhas inteligentes**: nomes de campanha, gatilho ou designação de lote, etapas de fluxo e recomendações de agendamento.
- **Tokens e campos:** Meus Tokens, tokens obrigatórios e personalizados e quaisquer campos personalizados necessários com seus tipos e valores.
- **Fluxo de Jornada:** Sequência de campanha, etapas de espera e lógica de decisão.
- **Relatórios e controle de qualidade:** Métricas de sucesso, relatórios recomendados e verificações de validação de pré-ativação.

### Criar um resumo de amostra {#create-a-sample-brief}

Solicite um resumo de amostra quando quiser que um exemplo se adapte. Você pode especificar um tópico ou tipo de campanha, como um lançamento de produto ou webinário. Se você solicitar um plano sem fornecer um resumo, a habilidade poderá usar um cenário de amostra, como um webinário de lançamento de produto, como a base para o plano.

### Polonês um breve ou revisar um plano {#polish-a-brief-or-revise-a-plan}

A habilidade identifica o tipo de documento a partir de seu conteúdo, em vez de depender apenas do texto de sua solicitação.

Um **resumo da campanha** geralmente descreve as metas, o público-alvo, a estratégia de mensagens, a linha do tempo e as métricas de sucesso. Um **plano de configuração** geralmente contém detalhes de implementação, como configurações de Smart List, etapas de fluxo do Smart Campaign, definições de token, especificações de email e requisitos técnicos.

Forneça o documento e as alterações solicitadas. Por exemplo, se você pedir para refinar um plano, mas fornecer um resumo da campanha, a habilidade tratará o documento como um resumo. Se você fornecer um plano de configuração e solicitar a revisão de um resumo, ele tratará o documento como um plano.

## Integração de regras organizacionais {#organizational-rules-integration}

Os documentos de configuração devem incorporar as regras de sua organização do contexto do sistema.

### Convenções de nomenclatura {#naming-conventions}

- Programas: `{{REGION}}_FY{{YEAR}}_{{QUARTER}}_{{TYPE}}_{{DATE}}_{{NAME}}`
- Emails: `{{PROGRAM_NAME}}_{{SEQUENCE}}_{{PURPOSE}}`
- Campanhas inteligentes: `{{NUMBER}}_{{TRIGGER_OR_BATCH}}_{{ACTION}}`

### Elementos obrigatórios {#required-elements}

- Três pastas locais (01 Emails, 02 Campanhas inteligentes, 03 Relatórios)
- Quatro tokens necessários (eventDate, eventTime, replyToEmail, senderName)
- Filtros de exclusão (Assinatura cancelada, Email inválido, Marketing suspenso, Incluído na lista de bloqueios)
- Conformidade de email (link de cancelamento de inscrição, endereço físico)

### Controle de qualidade de pré-ativação {#pre-activation-qa}

- Validação do padrão de nome
- Confirmação da estrutura de pastas
- Verificação de filtro de exclusão
- Verificações de elemento de conformidade

## Casos de uso {#use-cases}

**Planeje um programa de webinário:** Forneça o objetivo do webinário, o público-alvo, a linha do tempo do evento e as necessidades de mensagens. O plano de configuração pode destacar a estrutura do programa, as especificações de email, a sequência da campanha, os tokens e as verificações de controle de qualidade.

**Gerar um resumo de amostra:** Solicite um resumo de exemplo para um tipo de campanha e adapte-o aos detalhes da campanha antes de solicitar um plano de programa.

**Atualizar um plano de configuração existente:** Forneça o plano e especifique as alterações, como atualizar a linha de tempo, adicionar uma etapa da campanha ou revisar a lógica de público-alvo.

## Próximas etapas {#next-steps}

Após a conclusão de uma operação de planejamento, os prompts de acompanhamento apropriados podem incluir:

- &quot;Revisar este plano de configuração&quot;
- &quot;Obtenha um resumo de campanha de exemplo&quot;
- &quot;Criar este programa no Marketo&quot; (para criar um programa, você deve usar a habilidade [criar programas](/help/marketo/product-docs/coworker-for-marketo/skills/build-programs.md)).
