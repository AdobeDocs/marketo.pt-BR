---
unique-page-id: 10096409
description: Evite enviar conteúdo duplicado - Documentos do Marketo - Documentação do produto
title: Evite enviar conteúdo duplicado
exl-id: fd7118e8-6e34-4973-8aa5-effb774447fd
source-git-commit: daaf3dc9b4da95db743409c6e2a6c426ed00e9c7
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 3%

---

# Evite enviar conteúdo duplicado {#avoid-sending-duplicate-content}

Você já recebeu o mesmo email duas vezes? Irritante, não é?

Aqui estão sete cenários possíveis e resultados que devem ser levados em consideração para impedir o envio de uma mesma mensagem duas vezes com programas de engajamento.

## Cenários {#scenarios}

| O email é enviado de | A pessoa é | A pessoa recebe email |
|---|---|---|
| Uma campanha em um programa padrão separado, independente | Não é membro do programa padrão | Sim |
| Uma campanha em um programa padrão separado, independente | Um membro do programa padrão | Não |
| Uma campanha dentro de um programa padrão que é acionada por um elenco dentro da variável **same** Programa CEE | Um membro do programa padrão | Não |
| Uma campanha dentro de um programa padrão que é acionada por um elenco dentro da variável **same** Programa CEE | Não é membro do programa padrão | Sim |
| Uma campanha dentro de um programa padrão que é acionada por um elenco dentro de um **different** Programa CEE | Um membro do programa padrão | Não |
| Uma campanha dentro de um programa padrão que é acionada por um elenco dentro de um **different** Programa CEE | Não é membro do programa padrão | Sim |
| A **different** Programa CEE utilizando um fluxo inteligente | Membro de ambos os programas CEE | Não |
