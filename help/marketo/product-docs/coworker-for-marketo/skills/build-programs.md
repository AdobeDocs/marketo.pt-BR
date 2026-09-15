---
description: Use o Colaborador para o Marketo Engage para criar um programa do Marketo adaptando um modelo existente. Prepare campanhas inteligentes, agendamento e espaços reservados para ativos para revisar e refinar.
title: Criar programas
source-git-commit: 0949e5193333d56943a5c9a52c1715ecbcb274f3
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%
---
# Criar programas {#build-programs}

Descreva uma campanha de marketing em linguagem simples. O Co-worker para Marketo Engage adapta um modelo de programa existente para atender às suas necessidades, atualizando automaticamente o conteúdo do email e criando ativos adicionais duplicando a estrutura do modelo.

>[!PREREQUISITES]
>
>* Para usar esse recurso, primeiro você deve concordar com os [termos principais da Gen-AI e os termos complementares](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Entre em contato com a Equipe de conta da Adobe (seu gerente de conta) para obter detalhes.
>
>* Você deve ter permissão para criar programas em sua conta do Marketo e ter pelo menos um programa existente do Marketo para usar como modelo. O programa de modelo deve conter pelo menos um email e uma Campanha Inteligente.

## Como usar {#how-to-use}

1. Em Meu Marketo, clique no bloco **Colaborador do Marketo Engage**.

1. Selecione um programa modelo. Escolha um programa existente que corresponda ao seu tipo de campanha (por exemplo, Email, Webinário, Preparação).

1. Na janela do prompt, digite uma descrição da campanha que deseja criar. Seja tão específico ou tão geral quanto você deseja (você sempre pode refinar).

1. O colaborador do Marketo Engage confirma a interpretação do seu resumo e lista o que ele planeja criar. Analise isso antes de criá-lo.

1. Confirme e o Co-worker para Marketo Engage cria o programa em seu ambiente.

1. Abra o programa recém-criado no Marketo e revise a estrutura.

1. Substitua os ativos de email de espaço reservado pelo seu conteúdo real.

1. Verifique se os filtros do Smart Campaign e as etapas de fluxo correspondem ao público-alvo e à lógica desejados.

1. Após concluir todos os refinamentos manuais (configurar a lógica do Smart Campaign, finalizar filtros, personalizar o conteúdo do email), execute [Validar programas](/help/marketo/product-docs/coworker-for-marketo/skills/validate-programs.md) para garantir que suas alterações estejam em conformidade com as Regras Organizacionais antes da ativação.

## Casos de uso {#use-cases}

**Programa de registro em webinários**: um gerente de campanha digita &quot;Crie um programa de registro em webinário para nossa demonstração de produto em agosto. Envie um email de convite, um lembrete no dia anterior e um acompanhamento com o link de gravação depois.&quot; O colega de trabalho do Marketo Engage cria um programa com três Campanhas inteligentes (convite, lembrete, acompanhamento), emails de espaço reservado para cada uma e agendamento com base na data do evento.

**Campanha do acionador de pontuação do lead**: um especialista em operações de marketing digita &quot;Criar um programa que é acionado quando um lead atinge uma pontuação de 50 e o envia para uma Lista inteligente MQL.&quot; O colaborador do Marketo Engage cria o programa com um acionador de campanha que acompanha a alteração de pontuação e uma etapa de fluxo que adiciona o lead à lista MQL.

**Promoção de reengajamento**: um gerente de geração de demanda solicita uma série de reengajamento de 3 emails direcionada a clientes potenciais que não se engajaram em 90 dias. O colaborador do Marketo Engage cria a campanha em lote com o filtro de inatividade, três etapas de envio de email com etapas de espera apropriadas entre elas e uma etapa de fluxo para atualizar o status do lead se alguém se envolver novamente.

**Programa de acompanhamento de eventos**: depois de uma feira de negócios, um gerente pede ao Colaborador para que a Marketo Engage crie um programa de acompanhamento pós-evento que envie um email de agradecimento aos participantes e um email de erro para inscritos que não apareceram. O colaborador do Marketo Engage cria duas Campanhas inteligentes, uma para cada segmento, com os filtros e espaços reservados para email corretos.

>[!NOTE]
>
>Em cada exemplo acima, o Colaborador clona um modelo de programa existente (um simples programa de email ou evento com estrutura básica) e cria os emails e campanhas adicionais duplicando os ativos do modelo e atualizando seu conteúdo. As etapas e os filtros do fluxo do Campanha inteligente são adaptados sempre que possível, mas podem exigir refinamento manual para corresponder à lógica da campanha específica.

## Itens a serem observados {#things-to-note}

* Tenha uma ideia clara do que a campanha deve fazer, quem é o público-alvo, que ação aciona (ou se é um envio em lote) e qual é o objetivo.
* A seleção do modelo é obrigatória. Escolha um template com pelo menos um email e uma Campanha Inteligente. A ferramenta não pode funcionar com modelos vazios.
* O conteúdo de email é gerado automaticamente, mas os filtros e as etapas de fluxo do Smart Campaign permanecem manuais. Você deve configurar a lógica após a criação para corresponder ao comportamento pretendido da campanha.
* Os ativos adicionais são criados por duplicação. Se o breve chamar quatro emails, mas o modelo tiver um, a ferramenta criará três duplicatas. Revise todas para garantir a consistência; elas herdam o design e a estrutura do modelo.
* O colega de trabalho do Marketo Engage não pode acessar suas listas de público-alvo existentes automaticamente. Você deve configurar manualmente os filtros da Smart List para direcionar os segmentos reais após a criação do programa.
* Programas complexos de várias etapas com lógica de ramificação avançada podem precisar de refinamento manual após a criação.
* Se o ambiente do Marketo usa convenções de nomenclatura ou estruturas de pastas, especifique-as no seu resumo para que o programa seja criado no lugar certo.
