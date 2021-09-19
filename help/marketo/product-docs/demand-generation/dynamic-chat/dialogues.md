---
description: Diálogos - Documentos do Marketo - Documentação do produto
title: Diálogos
hide: true
hidefromtoc: true
source-git-commit: c46902686f1d5af63a51f5eaae2dc0e6afe99629
workflow-type: tm+mt
source-wordcount: '273'
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

Há vários atributos para escolher. Neste exemplo, estamos escolhendo Estado de lead _is_ Califórnia e o Tamanho da empresa _é maior que_ 50.

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
>O uso de um asterisco atua como um curinga abrangente. Assim, `https://*.website.com` colocaria a caixa de diálogo em cada página do site, incluindo subdomínios (por exemplo: support.site.com). E `https://website.com/folder/*` colocaria a caixa de diálogo em cada página HTML na pasta subsequente (por exemplo: nesse caso, considere que a pasta é &quot;esportes&quot;, portanto: website.com/sports/baseball.html, website.com/sports/football.html etc.).
