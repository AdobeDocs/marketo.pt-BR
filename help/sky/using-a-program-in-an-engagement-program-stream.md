---
title: using-a-programa-in-an-engagement-programa-stream
description: Uso de um Programa em um fluxo de Programa de envolvimento
translation-type: tm+mt
source-git-commit: 73df78512226c6c57625a73f14ba8b00bea195bd
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---


# Uso de um Programa em um fluxo de Programa de envolvimento

## Por que usar um programa aninhado em um fluxo de programa de envolvimento?

É fácil adicionar um email a um stream em um programa de envolvimento, e funciona bem. No entanto, se suas necessidades de negócios forem mais complexas, pode fazer sentido colocar o email dentro de um programa. Por exemplo, talvez você queira:

* Enviar um email para um subgrupo de pessoas no stream
* Enviar emails _diferentes_ para subgrupos dentro do fluxo
* Incluir landings page, formulários ou outros ativos no programa de envolvimento
* Ativar atribuição multitoque
* Adicionar etapas de fluxo extras, como emails de alerta

## O que acontece quando você usa um programa em um fluxo?

Ao usar um programa aninhado, a decisão de enviar um email para uma pessoa é baseada na associação ao programa e na ID do programa.

* Se você não for membro do programa, receberá emails que fazem parte do programa uma vez
* Se você for membro do programa, não receberá o email
* Se você não for mais um membro, mas já tiver recebido o email mais cedo por meio desse programa, você não receberá o email

Quando você usa um programa em um fluxo, não importa se você já recebeu esse email específico antes. Desde que o email não tenha sido enviado antes de _no programa específico_, você poderá recebê-lo novamente.

Pode tornar-se complicado misturar emails e programas em um programa de envolvimento. Você pode querer usar um ou o outro.

>[!TIP]
>
>Certifique-se de usar um filtro de Programa Membro de envolvimento em sua lista inteligente.

## O que acontece com pessoas que não atendem aos critérios de lista inteligente?

No evento de que alguém é filtrado da lista inteligente da campanha inteligente de um programa aninhado, ele não move para a próxima parte do conteúdo durante a transmissão atual. Eles irão para a próxima parte do conteúdo no fluxo para a conversão _seguinte_.

## O que um programa aninhado contém?

Um programa aninhado bem projetado contém emails, relatórios e campanhas inteligentes. Faz sentido mantê-los juntos.

O e-mail que você usa pode viver no programa, em um programa diferente ou até mesmo no Design Studio. Onde ela vive depende de como você quer usá-la.

Alterações no relatórios com o local do email. Assim, por exemplo, se o email estiver no Design Studio, no Relatório de desempenho de email, todas as métricas serão mostradas em uma linha - as diferentes castas serão combinadas. No entanto, no Relatório de desempenho do fluxo de envolvimento, os diferentes envios são exibidos separadamente.

>[!CAUTION]
>
>Se você quiser reenviar algo, é mais seguro criar um novo programa e campanha inteligente.
