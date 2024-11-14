---
description: Notas de versão do Dynamic Chat - Documentação do Marketo - Documentação do produto
title: Notas de versão do Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
exl-id: 12130dee-2dbf-4e71-b542-30d4732b1067
source-git-commit: cc8de935451fe5d6dc9c8dad19962391d8ed3535
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 3%

---

# Notas de versão do Dynamic Chat TEMP {#dynamic-chat-release}

## Versão de setembro/outubro de 2024 {#august-release}

### Análise de chat ao vivo aprimorada {#enhanced-live-chat-analytics}

Vários aprimoramentos foram feitos no Painel do Analytics, incluindo:

* Contagem total solicitada do bate-papo ao vivo: número de visitantes solicitados para um &quot;bate-papo com o agente&quot;

* Total de bate-papos ao vivo conectados: número de visitantes conectados versus total solicitado para um &quot;bate-papo com o agente&quot;

* Total de solicitações de bate-papo em tempo real perdidas: número de visitantes autônomos versus total solicitado para um &quot;bate-papo com o agente&quot;

* Duração média do chat em minutos: analise a &quot;duração média do chat&quot; entre visitantes e seus agentes

* Average Agent Response Time in Seconds: analise o &quot;tempo médio&quot; gasto pelos agentes para responder às perguntas e respostas do bate-papo ao vivo

* Painel diário: solicitações de bate-papo ao vivo conectadas com sucesso, solicitações de bate-papo ao vivo perdidas, classificar e filtrar atividades recentes de bate-papo ao vivo

CAPTURA DE TELA

### Pontuação de conversa {#conversation-scoring}

Quantifique seus leads com base na qualidade da interação de chat e use essa métrica como um Acionador/Filtro em Campanhas inteligentes do Marketo Engage. Use o novo atributo _pontuação da conversa_ nas seguintes atividades:

* Engajado com um diálogo
* Envolvido com um fluxo de conversa
* Envolvido com um agente

**O que observar:**

* O valor da pontuação será de 0, 1, 2, 3 (o valor padrão é nulo)

* Quando a conversa for concluída ou descartada, na atividade, salve o valor de pontuação e publique que que não pode ser editado   ???? (o que essa frase significa)

* Definição de uma pontuação:

   * Na caixa de entrada do agente - durante um chat ao vivo, o agente pode atualizar ou definir uma pontuação para a conversa, que é armazenada na atividade de conversa

   * No designer de fluxo - no cartão de meta, o usuário pode atualizar ou definir uma pontuação para a conversa

CAPTURA DE TELA

CAPTURA DE TELA

CAPTURA DE TELA

### Nova lógica de criação de clientes potenciais {#new-lead-creation-logic}

Se um cliente potencial preencher um formulário com o email `abc@test.com` e for cookie como xyz, depois preencher o mesmo formulário com o email `def@test.com`, um novo cliente potencial será criado, mas o cookie xyz será associado ao novo cliente potencial e removido do cliente potencial `abc@test.com`.

A partir de então, `abc@test.com` será um cliente em potencial sem cookie. LEAD ANÔNIMO?

Assim, quando um visitante com cookie abc chega em uma página e fornece uma ID de email como `abc@test.com`:

TABELA

### Tempo de carregamento do fluxo de conversa otimizado {#optimized-conversation-flow-load-time}

Para melhorar a experiência do usuário, um carregador shimmer agora é exibido em vez de um espaço em branco enquanto o fluxo de conversa é carregado. CONVERSA OU CONVERSA???

**Antes**

GIF

**Depois**

GIF

### Opção para herdar fonte {#option-to-inherit-font}

Agora você pode ativar o chatbot para herdar diretamente a fonte da página da Web em que está sendo hospedada, em vez de gerenciar a fonte da marca no Dynamic Chat. Ao habilitar essa opção, o chatbot utiliza a fonte definida na tag `<body>` da página.

CAPTURA DE TELA

### Integração do Demandbase com o Dynamic Chat {#demandbase-integration-with-dynamic-chat}

Os usuários do Demandbase podem trazer sua própria licença do Demandbase e ativar a integração. Use os atributos de pessoa do Demandbase para direcionamento de caixa de diálogo, identidade visual condicional e roteamento personalizado.

A resolução desses valores de atributo em relação a um lead seria feita em tempo real e é armazenada no respectivo perfil de lead.
