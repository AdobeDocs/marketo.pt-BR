---
description: Diálogos - Documentos do Marketo - Documentação do produto
title: Diálogos
hide: true
hidefromtoc: true
source-git-commit: 1a1d4cb7e013253ce7189150486ba03ea02d877d
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

# Diálogos {#dialogues}

As caixas de diálogo são as conversas de chat específicas configuradas. Eles podem ser personalizados por aparência, assim como o que é dito e quem vê.

## Criar uma nova caixa de diálogo {#create-a-new-dialogue}

1. Clique em **Diálogos**.

PICC

1. Clique no botão **Criar novo**.

PICC

1. Insira um nome (a descrição é opcional), defina o nível de prioridade e clique em **Save**.

PICC

>[!NOTE]
>
>EXPLICAR NÍVEL DE PRIORIDADE

## Critérios de público-alvo {#audience-criteria}

Semelhante às Smart Lists da Marketo, os atributos de Critérios de público-alvo permitem que você defina seu público-alvo.

Há vários atributos para escolher. Neste exemplo, estamos direcionando todos os leads conhecidos na Califórnia que trabalham em uma empresa com mais de 50 funcionários.

1. Pegue o atributo Estado de lead e arraste-o para a direita.

PICC

1. __ Está definido por padrão. No campo Selecionar valores , digite CA (também é possível clicar no menu suspenso e selecionar na lista).

PICC

1. Pegue o atributo Company Size e arraste-o para a direita.

PICC

1. Clique no menu suspenso do operador e selecione Maior que.

PICC

1. Digite 50 e clique em outro lugar na tela para salvar.

PICC

COMO CAPTURAR LEADS ANON

OBSERVAÇÃO - talvez tenha mencionado como inferido funciona/mostra um caso de uso, o email de cliente potencial está vazio

## Adicionar grupos {#add-groups}

Você também tem a opção de agrupar atributos, caso queira ter todos os atributos específicos junto com &quot;qualquer&quot; outro.

TERMINAR ISSO

## Destino {#target}

É aqui que você insere as URLs específicas nas quais deseja que uma caixa de diálogo específica seja exibida.

Formatos aceitáveis:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>O uso de um asterisco atua como um curinga abrangente. Assim, `https://*.website.com` colocaria a caixa de diálogo em cada página do site, incluindo subdomínios (por exemplo: `support.website.com`). E `https://website.com/folder/*` colocaria a caixa de diálogo em cada página HTML na pasta subsequente (por exemplo: nesse caso, considere que a pasta é &quot;esportes&quot;, portanto: website.com/sports/baseball.html, website.com/sports/football.html etc.).

## Designer de fluxo {#stream-designer}

O designer de fluxo contém cartões diferentes que podem ser adicionados para moldar a conversa de bate-papo.

TABELA

Mensagem: Use quando quiser fazer uma declaração sem nenhuma resposta necessária (por exemplo: &quot;Oi! Todos os itens estão 25% de desconto hoje com código SAVE25.&quot;)

Pergunta: Use quando quiser fazer uma pergunta de múltipla escolha, da qual você fornece as respostas disponíveis (por exemplo: Em que tipo de veículo você está interessado? Respostas = SUV, Compacto, Caminhão etc.)

Captura de informações: Use quando desejar coletar informações. Os três campos a serem escolhidos são Endereço de email, Número de telefone e Texto (o que permite que o visitante grave sua própria mensagem).

Programador de Compromissos: Fornece ao visitante um calendário de datas disponíveis para agendar um acompanhamento. A disponibilidade do calendário reflete [o próximo agente na linha](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing).

Objetivo: Este é o único cartão que os visitantes não verão. Cabe a você determinar em qual ponto uma meta é alcançada dentro do chat específico (por exemplo: se coletar o email do visitante for seu objetivo, coloque o cartão Meta após Captura de informações no fluxo.)

POSSÍVEL SEÇÃO PRÓPRIA

MOSTRAR EXEMPLOS ABAIXO