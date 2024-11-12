---
description: Notas de versão do Dynamic Chat - Documentação do Marketo - Documentação do produto
title: Notas de versão do Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: 342d52439a21668a3bf94e5149710b20e4ddb83f
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 4%

---

# Notas de versão do Dynamic Chat TEMP {#dynamic-chat-release}

## Versão de setembro/outubro de 2024 {#august-release}

### Análise aprimorada de bate-papo ao vivo {#enhanced-live-chat-analytics}

Vários aprimoramentos foram feitos no Painel do Analytics, incluindo:

* Contagem total solicitada do bate-papo ao vivo: número de visitantes solicitados para um &quot;Bate-papo com o agente&quot;

* Total de bate-papos ao vivo conectados: número de visitantes conectados versus total solicitado para um &quot;Bate-papo com o agente&quot;

* Total de solicitações de bate-papo em tempo real perdidas: número de visitantes autônomos versus total solicitado para um &quot;bate-papo com o agente&quot;

* Duração média do chat em minutos: analise a &quot;duração média do chat&quot; entre visitantes e seus agentes

* Tempo médio de resposta do agente em segundos: analise o &quot;tempo médio&quot; gasto pelos agentes para responder às perguntas e respostas do bate-papo ao vivo

* Painel diário: solicitações de bate-papo ao vivo conectadas com sucesso, solicitações de bate-papo ao vivo perdidas, classificar e filtrar atividades recentes de bate-papo ao vivo

CAPTURA DE TELA

### Pontuação da conversa

Quantifique seus leads com base na qualidade da interação de chat e use essa métrica como um Acionador/Filtro em Campanhas inteligentes do Marketo Engage. Use o novo atributo _pontuação da conversa_ nas seguintes atividades:

* Engajado com um diálogo
* Envolvido com um fluxo de conversa
* Envolvido com um agente

**O que observar:**

* O valor da pontuação será de 0, 1, 2, 3 (o valor padrão é nulo)

* Uma vez concluída ou descartada a conversa, na atividade, salve o valor de pontuação e publique que que ele não pode ser editado????????????????????????????? (o que isso significa)

* Definição de uma pontuação:

   * Na caixa de entrada do agente - durante um chat ao vivo, o agente pode atualizar ou definir uma pontuação para a conversa, que é armazenada na atividade de conversa

   * No designer de fluxo - no cartão de meta, o usuário pode atualizar ou definir uma pontuação para a conversa

CAPTURA DE TELA

CAPTURA DE TELA

CAPTURA DE TELA

### Nova Lógica de Criação de Cliente Potencial {#new-lead-creation-logic}

Se um cliente potencial preencher um formulário com o email `abc@test.com` e for cookie como xyz, depois preencher o mesmo formulário com o email `def@test.com`, um novo cliente potencial será criado, mas o cookie xyz será associado ao novo cliente potencial e removido do cliente potencial `abc@test.com`.

A partir de então, `abc@test.com` será um cliente em potencial sem cookie. UM CHUMBO?

Assim, quando um visitante com cookie abc chega em uma página e fornece uma ID de email como `abc@p.com`:

TABELA
