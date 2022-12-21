---
unique-page-id: 10098134
description: Adicionar um programa a um fluxo do programa de envolvimento - Documentos da Marketo - Documentação do produto
title: Adicionar um programa a um fluxo do programa de envolvimento
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Adicionar um programa a um fluxo do programa de envolvimento {#adding-a-program-to-an-engagement-program-stream}

## Por que usar um programa aninhado em um fluxo de programa de envolvimento? {#why-use-a-nested-program-in-an-engagement-program-stream}

É fácil adicionar um email a um fluxo em um programa de envolvimento e ele funciona bem. No entanto, se as necessidades de sua empresa são mais complexas, pode fazer sentido colocar o email dentro de um programa. Por exemplo, talvez você queira:

* Enviar um email para um subgrupo de pessoas no stream
* Enviar *different* emails para subgrupos no fluxo
* Incluir landing pages, formulários ou outros ativos na nuvem
* Habilitar atribuição multitoque
* Adicionar etapas de fluxo extras, como emails de alerta

## O que acontece quando você usa um programa em um stream? {#what-happens-when-you-use-a-program-in-a-stream}

Ao usar um programa aninhado, a decisão de enviar um email para uma pessoa é baseada na associação do programa e na ID do programa.

* Se você não for membro de um programa, receberá todos os emails que fazem parte do programa uma vez
* Se você for membro do programa, não receberá o email
* Se você não for mais um membro, mas tiver recebido o email anteriormente por meio desse programa, você não receberá o email

Quando você usa um programa em um stream, não importa se você já recebeu esse email específico antes. Contanto que o email não tenha sido enviado antes *nesse programa específico*, você poderá recebê-lo novamente.

Ele pode complicar a combinação de emails e programas em um programa de engajamento. Talvez você queira usar um ou o outro.

>[!TIP]
>
>Certifique-se de usar um **Membro do Programa de Envolvimento** na sua lista inteligente.

## O que acontece com as pessoas que não atendem aos critérios da lista inteligente? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

Caso alguém seja filtrado da lista inteligente da campanha inteligente de um programa aninhado, ele não avança para a próxima parte do conteúdo durante o lançamento atual. Eles avançarão para a próxima parte do conteúdo no fluxo para a variável *following* elenco.

## O que um programa aninhado contém? {#what-does-a-nested-program-contain}

Um programa aninhado bem projetado contém emails, relatórios e campanhas inteligentes. Faz sentido mantê-los juntos.

O e-mail usado pode estar ativo no programa, em um programa diferente ou até mesmo no Design Studio. Onde ele está dependerá de como você deseja usá-lo.

Relatar alterações com o local do email. Assim, por exemplo, se o email estiver no Design Studio, no Relatório de desempenho de email, todas as métricas serão mostradas em uma linha - os diferentes casts serão combinados. No entanto, no Relatório de desempenho do fluxo de envolvimento, os diferentes envios são exibidos separadamente.

>[!CAUTION]
>
>Se você quiser reenviar algo, é mais seguro criar um novo programa e uma campanha inteligente.

>[!MORELIKETHIS]
>
>* [Adicionar conteúdo a um fluxo](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [Noções básicas sobre programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)

