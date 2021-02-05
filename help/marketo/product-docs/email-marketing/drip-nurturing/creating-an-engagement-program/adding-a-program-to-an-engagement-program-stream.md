---
unique-page-id: 10098134
description: Adicionar um Programa a um fluxo de Programa de envolvimento - Documentos do marketing - Documentação do produto
title: Adicionando um Programa a um fluxo de Programa de envolvimento
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


# Adicionando um Programa a um fluxo de Programa de envolvimento {#adding-a-program-to-an-engagement-program-stream}

## Por que usar um programa aninhado em um fluxo de programa de envolvimento? {#why-use-a-nested-program-in-an-engagement-program-stream}

É fácil adicionar um email a um stream em um programa de envolvimento, e funciona bem. No entanto, se suas necessidades de negócios forem mais complexas, pode fazer sentido colocar o email dentro de um programa. Por exemplo, talvez você queira:

* Enviar um email para um subgrupo de pessoas no stream
* Enviar emails *diferentes* para subgrupos dentro do fluxo
* Incluir landings page, formulários ou outros ativos na criação
* Ativar atribuição multitoque
* Adicionar etapas de fluxo extras, como emails de alerta

## O que acontece quando você usa um programa em um fluxo? {#what-happens-when-you-use-a-program-in-a-stream}

Ao usar um programa aninhado, a decisão de enviar um email para uma pessoa é baseada na associação ao programa e na ID do programa.

* Se você não for membro de um programa, receberá todos os emails que fazem parte do programa uma vez
* Se você for membro do programa, não receberá o email
* Se você não for mais um membro, mas tiver recebido o email mais cedo por meio desse programa, você não receberá o email

Quando você usa um programa em um fluxo, não importa se você já recebeu esse email específico antes. Desde que o email não tenha sido enviado antes de *no programa específico*, você poderá recebê-lo novamente.

Pode tornar-se complicado misturar emails e programas em um programa de envolvimento. Você pode querer usar um ou o outro.

>[!TIP]
>
>Certifique-se de usar um filtro **Membro do Programa de envolvimento** na sua lista inteligente.

## O que acontece com pessoas que não atendem aos critérios de lista inteligente? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

No evento de que alguém é filtrado da lista inteligente da campanha inteligente de um programa aninhado, ele não move para a próxima parte do conteúdo durante a transmissão atual. Eles irão para a próxima parte do conteúdo no fluxo para a conversão *seguinte*.

## O que um programa aninhado contém? {#what-does-a-nested-program-contain}

Um programa aninhado bem projetado contém emails, relatórios e campanhas inteligentes. Faz sentido mantê-los juntos.

O e-mail que você usa pode viver no programa, em um programa diferente ou até mesmo no Design Studio. Onde ele vive dependerá de como você quiser usá-lo.

Alterações no relatórios com o local do email. Assim, por exemplo, se o email estiver no Design Studio, no Relatório de desempenho de email, todas as métricas serão mostradas em uma linha - as diferentes castas serão combinadas. No entanto, no Relatório de desempenho do fluxo de envolvimento, os diferentes envios são exibidos separadamente.

>[!CAUTION]
>
>Se você quiser reenviar algo, é mais seguro criar um novo programa e campanha inteligente.

>[!MORELIKETHIS]
>
>* [Adicionar conteúdo a um fluxo](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [Como entender Programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)

