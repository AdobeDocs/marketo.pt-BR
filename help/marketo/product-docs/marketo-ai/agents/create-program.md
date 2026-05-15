---
description: Use a IA do Marketo para criar um programa do Marketo a partir de um resumo em linguagem simples. Obtenha campanhas inteligentes, agendamento e espaços reservados para ativos prontos para revisar e refinar.
title: Criar programa
beta: true
hide: true
source-git-commit: f552c0b0219aede39e0742466ab2473e8e924e55
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Criar programa {#create-program}

Descreva uma campanha de marketing em linguagem simples e a IA do Marketo criará a estrutura do programa, completa com espaços reservados para ativos e agendamento.

>[!PREREQUISITES]
>
>* Para usar esse recurso, primeiro você deve concordar com os [termos principais da Gen-AI e os termos complementares](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Entre em contato com a Equipe de conta da Adobe (seu gerente de conta) para obter detalhes.
>
>* Você deve ter permissão para criar programas em sua conta do Marketo.

## Como usar {#how-to-use}

1. Em Minha Marketo, clique no bloco **Criar com IA**.

1. Na janela do prompt, digite uma descrição da campanha que deseja criar. Seja tão específico ou tão geral quanto você deseja (você sempre pode refinar).

1. A IA do Marketo confirma a interpretação do resumo e lista o que ele planeja criar. Analise isso antes de criá-lo.

1. Confirme e a IA do Marketo criará o programa em seu ambiente.

1. Abra o programa recém-criado no Marketo e revise a estrutura.

1. Substitua os ativos de email de espaço reservado pelo seu conteúdo real.

1. Verifique se os filtros de campanha inteligentes e as etapas de fluxo correspondem ao público-alvo e à lógica desejados.

1. Execute o agente [Controle de qualidade do programa](/help/marketo/product-docs/marketo-ai/agents/program-qa.md) antes de ativar.

## Casos de uso {#use-cases}

**Programa de registro em webinários**: um gerente de campanha digita &quot;Crie um programa de registro em webinário para nossa demonstração de produto em agosto. Envie um email de convite, um lembrete no dia anterior e um acompanhamento com o link de gravação depois.&quot; A IA do Marketo cria um programa com três campanhas inteligentes (convite, lembrete, acompanhamento), emails de espaço reservado para cada uma e agendamento com base na data do evento.

**Campanha do acionador de pontuação do lead**: um especialista em operações de marketing digita &quot;Criar um programa que é acionado quando um lead atinge uma pontuação de 50 e o envia para uma lista inteligente MQL.&quot; A IA do Marketo cria o programa com um acionador de campanha que escuta a alteração de pontuação e uma etapa de fluxo que adiciona o lead à lista MQL.

**Promoção de reengajamento**: um gerente de geração de demanda solicita uma série de reengajamento de 3 emails direcionada a clientes potenciais que não se engajaram em 90 dias. A IA do Marketo cria a campanha em lote com o filtro de inatividade, três etapas de envio de email com etapas de espera apropriadas entre elas e uma etapa de fluxo para atualizar o status do lead se alguém se envolver novamente.

**Programa de acompanhamento de eventos**: depois de uma feira de negócios, um gerente solicita à Marketo AI que crie um programa de acompanhamento pós-evento que envie um email de agradecimento aos participantes e um email de erro para inscritos que não participaram. A IA do Marketo cria duas campanhas inteligentes, uma para cada segmento, com os filtros e espaços reservados para email corretos.

## Itens a serem observados {#things-to-note}

* Tenha uma ideia clara do que a campanha deve fazer; quem é o público-alvo, que ação aciona (ou se é um envio em lote) e qual é o objetivo.
* Nenhum modelo ou formulário é necessário antecipadamente. A IA do Marketo cria a estrutura e você pode conectar os ativos posteriormente (você ainda é responsável por escrever uma cópia de email e configurar quaisquer páginas de aterrissagem).
* A IA do Marketo não pode acessar suas listas de públicos-alvo existentes automaticamente. Você deve conectar filtros de lista inteligente aos segmentos reais depois que o programa for criado.
* Programas complexos de várias etapas com lógica de ramificação avançada podem precisar de refinamento manual após a criação.
* Se o ambiente do Marketo usar convenções de nomenclatura ou estruturas de pastas. Especifique-os no seu resumo para que o programa seja criado no lugar certo.
