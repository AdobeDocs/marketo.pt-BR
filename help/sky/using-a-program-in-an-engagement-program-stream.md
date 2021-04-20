---
title: usar-um-programa-em-um-envolvimento-programa-stream
description: Uso de um programa em um fluxo de programa de envolvimento
exl-id: b75c926d-d545-4557-970f-c893818d9566
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Uso de um programa em um fluxo de programa de envolvimento

## Por que usar um programa aninhado em um fluxo de programa de envolvimento?

É fácil adicionar um email a um fluxo em um programa de envolvimento e ele funciona bem. No entanto, se as necessidades de sua empresa são mais complexas, pode fazer sentido colocar o email dentro de um programa. Por exemplo, talvez você queira:

* Enviar um email para um subgrupo de pessoas no stream
* Enviar _emails diferentes_ para subgrupos no fluxo
* Incluir landing pages, formulários ou outros ativos no programa de envolvimento
* Habilitar atribuição multitoque
* Adicionar etapas de fluxo extras, como emails de alerta

## O que acontece quando você usa um programa em um stream?

Ao usar um programa aninhado, a decisão de enviar um email para uma pessoa é baseada na associação do programa e na ID do programa.

* Se você não for membro do programa, receberá todos os emails que fazem parte do programa uma vez
* Se você for membro do programa, não receberá o email
* Se você não for mais um membro, mas já tiver recebido o email anteriormente por meio desse programa, você não receberá o email

Quando você usa um programa em um stream, não importa se você já recebeu esse email específico antes. Contanto que o email não tenha sido enviado antes de _no programa específico_, você poderá recebê-lo novamente.

Ele pode complicar a combinação de emails e programas em um programa de engajamento. Talvez você queira usar um ou o outro.

>[!TIP]
>
>Certifique-se de usar um filtro Membro do programa de envolvimento em sua lista inteligente.

## O que acontece com as pessoas que não atendem aos critérios da lista inteligente?

Caso alguém seja filtrado da lista inteligente da campanha inteligente de um programa aninhado, ele não avança para a próxima parte do conteúdo durante o lançamento atual. Eles avançarão para a próxima parte do conteúdo no fluxo para a conversão _a seguir_.

## O que um programa aninhado contém?

Um programa aninhado bem projetado contém emails, relatórios e campanhas inteligentes. Faz sentido mantê-los juntos.

O e-mail usado pode estar ativo no programa, em um programa diferente ou até mesmo no Design Studio. Onde ele está depende de como você quer usá-lo.

Relatar alterações com o local do email. Assim, por exemplo, se o email estiver no Design Studio, no Relatório de desempenho de email, todas as métricas serão mostradas em uma linha - os diferentes casts serão combinados. No entanto, no Relatório de desempenho do fluxo de envolvimento, os diferentes envios são exibidos separadamente.

>[!CAUTION]
>
>Se você quiser reenviar algo, é mais seguro criar um novo programa e uma campanha inteligente.
